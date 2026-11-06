# Função do efeito

A função é o que um efeito faz no jogo digital, escrita em JSON no campo `function` do efeito, dentro da definição da carta. O texto do efeito é o que o jogador lê. A função é o que o jogo executa.

```json
"function": {
    "annotation": [{ "Modifier": "hero_level" }],
    "validation": [],
    "body": [{ "Expr": "$hero_level += 1" }]
}
```

| Campo        | O que é                                                                                                     | {.compact}
| ---          | ---                                                                                                         |
| `annotation` | Para que a função serve. Veja [Anotações](#anotações).                                                      |
| `validation` | Uma lista de [instruções](statements.md) para cada item dos `requirements` do efeito. Cada lista precisa terminar em `true`, ou o corpo não roda. |
| `body`       | As [instruções](statements.md) que rodam depois que todas as validações passaram.                           |

Um efeito tem no máximo **1** função. Duas coisas que uma carta faz são dois efeitos, cada um com a sua.

---

## Quando a função roda

Hoje só uma coisa roda funções: o cálculo de uma [propriedade](properties.md), como o nível de um herói. Um efeito roda nesse cálculo quando:

- ele tem uma `function`;
- ele está em jogo: numa carta revelada de um herói em cena, numa carta de uma pilha utilizável ou numa técnica de um dummy, conforme as palavras-chave de escopo do efeito;
- ele tem a palavra-chave [<span class="keyword-activation">Permanente</span>](/gameplay/effect.md) (`ActivationPermanent`);
- a sua `annotation` lista `{ "Modifier": "<nome da propriedade>" }`.

Os efeitos rodam da maior prioridade para a menor. Efeitos com a mesma prioridade rodam na ordem em que o jogo os encontrou.

!!!warning Nada filtra o alvo
Todo efeito em jogo que modifica uma propriedade roda para **todo** herói cujo valor é pedido, não só para o dono da carta. Um efeito que deve valer só para o dono precisa verificar isso ele mesmo, com a função [`is_owner()`](expressions.md#do-jogo).
!!!

!!!secondary Exemplo
Uma carta com `$hero_level += 1` e sem validação, revelada na [<span class="main"><b>MESA</b></span>](/hero/table/) de um herói, dá **+1** de nível a todos os heróis em cena. Com `[[{ "Expr": "is_owner()" }]]` na `validation`, dá **+1** só ao herói dono da carta.
!!!

---

## Anotações

| Anotação                    | Significado                                                                                     | {.compact}
| ---                         | ---                                                                                             |
| `{ "Modifier": "<nome>" }`  | A função modifica a propriedade `<nome>`. Liste uma anotação para cada propriedade modificada.  |
| `{ "Priority": <número> }`  | Quando a função roda em relação às outras. Sem ela, a prioridade é **0**. Uma prioridade positiva roda antes das funções sem prioridade, e uma negativa roda depois. |

!!!secondary Exemplo
Um limite como "nível no máximo **5**" usa uma prioridade negativa, para rodar depois de todos os bônus:

```json
"annotation": [{ "Modifier": "hero_level" }, { "Priority": -1 }],
"body": [{ "Expr": "$hero_level = min($hero_level, 5)" }]
```
!!!

---

## O que ainda falta

- Ler mais da situação em que a função roda. Hoje as [funções do jogo](expressions.md#do-jogo) só comparam o agente com o dono da carta e o time dele.
- Gatilhos. Hoje só rodam modificadores permanentes.
- Efeitos de campanha.

As instruções que ainda faltam estão no fim da página [Instruções](/decklex/statements.md).
