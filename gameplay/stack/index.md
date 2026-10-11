---
label: Monte de Cartas
icon: stack
order: 30
---

# Monte de Cartas

{{ briefing `Card Stacks` `Monte de cartas é o nome dado a qualquer conjunto de cartas empilhadas utilizado no jogo.` }}

Durante uma partida, principalmente no formato padrão de campanhas, existem diversos montes de cartas utilizados para alimentar a partida com novas cartas e para armazenar cartas descartadas e utilizadas. Cada um desses montes tem um nome e função específicos.

Um monte de face para cima é chamado de [pilha](#pilhas), e um monte de face para baixo é chamado de [baralho](#baralhos).

Todo monte é definido por três configurações:

{.striped}
Configuração | Em inglês | O que define
--- | --- | ---
**Visibilidade** | *Visibility* | Se as cartas ficam de face para cima ou para baixo, e quem pode vê-las.
**Uso** | *Usable* | Quando os efeitos das cartas do monte são considerados.
**Afetados** | *Affects* | Quais personagens são afetados pelos efeitos das cartas do monte.

---

## Dono

Um monte pode ter um dono. O controlador de um monte é o controlador do seu dono.

A visibilidade de um monte se refere ao seu controlador, enquanto os efeitos das cartas se referem ao seu dono.

- Apenas o dono de um monte pode ativar e usar as cartas dele.
- Um monte sem dono pode ter suas cartas ativadas e usadas por qualquer um.

---

## Visibilidade

A visibilidade define a orientação das cartas do monte e quem pode vê-las. Uma carta adicionada a um monte assume a orientação dele.

{.striped}
Visibilidade | Em inglês | Tipo de monte | Quem vê as cartas
--- | --- | --- | ---
**Face para cima** | *Face Up* | Pilha | Todos os jogadores.
**Face para baixo** | *Face Down* | Baralho | Ninguém.
**Face para baixo, só o controlador** | *Face Down Owner* | Baralho | Apenas o controlador do monte.

### Pilhas

São chamados de pilhas os montes de cartas colocados de face para cima (_reveladas_), e portanto visíveis para todos os jogadores, como o [entreposto](trading-post.md).

### Baralhos

São chamados de baralhos os montes de cartas colocados de face para baixo (_ocultas_) e disponíveis para os jogadores conforme as regras do jogo. Cada baralho possui um conjunto de cartas que podem ser utilizadas durante a partida, e que são embaralhadas e dispostas de forma aleatória. Diferente do entreposto, a ordem das cartas em um baralho é importante, e as cartas devem ser mantidas na ordem em que foram embaralhadas e dispostas, a menos que um efeito ou mecânica de jogo permita ou exija que as cartas sejam reordenadas.

Por padrão, ninguém pode ver as cartas de um baralho. Alguns baralhos, porém, podem ser vistos pelo seu controlador, e apenas por ele.

!!!
Em formatos competitivos, é comum que os jogadores montem seus próprios baralhos, escolhendo as cartas que irão compor seus baralhos a partir de um pool de cartas pré-definido, e seguindo regras específicas para a construção do baralho. Nestes casos, o formato de jogo vai especificar claramente as regras de construção dos baralhos, bem como as regras de interação com eles.
!!!

#### Baralho Vazio

Quando um baralho ficar sem cartas e por algum meio for necessário comprar ou descartar uma carta deste baralho, ele deve ser reabastecido a partir do entreposto

O Mestre deve embaralhar 100 cartas daquele naipe no entreposto, ou a quantidade que estiver disponível, e colocá-las de face para baixo para formar um novo baralho.

Se não houver nenhuma carta elegível no entreposto, o baralho é considerado vazio e não pode mais ser utilizado até que cartas sejam adicionadas ao baralho por outros meios, ou no futuro, quando houverem cartas elegíveis no entreposto e o baralho tiver que ser reabastecido.

---

## Efeitos das Cartas em um Monte

Uma carta de face para baixo em um monte **nunca** tem seus efeitos considerados, seja qual for a configuração do monte. O que vale é a orientação da própria carta, e não a orientação padrão do monte.

Para as cartas de face para cima, duas configurações do monte dizem quando os efeitos são considerados e quem é afetado por eles.

### Uso

Define quando os efeitos das cartas de face para cima do monte são considerados.

{.striped}
Uso | Em inglês | Efeitos considerados | Exemplo
--- | --- | --- | ---
**Sempre** | *Always* | Todos os efeitos das cartas de face para cima. | {{ scenario }}
**Nunca** | *Never* | Nenhum efeito, nem mesmo os das cartas de face para cima. | Cartas banidas, [Limbo](/gameplay/limbo.md)
**Com palavra-chave** | *Keyworded* | Apenas os efeitos com a palavra-chave {{ pile }} ou {{ anywhere }} das cartas de face para cima. | [Entreposto](trading-post.md)

### Afetados

Define quais personagens são afetados pelos efeitos das cartas do monte, quando eles são considerados.

{.striped}
Afetados | Em inglês | Quem é afetado
--- | --- | ---
**Todos** | *Everyone* | Todos os personagens.
**Dono** | *Owner* | Apenas o dono do monte.

Esta configuração diz quem recebe os efeitos, e não quem pode ativá-los. A ativação segue sempre a regra do [dono](#dono).

!!!
Em um monte que afeta todos, uma carta que concede +2 de {{ dmg }} concede este bônus a todos os personagens. Já uma carta com um efeito ativável neste mesmo monte só pode ser ativada pelo dono do monte.
!!!

### Estado das Cartas

As cartas em um monte não possuem estado, ou seja, não são consideradas nem restauradas, nem consumidas, ou qualquer outro estado que uma carta possa ter, a menos que seja especificado o contrário por um efeito de carta ou mecânica de jogo.

---

## Buscar Cartas

Alguns efeitos de cartas e mecânicas de jogo permitem que os jogadores busquem cartas em um monte de cartas, e as obtenham, descartem ou realizem outras tarefas.

Este processo de ver um monte a procura de uma carta, ou filtrando cartas por critérios específicos, é conhecido como "busca".

Quando uma busca é realizada em um baralho com cartas ocultas, o jogador precisa olhar as cartas do baralho para encontrar a carta que deseja obter. Após localizar e/ou selecionar a carta desejada, ele deve embaralhar o baralho novamente para ocultar as cartas de forma que ele não tenha mais conhecimento sobre a posição das cartas.

---
