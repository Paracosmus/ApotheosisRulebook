---
label: Glossário
layout: page
---

# Glossário

Este livro e as cartas do jogo utilizam termos com significados específicos. Abaixo estão listados esses termos e seus significados.

---

## A

[!card compact](gameplay/attachment.md)

## B

## C

[!card compact](gameplay/setup/campaign.md) [!card compact](/cards/)

[!card compact](gameplay/setup/) [!card compact](gameplay/counter.md)

## D

[!card compact](gameplay/die.md)

## E

## F

[!card compact](gameplay/setup/format/)

## G

## H

## I

[!card compact](battle/initiative.md)

## J

## K

## L

[!card compact](gameplay/limbo.md)

## M

[!card compact](battle/piece/dummy.md) [!card compact](gameplay/game-mode/battle-mode.md)

[!card compact](gameplay/game-mode/) [!card compact](gameplay/game-mode/story-mode.md)

## N

## O

## P

## Q

## R

## S

## T

## U

## V

[!card compact](gameplay/setup/variant.md) [!card compact](gameplay/game-mode/travel-mode.md)

## W

## X

## Y

## Z

---

## Cartas


| Termo          | Inglês        | Significado |
| -------------- | ------------- | ----------- |
| **Consumir**   | *Exhaust*     | Girar a carta para que ela fique na horizontal, em relação à {{ table }} do Herói |
| **Recuperar**  | *Recover*     | Girar a carta para que ela fique na vertical, em relação à {{ table }} do Herói |
| **Enviar**     | *Send*        | Mover uma carta para o destino especificado. Enviar sempre diz para onde a carta vai; quando o destino é um monte de cartas, ela é colocada no topo dele |
| **Descartar**  | *Discard*     | Colocar uma carta no topo do {{ tradingPost }} |
| **Enterrar**   | *Bury*        | Colocar uma carta no fundo de um monte de cartas. Diferente de descartar, enterrar sempre especifica o monte |
| **Banir**      | *Banish*      | Colocar uma carta no topo da pilha de {{ banished }}, removendo-a do jogo permanentemente |
| **Obter**      | *Get*         | É quando uma carta passa a estar sobre o controle do Herói. Quando uma carta é obtida a não ser que a situação especifique o contrário, o jogador decide onde colocá-la, seja em sua {{ table }}, {{ inv }} ou anexada a uma carta por mecânica de jogo |
| **Baixar**     | *Place*       | Adicionar uma carta à {{ table }} |
| **Puxar**      | *Draw*        | Pegar a carta do topo do baralho especificado e adicionar ao {{ inv }}, sem mostrá-la |
| **Revelar**    | *Reveal*      | Mostrar uma carta que está oculta, geralmente virando-a de face para cima, ou mostrando-a para todos os jogadores |
| **Ocultar**    | *Conceal*     | Esconder uma carta que está revelada, geralmente virando-a de face para baixo |
| **Buscar**     | *Search*      | Escolher uma carta na pilha ou baralho especificado, geralmente com limitações, mostrá-la e adicioná-la ao {{ inv }} |
| **Exilar**     | *Exile*       | Colocar uma carta no topo do [Limbo](/gameplay/limbo.md), removendo-a do jogo temporariamente, geralmente com condições para retornar ao jogo |
| **Resgatar**   | *Retrieve*    | Retornar uma carta do Limbo para o jogo, geralmente nas mesmas condições em que foi exilada |
| **Mesa**       | *Table*       | Local da área do jogo onde um Herói coloca suas cartas |
| **Ficha**      | *Sheet*       | Zona da {{ table }} do Herói onde estão suas cartas de ficha |
| **Zona Extra** | *Extra Zone*  | Zona da {{ sheet }} do Herói onde algumas mecânicas de jogo e efeitos de cartas podem colocar cartas de ficha extras |
| **Inventário** | *Inventory*   | Zona onde o Herói guarda as cartas que são de sua posse, mas não estão na sua {{ table }}. Geralmente representada pelas cartas seguradas na mão |

Ao enviar, descartar, enterrar, banir ou exilar uma carta para um monte, ela assume a orientação do monte para onde vai, conforme a [visibilidade](/gameplay/stack/index.md#visibilidade) dele.

---

## Tabuleiro

| Termo                    | Inglês          | Significado |
| ------------------------ | --------------- | ----------- |
| **Componente**           | *Component*     | Qualquer elemento físico do jogo, como cartas, peças, contadores, etc. |
| **Peça**                 | *Piece*          | Peão que representa um personagem ou objeto no tabuleiro de batalha |
| **Mover**                | *Move*          | Colocar uma peça em outra casa do tabuleiro |
| **Distância**            | *Distance*      | Alcance da ação ou movimento |
| **Trajeto / Trajetória** | *Trajectory*    | Conjunto de casas do tabuleiro por onde passa a linha reta entre o personagem que executa a ação e o alvo da ação |
| **Direção**              | *Direction*     | Vetor de direção de uma ação que parte de uma casa do tabuleiro até outra casa. É uma linha reta com comprimento infinito para ambos os lados e um sentido de direção |
| **Adjacente**            | *Adjacent Tile* | Aquilo que está em uma casa do tabuleiro, ou é uma casa do tabuleiro, que está ao lado de outra casa do tabuleiro. Não inclui casas diagonais |
| **Casa Bloqueada**       | *Blocked Tile*  | Casa que contém um obstáculo permanente, como uma parede. Nenhuma peça pode ocupá-la ou passar por ela, e trajetórias de ataques diretos não podem atravessá-la |
| **Casa Ocupada**         | *Occupied Tile* | Existe uma peça nesta casa do tabuleiro |
| **Casa Vazia**           | *Empty Tile*    | Qualquer casa do tabuleiro que não tenha uma peça |
| **Casa Desabilitada**    | *Disabled Tile* | Nenhuma peça pode ser colocada ou passar por esta casa do tabuleiro, para todos os fins, ela não existe. Trajetórias de ataques não podem passar por ela |
| **Modelo**               | *Dummy*         |  |

---

## Outros

| Termo          | Inglês    | Significado |
| -------------  | --------- | ----------- |
| **Ação Total** | *All-in*  | O personagem não pode ter realizado nenhuma ação ou jogada não automática (passiva) neste Ciclo para realizar uma Ação Total; feito isso, ele só terá um turno no próximo *Ciclo* |
| **Substituir** | *Replace* | Um elemento de jogo é substituído por outro determinado, herdando o estado do original<br><br>**Quando uma carta**: Ela é substituída por outra colocada no mesmo espaço, a nova carta recebe todos os contadores e anexos da carta original, e a carta original é enterrada<br><br>Colocar uma carta em um espaço ocupado sem uma mecânica de substituição, como ao adquirir uma {{ class }}, não é substituir: a carta anterior é descartada para o {{ tradingPost }}, levando consigo seus anexos e contadores<br><br>**Quando uma peça**: Ela é substituída por outra, a nova peça mantém a {{ hp }}, {{ ap }}, Marcadores, ordem do turno e posição no tabuleiro da peça original, a peça original é removida do jogo |
| **Ciclo**      | *Stint*   | O período entre uma Fase de Recomposição e outra |
| **Dono**        | *Owner*      | O personagem, geralmente um Herói, a quem uma carta ou um monte de cartas pertence |
| **Controlador** | *Controller* | O jogador que controla um Herói e, por consequência, as cartas e montes de cartas desse Herói. Um Herói sem jogador é controlado pelo Mestre de Jogo |

---

Teammate vs Team Member (Parceiro vs Membro do Time)
Teammate se refere aos demais membros do seu time que não são você, enquanto Team Member se refere a qualquer membro do time, incluindo você mesmo.

---
