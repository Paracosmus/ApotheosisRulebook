---
label: Dado
icon: dice
order: 35
---

# Dado

{{ briefing `Die` `Inúmeras ações no jogo são resolvidas através da rolagem de dados, incluindo testes, ataques, efeitos, entre outros.` }}

Os dados utilizados são de seis faces, representados pela sigla **D6**. Em alguns casos, serão necessários dados com menos faces, então o dado de seis faces deve ser tratado da seguinte forma:

| {{ d1d6 }} D6 | {{ d1d3 }} D3  | {{ d1d2 }} D2 |
|--- |--- |---
| Role o dado de 6 faces e utilize o número obtido como resultado. | Considera-se o dado de 6 faces como um dado de 3 faces:<br/>• 1 e 2 = 1<br/>• 3 e 4 = 2<br/>• 5 e 6 = 3 | Considera-se o dado de 6 faces como um dado de 2 faces:<br/>• 1, 2 e 3 = 1<br/>• 4, 5 e 6 = 2

!!!light
Múltiplos dados são referidos na forma {{ e2d6 }}, {{ e3d2 }}, etc.
!!!

## Quem Rola os Dados

**Quando uma mecânica de jogo** determinar a rolagem de dados, o jogador que rola os dados é sempre o jogador que desencadeou a mecânica.

**Quando uma carta** determinar a rolagem de dados, o jogador que rola os dados é sempre o jogador que tem posse da carta no momento de sua ativação, ou quando a ativação for manual, o jogador que ativar a carta.

---

## Tipos de Dados

### Dado Principal

Do conjunto de dados rolados, um deles deve ser distinto dos demais, seja por ser rolado antes de todos ou por ter uma aparência diferente. Este é o dado principal.

O dado principal determina se houve uma [Rolagem Perfeita](#dados-extras-rolagem-perfeita) (valor natural 6). Como apenas ele é considerado para esse efeito, a chance de rolagem perfeita é sempre 1 em 6, independentemente do número de dados rolados.

### Dados Secundários

São todos os demais dados em uma rolagem de dados que não sejam o dado principal, nem sejam dados extras obtidos por uma rolagem crítica.

### Dados Extras (Rolagem Perfeita)

Quando o dado principal obtiver um 6 natural (rolagem perfeita), o jogador deve:

1. Rolar {{ e1d3 }} adicional e somar o resultado ao total da rolagem.
2. Se o valor natural no dado de 6 faces for novamente 6 (rolagem perfeita), rolar outro {{ e1d3 }} adicional.
3. Repetir o passo anterior até que o valor natural seja diferente de 6.

---

## Dado Aleatório

Em alguns casos, pode ser solicitada a rolagem de **Dados Aleatórios**. Isso significa que o jogador deve rolar os dados solicitados, ignorar quaisquer bônus e efeitos de carta que afetem a rolagem de dados e considerar apenas o valor obtido no dado.

Estes dados também não compartilham as características da carta ou mecânica que os solicitou.

Rolagens aleatórias seguem a mesma estrutura de conjunto de dados, tendo um dado principal, secundários e extras.

---
