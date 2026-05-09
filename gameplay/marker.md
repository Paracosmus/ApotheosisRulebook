# Marcador

|||{.briefing} [!badge text="Marker" variant="ghost"]
  É uma mecânica que representa um estado ou condição de um personagem. Eles são usados para indicar que um personagem está em uma situação específica, como estar ferido, amaldiçoado, furtivo, encantado, feliz, envenenado, doente, entre outros
|||
    
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

  > [<span class="keyword-activation">Ativar</span>](/cards/effect.md) O alvo recebe **ABENÇOADO**.

  > [<span class="keyword-activation">Permanente</span>](/cards/effect.md) Personagens com **ABENÇOADO** recebem <span class="positive">+3</span> de **testes**.
!!!

!!!secondary Exemplo 2 - Ruim
  Uma carta com os seguintes efeitos:

  > [<span class="keyword-activation">Ativar</span>](/cards/effect.md) Se esta carta causar <b>DANO</b>, o alvo recebe **ENVENENADO**.

  > [<span class="keyword-activation">Auto</span>](/cards/effect.md) [<span class="keyword-timing">Fase de Recomposição</span>](/cards/effect.md) Personagens com **ENVENENADO** perdem <span class="negative">10</span> de [<span class="hp"><b>VIDA</b></span>](/hero/#vida).
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

  > [<span class="keyword-activation">Permanente</span>](/cards/effect.md) <span class="req">【</span> Se possuir **PÉ FRATURADO** <span class="req">】</span> Restaure apenas metade dos seus pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) na [<span class="keyword-timing">Fase de Recomposição</span>](/cards/effect.md).

  A fratura poderia ser curada ao visitar um médico e usar um gesso por um tempo, ou fazendo um teste de _Medicina_( [<span class="knowledge"><b>INSTRUÇÃO</b></span>](/hero/knowledge.md#instrução) + [<span class="house"><b>INT</b></span>](/hero/attributes.md)  por exemplo).
!!!

!!!secondary Exemplo 2
  > O personagem é petulante com uma poderosa bruxa e é amaldiçoado por ela.

  É adicionado sobre demanda o marcador **AMALDIÇOADO**, e o seguinte efeito é adicionado aos efeitos de campanha.

  > [<span class="keyword-activation">Permanente</span>](/cards/effect.md) [<span class="keyword-limit">Apenas no seu Turno</span>](/cards/effect.md) <span class="req">【</span> Se possuir **AMALDIÇOADO** <span class="req">】</span> Você recebe <span class="negative">-5</span> em **testes**.

  A maldição poderia ser removida ao se desculpar com a bruxa, ou fazendo um teste de _Carisma_( [<span class="knowledge"><b>ARCANO</b></span>](/hero/knowledge.md#arcano) + [<span class="house"><b>CAR</b></span>](/hero/attributes.md) ) por exemplo.
!!!

!!!secondary Exemplo 3 - Tempo de Duração
  > O personagem bebe demais em uma festa e fica embriagado.

  É adicionado sobre demanda o marcador **EMBRIAGADO**, e o seguintes efeitos são adicionados aos efeitos de campanha.

  > [<span class="keyword-activation">Permanente</span>](/cards/effect.md) <span class="req">【</span> Se possuir **EMBRIAGADO** <span class="req">】</span> <span class="positive">+2</span> de [<span class="house"><b>CAR</b></span>](/hero/attributes.md) e <span class="negative">-2</span> de [<span class="house"><b>AGI</b></span>](/hero/attributes.md) .

  > [<span class="keyword-activation">Permanente</span>](/cards/effect.md) <span class="req">【</span> Quando mudar o período do dia; Se possuir **EMBRIAGADO** <span class="req">】</span> Remova **EMBRIAGADO**.
!!!

Quando nenhum personagem possuir um marcador narrativo, o efeito pode ser removido ou desativado, a critério do Mestre de Jogo.

---
