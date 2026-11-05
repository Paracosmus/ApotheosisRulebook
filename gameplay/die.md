# Dado

|||{.briefing} [!badge text="Die" variant="ghost"]
  Inúmeras ações no jogo são resolvidas através da rolagem de dados, incluindo testes, ataques, efeitos, entre outros.
|||
    
O jogo usa dados de **2**, **3**, **4**, **5**, **6**, **8**, **10**, **12**, **20** e **100** faces, representados pela letra **D** seguida do número de faces, como **D6** ou **D20**.

Uma rolagem é escrita com o ícone do dado seguido pela notação de RPG: quantidade de dados, a letra *d* e o número de faces. Por exemplo, <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">2</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">10</span></span></span> e <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">20</span></span></span>.

Os dados D2, D3, D5 e D100 são rolados com outros dados, da seguinte forma:

| <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">2</span></span></span> | <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">3</span></span></span> | <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">5</span></span></span> | <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">100</span></span></span> |
|--- |--- |--- |---
| Considera-se o dado de 6 faces como um dado de 2 faces:<br/>• 1, 2 e 3 = 1<br/>• 4, 5 e 6 = 2 | Considera-se o dado de 6 faces como um dado de 3 faces:<br/>• 1 e 2 = 1<br/>• 3 e 4 = 2<br/>• 5 e 6 = 3 | Considera-se o dado de 10 faces como um dado de 5 faces:<br/>• 1 e 2 = 1<br/>• 3 e 4 = 2<br/>• 5 e 6 = 3<br/>• 7 e 8 = 4<br/>• 9 e 10 = 5 | Rolam-se 2 dados de 10 faces, um para a dezena e outro para a unidade:<br/>• em cada dado, o 10 vale 0<br/>• o resultado é a dezena seguida da unidade, como 7 e 3 = 73<br/>• 0 e 0 = 100

!!!light
Múltiplos dados são referidos pela quantidade antes da letra *d*, como em <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">2</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">6</span></span></span> e <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">3</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">2</span></span></span>.
!!!

## Quem Rola os Dados

**Quando uma mecânica de jogo** determinar a rolagem de dados, o jogador que rola os dados é sempre o jogador que desencadeou a mecânica.

**Quando uma carta** determinar a rolagem de dados, o jogador que rola os dados é sempre o jogador que tem posse da carta no momento de sua ativação, ou quando a ativação for manual, o jogador que ativar a carta.

---

## Tipos de Dados

### Valor Natural

O valor natural de um dado é o número que aparece na face do dado rolado, antes de qualquer leitura, bônus ou efeito. Em um D3, é o número do dado de 6 faces, de **1** a **6**. Em um D5, é o número do dado de 10 faces, de **1** a **10**.

### Dado Principal

Toda rolagem de dados tem um único dado principal: o primeiro dado da lista de dados rolados. Ele deve ser distinto dos demais, seja por ser rolado antes de todos ou por ter uma aparência diferente.

Apenas o dado principal é considerado para saber se houve uma [Rolagem Perfeita](#dados-extras-rolagem-perfeita).

!!!
Por exemplo, em uma rolagem de <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">2</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">6</span></span></span>, apenas um dos dois dados é o dado principal. Em uma rolagem de <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">8</span></span></span> + <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">4</span></span></span>, o D8 é o dado principal, porque vem primeiro na lista.
!!!

### Dados Secundários

São todos os demais dados em uma rolagem de dados que não sejam o dado principal, nem sejam dados extras obtidos por uma rolagem perfeita.

### Dados Extras (Rolagem Perfeita)

Uma rolagem perfeita acontece quando o dado principal tira o maior valor natural possível do dado rolado. Não é sempre o 6: é o maior número que aquele dado pode mostrar. Em um D3, é o 6 natural do dado de 6 faces. Em um D5, é o 10 natural do dado de 10 faces. Em um D20, é o 20. No <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">100</span></span></span>, o dado principal é o <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">10</span></span></span> da dezena, e a rolagem perfeita acontece quando ele tira **9**.

Em uma rolagem perfeita, o jogador deve:

1. Rolar <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">3</span></span></span> adicional e somar o resultado ao total da rolagem.
2. Se esse <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">3</span></span></span> também tirar o seu maior valor natural, o 6, rolar outro <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">3</span></span></span> adicional.
3. Repetir o passo anterior até que o valor natural seja diferente de 6.

---

## Dado Aleatório

Em alguns casos, pode ser solicitada a rolagem de **Dados Aleatórios**. Isso significa que o jogador deve rolar os dados solicitados, ignorar quaisquer bônus e efeitos que afetem a rolagem de dados e considerar apenas o valor obtido no dado.

Estes dados também não compartilham as características da carta ou mecânica que os solicitou.

Rolagens aleatórias seguem a mesma estrutura de conjunto de dados, tendo um dado principal, secundários e extras.

---
