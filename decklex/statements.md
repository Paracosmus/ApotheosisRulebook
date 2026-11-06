---
label: Instruções
icon: list-ordered
order: 115
---
# Instruções
> As instruções da Decklex

As listas de uma [função](function.md), como a `validation` e o `body`, são feitas de instruções, que rodam em ordem. Toda instrução escreve todos os seus campos. Cada uma também grava o seu resultado numa [variável](variables.md) com o nome dela: `$Expr`, `$Return`, `$If` e `$For`.

| Tipo          | O que é                                                                                                                       | {.compact}
| ---           | ---                                                                                                                           |
| `Texto`       | Um texto entre aspas.                                                                                                         |
| `Valor`       | Um número inteiro, um texto, `true` ou `false`, ou um bloco. Um texto que começa com `$` é lido como a variável com esse nome. |
| `[Instrução]` | Uma lista de instruções. Uma lista vazia vale `true`.                                                                         |
| `Ação`        | Uma [ação de jogo](actions.md), escrita como um objeto com o seu `type`.                                                      |

Um bloco é uma lista de instruções usada como valor. Ele roda e vale o resultado da sua última instrução.

---

## Básicas

[//]: <> (=========================================================================================)

:::api
### Expr

Calcula uma [expressão](expressions.md). Uma atribuição a `$nome` grava a variável, só se a expressão inteira der certo.

```rust !#1 Campos
expressão: Texto      // Escrita direto: { "Expr": "<expressão>" }
```

**Resultado:** o valor da expressão, `true` numa atribuição, ou `false` se a expressão não puder ser calculada.

==- [!badge variant="success" size="l" icon="code" corners="Square" text="Exemplo"]
```json
{ "Expr": "$hero_level += 1" }
```
===
:::
<br>


[//]: <> (=========================================================================================)

:::api
### Return

Encerra a função com um valor, mesmo de dentro de um [If](#if) ou de um [For](#for).

```rust !#1 Campos
valor: Valor          // Escrito direto: { "Return": <valor> }
```

**Resultado:** o valor.

Dentro de um requisito da `validation` ou de um bloco, o `Return` encerra só aquele requisito ou bloco, que passa a valer o valor do `Return`.

==- [!badge variant="success" size="l" icon="code" corners="Square" text="Exemplo"]
```json
{ "Return": "$hero_level" }
```
==- [!badge variant="success" size="l" icon="code" corners="Square" text="Bloco"]
A segunda instrução lê o resultado da primeira, e o bloco vale **6**:
```json
{ "Return": [{ "Expr": "1 + 1" }, { "Expr": "$Expr * 3" }] }
```
===
:::
<br>


---

## Controle de fluxo

[//]: <> (=========================================================================================)

:::api
### If

Roda uma de duas listas de instruções, conforme uma condição.

```rust !#1-3 Campos
condition: [Instrução]    // Julgada como um requisito: só passa se terminar em true
then: [Instrução]         // Roda se a condição passar
otherwise: [Instrução]    // Roda se não passar. Escreva [] quando não houver nenhuma
```

**Resultado:** o resultado da lista que rodou.

!!!
O número **1** não é `true`. Uma condição que termina em **1**, ou numa expressão que não pode ser calculada, roda o `otherwise`.
!!!

==- [!badge variant="success" size="l" icon="code" corners="Square" text="Exemplo"]
```json
{ "If": {
    "condition": [{ "Expr": "$base >= 3" }],
    "then": [{ "Expr": "$hero_level += 1" }],
    "otherwise": []
} }
```
==- [!badge variant="success" size="l" icon="code" corners="Square" text="Senão, se"]
Um `If` dentro do `otherwise` faz um "senão, se". Aqui o herói ganha **+2** de nível com `$base` a partir de **5**, e **+1** com `$base` de **3** ou **4**:
```json
{ "If": {
    "condition": [{ "Expr": "$base >= 5" }],
    "then": [{ "Expr": "$hero_level += 2" }],
    "otherwise": [
        { "If": {
            "condition": [{ "Expr": "$base >= 3" }],
            "then": [{ "Expr": "$hero_level += 1" }],
            "otherwise": []
        } }
    ]
} }
```
===
:::
<br>


[//]: <> (=========================================================================================)

:::api
### For

Repete uma lista de instruções uma vez para cada número inteiro de `from` até `to`, incluindo os dois.

```rust !#1-4 Campos
variable: Texto       // Recebe o número de cada volta, escrita com $: "$i"
from: Valor           // O primeiro número
to: Valor             // O último número, incluído
body: [Instrução]     // As instruções de cada volta
```

**Resultado:** o resultado da última volta.

- Se `from` for maior que `to`, o `body` não roda, e o resultado é `true`.
- Depois do laço, a variável guarda o último número.
- Um `For` de mais de **1000** voltas é recusado inteiro: o `body` não roda, e o resultado é `false`.

!!!warning A variável do laço é da partida
`$i` é uma [variável](variables.md) como as outras: todos os efeitos da mesma ação veem o mesmo `$i`. Dois `For`, um dentro do outro, precisam de variáveis com nomes diferentes.
!!!

==- [!badge variant="success" size="l" icon="code" corners="Square" text="Exemplo"]
Soma ao nível os números de **1** até `$base`:
```json
{ "For": {
    "variable": "$i",
    "from": 1,
    "to": "$base",
    "body": [{ "Expr": "$hero_level += $i" }]
} }
```
==- [!badge variant="success" size="l" icon="code" corners="Square" text="Return no laço"]
Um `Return` dentro do `body` encerra o laço e a função. Esta função devolve **4**, o primeiro número cujo quadrado passa de **10**:
```json
{ "For": {
    "variable": "$i",
    "from": 1,
    "to": 10,
    "body": [
        { "If": {
            "condition": [{ "Expr": "$i * $i > 10" }],
            "then": [{ "Return": "$i" }],
            "otherwise": []
        } }
    ]
} }
```
===
:::
<br>


---

## Ações de jogo

[//]: <> (=========================================================================================)

:::api
### Command

Faz uma [ação de jogo](actions.md), como mover uma carta ou mudar a {{ hp }} de uma peça.

```rust !#1 Campos
ação: Ação            // Escrita direto: { "Command": { "type": "<ação>", … } }
```

**Resultado:** `true` se a ação foi feita, ou `false` se foi recusada.

- O efeito faz a ação por conta própria, e ela entra no histórico da partida sem jogador. Todas as checagens da ação valem.
- Uma ação do Mestre do Jogo, como criar um time, é sempre recusada.
- Uma ação recusada não muda nada. As ações que o efeito já fez continuam feitas, e a função segue para a próxima instrução.
- As variáveis continuam valendo depois da ação.
- Um id é escrito por extenso. Ainda não existe forma de um efeito obter o id de uma carta ou de um herói da partida.

==- [!badge variant="success" size="l" icon="code" corners="Square" text="Exemplo"]
```json
{ "Command": {
    "type": "ChangePieceHealth",
    "source": { "Character": { "Hero": "3fa85f64-5717-4562-b3fc-2c963f66afa6" } },
    "amount": -2
} }
```
===
:::
<br>


---

## O que ainda falta

- Outras repetições (`while`, "para cada"), `break` e `continue`, e `switch`.
