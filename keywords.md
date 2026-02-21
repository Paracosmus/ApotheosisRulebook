---
label: Palavras-Chave
layout: page
---

# Palavras-Chave

Este livro e as cartas do jogo, utilizam em seus textos, palavras que possuem significados específicos no jogo. Abaixo estão listados estes termos e seus significados.

---

## Cartas

|
---   | ---
| **Consumir**   | *Exhaust*     | Girar a carta para que ela fique na horizontal, em relação à {{ table }} do Herói |
| **Recuperar**  | *Recover*     | Girar a carta para que ela fique na vertical, em relação à {{ table }} do Herói |
| **Descartar**  | *Discard*     | Colocar uma carta na pilha de descarte |
| **Enterrar**   | *Bury*        | Colocar uma carta no fundo do baralho específico do naipe |
| **Banir**      | *Banish*      | Remover uma carta do jogo |
| **Obter**      | *Get*         | Adicionar uma carta da pilha de descarte ao {{ inv }} |
| **Baixar**     | *Place*       | Adicionar uma carta à {{ table }} |
| **Puxar**      | *Draw*        | Pegar a carta do topo do baralho especificado e adicionar ao {{ inv }}, sem mostrá-la |
| **Revelar**    | *Reveal*      | Mostrar uma carta que está oculta, geralmente virando-a de face para cima, ou mostrando-a para todos os jogadores |
| **Ocultar**    | *Conceal*     | Esconder uma carta que está revelada, geralmente virando-a de face para baixo |
| **Buscar**     | *Search*      | Escolher uma carta na pilha ou baralho especificado, geralmente com limitações, mostrá-la e adicioná-la ao {{ inv }} |
| **Mesa**       | *Table*       | Local da área do jogo onde um Herói coloca suas cartas |
| **Ficha**      | *Sheet*       | Zona da {{ table }} do Herói onde estão suas cartas de ficha |
| **Zona Extra** | *Extra Slots* | Zona da {{ sheet }} do Herói onde algumas mecânicas de jogo e efeitos de cartas podem colocar cartas de ficha extras |
| **Inventário** | *Inventory*   | O conjunto de cartas na mão do jogador |

---

## Tabuleiro

|
---   | ---
| **Peça**                 | *Piece*         | Peão que representa um personagem ou objeto no tabuleiro de batalha |
| **Mover**                | *Move*          | Colocar uma peça em uma outra casa do tabuleiro |
| **Distância**            | *Distance*      | Alcance da ação ou movimento |
| **Trajeto / Trajetória** | *Trajectory*    | Conjunto de casas do tabuleiro por onde passa a linha reta entre o personagem executando a ação e o alvo de ação |
| **Direção**              | *Direction*     | Vetor de direção de uma ação que parte de uma casa do tabuleiro até outra casa. Sendo uma linha reta com comprimento infinito para ambos os lados e um sentido de direção |
| **Adjacente**            | *Adjacent Tile* | Aquilo que está em uma casa do tabuleiro, ou é uma casa do tabuleiro, que está ao lado de outra casa do tabuleiro. Não incluindo casas diagonais |
| **Casa Bloqueada**       | *Blocked Tile*  | Nenhuma peça pode ser colocado nesta casa do tabuleiro, trajetórias de ataques DIRETOS não podem passar por esta casa. Geralmente por já estar ocupada por uma peça |
| **Casa Ocupada**         | *Occupied Tile* | Existe uma peça nesta casa do tabuleiro |
| **Casa Vazia**           | *Empty Tile*    | Qualquer casa do tabuleiro que não tenha uma peça nela |
| **Casa Desabilitada**    | *Disabled Tile* | Nenhuma peça pode ser colocada ou passar por esta casa do tabuleiro, para todos os fins, ela não existe. Trajetórias de ataques não podem passar por elas |

---

## Outros

|
---   | ---
| **Ação Total** | *All-in*  | O personagem não pode ter realizado nenhuma ação ou jogada não automática (passiva) neste Ciclo para realizar uma Ação Total; feito isto, ele só terá um turno no próximo *Ciclo* |
| **Substituir** | *Replace* | Um elemento de jogo é substituído por outro determinado, herdando o estado do original<br><br>**Quando uma carta**: Ela é substituída por outra, a nova carta recebe todos os contadores e anexos da carta original, e a carta original é enviada para o mesmo local em que estava a nova carta, se possível, caso contrário, a carta original é descartada para a pilha de descarte<br><br>**Quando uma peça**: Ela é substituída por outra, a nova peça mantem a {{ hp }}, {{ ap }}, Marcados e posição no tabuleiro da peça original, a peça original é removida do jogo |
| **Ciclo**      | *Stint*   | O período entre uma Fase de Recomposição e outra |
