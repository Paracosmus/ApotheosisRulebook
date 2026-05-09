---
label: Pilhas de Cartas
icon: stack
order: 30
---

# Pilhas de Cartas

{{ briefing `Card Stacks` `Pilha de cartas é o nome dado a qualquer monte de cartas utilizado no jogo.` }}

Durante uma partida, principalmente no formato padrão de campanhas, existem diversas pilhas de cartas utilizadas para alimentar a partida com novas cartas e para armazenar cartas descartadas e utilizadas. Cada uma dessas pilhas de cartas tem um nome e função específicos.

Quando uma carta está em uma pilha, por padrão, ela não possui efeito e nao é considerado ativa (em jogo), a menos que seja especificado o contrário por um efeito de carta ou mecânica de jogo. Além disso, estas cartão não possuem estado, ou seja, não são consideradas nem restauradas, nem consumidas, ou qualquer outro estado que uma carta possa ter, a menos que seja especificado o contrário por um efeito de carta ou mecânica de jogo.

---

## Baralhos

São chamados de baralhos as pilhas de cartas colocadas de face para baixo (_ocultas_) e disponíveis para os jogadores conforme as regras do jogo. Cada baralho possui um conjunto de cartas que podem ser utilizadas durante a partida, e que são embaralhadas e dispostas de forma aleatória. Diferente da pilha de descarte, a ordem das cartas em um baralho é importante, e as cartas devem ser mantidas na ordem em que foram embaralhadas e dispostas, a menos que um efeito ou mecânica de jogo permita ou exija que as cartas sejam reordenadas.

O conteúdo de um baralho é definido pela campanha ou formato de jogo, estando vazios por padrão. Sendo que uma composição inicial de cartas pode ser definida, bem como novas cartas podem ser adicionadas da caixa aos baralhos conforme a campanha progride, certos marcos e tarefas são concluídos ou conforme outras mecânicas estabelecidas pela campanha ou formato são executadas.

!!!
Em formatos competitivos, é comum que os jogadores montem seus próprios baralhos, escolhendo as cartas que irão compor seus baralhos a partir de um pool de cartas pré-definido, e seguindo regras específicas para a construção do baralho. Nestes casos, o formato de jogo vai especificar claramente as regras de construção dos baralhos, bem como as regras de interação com eles.
!!!

### Baralhos de Campanha

No formato padrão de campanhas, existem sete baralhos de campanha, um para cartas de cada naipe. Este baralhos são a fonte principal de novas cartas para os jogadores, e são utilizados para expandir o pool de cartas conforme a campanha progride.

Novas cartas podem ser adicionadas a estes baralhos pela campanha, e estas cartas são enviadas para os personagens ou para a pilha de descarte seja pela campanha, mecânica de jogo ou efeito de carta.

{.striped}
Baralho         | Naipe
--------------- |------
{{ factors }}   | Para cartas de {{ house }}
{{ tavern }}    | Para cartas de {{ class }}
{{ wound }}     | Para cartas de {{ entity }}
{{ market }}    | Para cartas de {{ item }}
{{ academy }}   | Para cartas de {{ skill }}
{{ bestiary }}  | Para cartas de {{ companion }}
{{ sanctuary }} | Para cartas de {{ event }}

#### Baralho Vazio

Quando um baralho ficar sem cartas e por algum meio for necessário comprar ou descartar uma carta deste baralho, ele deve ser reabastecido a partir de sua pilha de descarte

O Mestre deve embaralhar 100 cartas daquele naipe na pilha de descarte, ou a quantidade que estiver disponível, e colocá-las de face para baixo para formar um novo baralho.

Se não houver nenhuma carta elegível na pilha de descarte, o baralho é considerado vazio e não pode mais ser utilizado até que cartas sejam adicionadas ao baralho por outros meios, ou no futuro, quando houverem cartas elegíveis na pilha e destacar e o baralho tiver que ser reabastecido.

---

## Pilha de Descarte

A pilha de descarte é a zona central para onde as cartas são enviadas quando são descartadas no formato padrão, ou seja, quando deixam de estar ativas ou na mão de um personagem. Quando o comando "descartar" é utilizado, as cartas são enviadas para a pilha de descarte.

Esta pilha é de visibilidade pública, e as cartas nela ficam de face para cima, portanto, reveladas para todos os jogadores. As cartas da pilha não são de controle de nenhum jogador, nem mesmo do Mestre, e podem ser interagidas por qualquer jogador conforme as regras do jogo.

A ordem das cartas na pilha de descarte não é importante, e elas podem ser reordenadas e organizadas livremente pelos jogadores. Já que efeitos e mecânicas de jogo que interagem com a pilha de descarte não dependem da ordem das cartas, mas sim do conteúdo da pilha.

!!!
Em alguns formatos de jogo, principalmente em formatos onde cada jogador monta seu próprio baralho individualmente, cada jogador ou personagem pode ter sua própria pilha de descarte, e esta pilha pode ser considerado de controle do jogador ou personagem. Nestes casos, o formato de jogo vai especificar claramente as regras de interação com estas pilhas de descarte.
!!!

### Trocar Cartas

Um personagem pode realizar uma Ação Total para trocar [cartas de recurso](/cards/index.md) livremente com a pilha de descarte da campanha.

Ele deve selecionar as cartas que deseja obter da pilha de descarte e então selecionar cartas que possui cuja soma dos valores seja igual ou superior à soma dados valores das cartas que deseja obter. As cartas trocadas são descartadas para suas respectivas pilhas de descarte, e as cartas obtidas são colocadas no {{ inv }} do Herói ou anexos do {{ companion }}.

!!!
Observe que cada naipe de Recurso tem um tipo de valor, e portanto não pode ser trocada por cartas de outro tipo. Por exemplo, uma carta de {{ item }} cujo valor é medido pelo seu {{ price }}, não pode ser trocada por uma carta de {{ skill }}, cujo valor é medido em {{ xp }}.

Portanto, se uma troca envolver cartas de múltiplos naipes de recurso, cada tipo de valor deve ser avaliado e quitado individualmente.
!!!

#### Restrição de Local

Para trocar cartas de recurso com uma pilha de descarte ou obter cartas de ficha pelas suas respectivas mecânicas (<a class="class" href="/cards/class.md#progredir">Progressão</a>, <a class="entity" href="/cards/entity.md#incorporar">Incorporação</a>), o personagem deve estar em um local que permita tal ação.

Os locais no jogo são definidos pela campanha ou formato de jogo, e cada local tem um nível de acesso individual para cada baralho, que vai de **0** a **3**. O nível de acesso de um local define o nível máximo que as cartas obtidas podem ter.

O nível de casso do local não limita o acesso pelo efeito de cartas. Os efeitos podem ou não estabelecerem seus próprios filtros.

#### Restrição de Batalha

Indiferente do nível de acesso do local em que a batalha estiver acontecendo, o nível de acesso de todas as pilhas de descarte durante uma batalha é sempre 0, impossibilitando a troca de cartas.

Alguns efeitos de cartas, como cartas de {{ event }} no {{ scenario }}, entre outras, podem modificar o nível de acesso de um local, isso inclui durante uma batalha, permitindo dessa forma a troca de cartas em batalha.

---

## Buscar Cartas

Alguns efeitos de cartas e mecânicas de jogo permitem que os jogadores busquem cartas em um pilhas de cartas, e as obtenham, descartem ou realizem outras tarefas.

Este processo de ver uma pilha a procura de uma carta, ou filtrando cartas por critérios específicos, é conhecido como "busca".

Quando uma busca é realizada em um baralho com cartas ocultas, o jogador precisa olhar as cartas do baralho para encontrar a carta que deseja obter. Após localizar e/ou selecionar a carta desejada, ele deve embaralhar o baralho novamente para ocultar as cartas de forma que ele não tenha mais conhecimento sobre a posição das cartas.

---
