---
label: Baralhos
icon: stack
order: 5
---

# Baralhos

São montes de cartas colocadas de face para baixo (_ocultas_) e disponíveis para todos os jogadores conforme as regras do jogo. Cada baralho possui um conjunto de cartas que podem ser utilizadas durante a partida, e que são embaralhadas e dispostas de forma aleatória.

O conteúdo de um baralho é definido pela campanha ou formato de jogo, estando vazios por padrão. Sendo que uma composição inicial de cartas pode ser definida, bem como novas cartas podem ser adicionadas da caixa aos baralhos conforme a campanha progride, certos marcos e tarefas são concluídos ou conforme outras mecânicas estabelecidas pela campanha ou formato.

| {.compact}
|---|---
{{ factors }}   | Composto por cartas de {{ house }}
{{ tavern }}    | Composto por cartas de {{ class }}
{{ wound }}     | Composto por cartas de {{ entity }}
{{ market }}    | Composto por cartas de {{ item }}
{{ academy }}   | Composto por cartas de {{ skill }}
{{ bestiary }}  | Composto por cartas de {{ companion }}
{{ sanctuary }} | Composto por cartas de {{ event }}

### Usar um Baralho

As cartas desses baralhos se tornam disponíveis para os jogadores conforme algumas mecânicas de jogo explicadas em suas respectivas sessões neste manual, ou mesmo efeitos de cartas.

### Fim do Baralho

Quando um baralho ficar sem cartas, a metade inferior da sua respectiva [pilha de descarte](#pilhas-de-descarte) é embaralhada e disposta novamente como o baralho.

Se houver uma ou menos cartas na pilha de descarte, o baralho é considerado vazio e não pode mais ser utilizado até que cartas sejam adicionadas ao baralho por outros meios, mesmo que novas cartas sejam enviadas para a pilha de descarte.

---

## Pilhas de Descarte

Cada um dos baralhos anteriormente mencionados possuem também sua respectiva pilhas de descarte, que são compostas por cartas que foram descartadas durante a partida na ordem em que foram descartadas, portanto, uma carta descartada sempre vai para o topo da pilha de descarte de seu naipe.

As pilhas de descartes são mantidas com as suas cartas de face para cima (_reveladas_), e são visíveis para todos os jogadores, que estão livres para pegá-las e olhar seus conteúdos a qualquer momento.

> Quando um texto se referir a um dos baralhos pelo nome, ele também especificará se refere à pilha de descarte ou ao baralho em si.

### Trocar Cartas

No caso dos baralhos de [cartas de Recurso](/cards/index.md), um personagens pode sacrificar o seu turno para trocar cartas livremente com uma pilha de descarte selecionada.

Ele deve selecionar as cartas que deseja obter da pilha de descarte e então selecionar cartas que possui cuja soma dos valores seja igual ou superior à soma dados valores das cartas que deseja obter. As cartas trocadas são descartadas para suas respectivas pilhas de descarte, e as cartas obtidas são colocadas no {{ inv }} do personagem.

!!!
Observe que cada carta de Recurso tem um tipo de valor, e portanto não pode ser trocada por cartas de outro tipo. Por exemplo, uma carta de {{ item }} cujo valor é medido pelo seu {{ price }}, não pode ser trocada por uma carta de {{ skill }}, cujo valor é medido em {{ xp }}.
!!!

### Restrição de Local

Para trocar livremente cartas com uma pilha de descarte, o personagem deve estar em um local que permita tal ação.

Os locais no jogo são definidos pela campanha ou formato de jogo, e tem um nível de acesso individual para cada baralho, que vai de 0 a 3. O nível de acesso de um local define o nível máximo que as cartas obtidas podem ter.

!!!
Note que, a limitação de nível de acesso de um local restringe apenas a troca de cartas entre o personagem e a pilha de descarte por esta mecânica de troca livre. Quando efeitos de cartas ou outras mecânicas de jogo requererem interação com cartas das pilhas de descartes, essas limitações devem ser ignoradas.
!!!

### Restrição de Batalha

Indiferente do nível de acesso do local em que a batalha estiver acontecendo, o nível de acesso de todas as pilhas de descarte durante uma batalha é sempre 0, impossibilitando a troca de cartas.

> Alguns efeitos de cartas, como cartas de {{ event }} no {{ scenario }}, entre outras, podem modificar o nível de acesso de um local, isso inclui durante uma batalha.

---

## Outros Baralhos

Alguns efeitos de cartas, campanhas e formatos de jogo podem adicionar outros baralhos, geralmente não tendo uma pilha de descarte associada, e utilizando as pilhas de descarte dos naipes.

Quando um texto se referir a um baralho, sem específicá-lo pelo nome, ele se refere a qualquer baralho, inclusive estes, exceto pilhas de descarte.

### Arcofluxo

Estes baralhos geralmente são criados por cartas de {{ event }} com a propriedade _Lagvig_, para mudar o formato da partida. São compostos por todas as cartas de recurso do personagem, que são embaralhadas e dispostas.

---
