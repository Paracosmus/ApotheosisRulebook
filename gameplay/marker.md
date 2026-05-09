---
label: Marcadores
icon: bookmark
order: 65
---
{{ review() }}

# Marcadores

{{ briefing `Marker` `É uma mecânica que representa um estado ou condição de um personagem. Eles são usados para indicar que um personagem está em uma situação específica, como estar ferido, amaldiçoado, furtivo, encantado, feliz, envenenado, doente, entre outros` }}

O marcador é um nome único aplicado ao personagem, tendo ou não uma peça no tabuleiro. Efeitos que exploram este marcador devem ser aplicados àquele personagem, sendo que o marcador não faz nada por si só.

O nome do marcador é a sua única característica, ele é utilizado para identificar o marcador e suas interações com as cartas, sendo que o nome de todo marcador começa com o identificador .

!!!secondary Exemplo de Nomes de Marcadores
**FERIDO**, **AMALDIÇOADO**, **FURTIVO**, **ENCANTADO**, **FELIZ**, **ENVENENADO**, **DOENTE**, etc.
!!!

Os marcadores são de caráter permanente. Uma vez recebido um marcador, ele permanece no personagem até que seja removido por um efeito.

Cada personagem pode ter infinitos marcadores, mas apenas um marcador de cada nome. Se um efeito resultar no personagem possuir marcadores duplicados, ignore a adição do marcador em excesso.

---

## Receber um Marcador

---

## Remover um Marcador

---

## Marcadores Narrativos

Marcadores podem ser criados sobre demanda pelo mestre de jogo, ao seu critério, para se encaixar com eventos imprevistos em jogo.

É comum que durante a narrativa, os personagens realizem ações inesperadas que levem a necessidade da adição de um marcador para representar uma nova condição ou estado.

!!!secondary Exemplo 1
  > O personagem pula de um telhado e acaba quebrando o pé.

  É adicionado sobre demanda o marcador **PÉ FRATURADO**, e o seguinte efeito é adicionado aos efeitos de campanha.

  > {{ permanent }} {{ req 'Se possuir **PÉ FRATURADO**' }} Restaure apenas metade dos seus pontos de {{ ap }} na {{ resetPhase }}.
!!!

!!!secondary Exemplo 2
  > O personagem é petulante com uma poderosa bruxa e é amaldiçoado por ela.

  É adicionado sobre demanda o marcador **AMALDIÇOADO**, e o seguinte efeito é adicionado aos efeitos de campanha.

  > {{ permanent }} {{ yourTurn }} {{ req 'Se possuir **AMALDIÇOADO**' }} Você recebe {{ n'-5' }} em **testes**.
!!!

!!!secondary Exemplo 3 - Tempo de Duração
  > O personagem bebe demais em uma festa e fica embriagado.

  É adicionado sobre demanda o marcador **EMBRIAGADO**, e o seguintes efeitos são adicionados aos efeitos de campanha.

  > {{ permanent }} {{ req 'Se possuir **EMBRIAGADO**' }} {{ p'+2' }} de {{ cha }} e {{ n'-2' }} de {{ agi }} .

  > {{ permanent }} {{ req 'Quando mudar o período do dia; Se possuir **EMBRIAGADO**' }} Remova **EMBRIAGADO**.
!!!

Quando nenhum personagem possuir um marcador narrativo, o efeito pode ser removido ou desativado, a critério do Mestre de Jogo.

---
