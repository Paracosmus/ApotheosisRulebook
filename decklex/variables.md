---
label: Variáveis
icon: package
order: 110
---

# Variáveis

Uma variável é um valor com nome, escrito com `$` na frente: `$base`, `$hero_level`. As variáveis pertencem à partida, não ao efeito. Todos os efeitos que rodam durante uma mesma ação leem e gravam as mesmas variáveis, e o jogo apaga todas quando a ação termina.

Uma variável que ainda não recebeu valor vale **0**.

---

## Variáveis do jogo

| Variável              | Quem grava                                                  | O que guarda                                                                                  | {.compact}
| ---                   | ---                                                         | ---                                                                                           |
| `$base`               | O jogo, antes do primeiro efeito de uma propriedade         | A soma dos bônus da propriedade. É a mesma para todos os efeitos dessa propriedade.           |
| `$<nome da propriedade>` | O jogo começa com o valor de `$base`, e cada efeito o altera | O valor como os efeitos anteriores o deixaram. O que o último efeito deixa é o valor final.   |
| `$Expr`, `$Return`, `$If`, `$For` | Cada [instrução](statements.md)                 | O último resultado daquela instrução.                                                         |
| Qualquer outro `$nome` | Um `Expr` que atribui a ele, ou um `For` que o usa como variável | O valor atribuído, até o fim da ação.                                               |

As propriedades e os seus bônus estão em [Propriedades](properties.md).

!!!secondary Exemplo
Um herói tem uma {{ house }} de nível **1** e uma {{ class }} de nível **2**. Ao calcular `hero_level`, o jogo grava **3** em `$base` e em `$hero_level`. O primeiro efeito faz `$hero_level += 1` e deixa **4**. O segundo lê **4** em `$hero_level` e **3** em `$base`.
!!!

---

## Cuidados

!!!warning Só a variável da propriedade calculada é lida de volta
Um efeito que também grava a variável de outra propriedade (`$hero_agility += 1; $hero_strength += 1`) tem essa gravação ignorada no cálculo atual. A outra propriedade roda o efeito de novo quando for calculada. Ler a variável de outra propriedade dá o que foi deixado nela por último, não o valor dela.
!!!

!!!warning `$base` pode ser alterada
Nada impede uma função de gravar `$base`. Os efeitos seguintes da mesma propriedade leem o número alterado.
!!!

- **Nomes em snake_case.** `$hero-level` é lido como `$hero - level`.
