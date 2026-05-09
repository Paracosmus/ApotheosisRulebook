---
label: Marcador
icon: bookmark
order: 65
---

# Marcador

{{ briefing `Marker` `É uma mecânica que representa um estado ou condição de um personagem. Eles são usados para indicar que um personagem está em uma situação específica, como estar ferido, amaldiçoado, furtivo, encantado, feliz, envenenado, doente, entre outros` }}

O marcador é um nome único aplicado ao personagem, tendo ou não uma peça no tabuleiro. Efeitos que exploram este marcador devem ser aplicados àquele personagem, sendo que o marcador não faz nada por si só.

O nome do marcador é a sua única característica, ele é utilizado para identificar o marcador e suas interações com as cartas, sendo que o nome de todo marcador começa com o identificador .

!!!secondary Exemplo de Nomes de Marcadores
**FERIDO**, **AMALDIÇOADO**, **FURTIVO**, **ENCANTADO**, **FELIZ**, **ENVENENADO**, **DOENTE**, etc.
!!!

---

## Receber um Marcador

Marcadores podem ser recebidos por meio de efeitos de cartas, ou por efeitos de campanha, ou por situações narrativas criadas sobre demanda pelo mestre de jogo.

Os marcadores são de caráter permanente. Uma vez recebido um marcador, ele permanece no personagem até que seja removido por um efeito.

Cada personagem pode ter infinitos marcadores, mas apenas um marcador de cada nome. Se um efeito resultar no personagem possuir marcadores duplicados, ignore a adição do marcador em excesso.

---

## Remover um Marcador

Marcadores podem ser removidos por meio de efeitos de cartas, ou por efeitos de campanha, ou por situações narrativas criadas sobre demanda pelo mestre de jogo.

Para remover um marcador, o efeito deve especificar o nome do marcador a ser removido. Se o personagem não possuir o marcador especificado, o efeito pode ser aplicado, apenas ignore a parte de remoção.

---

## Usar um Marcador

Marcadores podem ser usados por meio de efeitos, o marcador não tem um efeito por si só. Efeitos de carta e campanha exploram o marcador para criar condições e situações específicas para o personagem, que podem ser boas ou ruins.

!!!secondary Exemplo 1 - Bom
  Uma carta com os seguintes efeitos:

  > {{ activate }} O alvo recebe **ABENÇOADO**.

  > {{ permanent }} Personagens com **ABENÇOADO** recebem {{ p'+3' }} de **testes**.
!!!

!!!secondary Exemplo 2 - Ruim
  Uma carta com os seguintes efeitos:

  > {{ activate }} Se esta carta causar {{ dmg }}, o alvo recebe **ENVENENADO**.

  > {{ auto }} {{ resetPhase }} Personagens com **ENVENENADO** perdem {{ n'10' }} de {{ hp }}.
!!!

Quando a carta ou efeito que explora o marcador é removida, o marcador permanece no personagem, no entanto o marcador não terá mais consequências até que outra carta ou efeito o explore novamente.

Observe que qualquer carta pode explorar um marcador em seus efeitos, mesmo que o marcador em questão tenha sido adicionado ao personagem por outros meios ou cartas.

---

## Marcadores Narrativos

Marcadores podem ser criados sobre demanda pelo mestre de jogo, ao seu critério, para se encaixar com eventos imprevistos em jogo.

É comum que durante a narrativa, os personagens realizem ações inesperadas que levem a necessidade da adição de um marcador para representar uma nova condição ou estado.

!!!secondary Exemplo 1
  > O personagem pula de um telhado e acaba quebrando o pé.

  É adicionado sobre demanda o marcador **PÉ FRATURADO**, e o seguinte efeito é adicionado aos efeitos de campanha.

  > {{ permanent }} {{ req 'Se possuir **PÉ FRATURADO**' }} Restaure apenas metade dos seus pontos de {{ ap }} na {{ resetPhase }}.

  A fratura poderia ser curada ao visitar um médico e usar um gesso por um tempo, ou fazendo um teste de _Medicina_( {{ instruction }} + {{ int }}  por exemplo).
!!!

!!!secondary Exemplo 2
  > O personagem é petulante com uma poderosa bruxa e é amaldiçoado por ela.

  É adicionado sobre demanda o marcador **AMALDIÇOADO**, e o seguinte efeito é adicionado aos efeitos de campanha.

  > {{ permanent }} {{ yourTurn }} {{ req 'Se possuir **AMALDIÇOADO**' }} Você recebe {{ n'-5' }} em **testes**.

  A maldição poderia ser removida ao se desculpar com a bruxa, ou fazendo um teste de _Carisma_( {{ arcane }} + {{ cha }} ) por exemplo.
!!!

!!!secondary Exemplo 3 - Tempo de Duração
  > O personagem bebe demais em uma festa e fica embriagado.

  É adicionado sobre demanda o marcador **EMBRIAGADO**, e o seguintes efeitos são adicionados aos efeitos de campanha.

  > {{ permanent }} {{ req 'Se possuir **EMBRIAGADO**' }} {{ p'+2' }} de {{ cha }} e {{ n'-2' }} de {{ agi }} .

  > {{ permanent }} {{ req 'Quando mudar o período do dia; Se possuir **EMBRIAGADO**' }} Remova **EMBRIAGADO**.
!!!

Quando nenhum personagem possuir um marcador narrativo, o efeito pode ser removido ou desativado, a critério do Mestre de Jogo.

---
