---
label: Personagem
icon: person
order: 70
---
{{ review() }}

# Personagem

{{ briefing `Character` `É toda representação de um indivíduo animado, ou seja, que pode se mover, agir e interagir com o ambiente do jogo, e que pode ser controlada por um jogador ou pelo mestre de jogo, e que possui características, habilidades e estatísticas específicas.` }}

Os personagens são representados por cartas, miniaturas ou meeples no tabuleiro, e são os principais agentes através dos quais os jogadores interagem com o mundo do jogo.

Personagem é a forma de se designar qualquer referência que represente um ser animado, englobando humanos, animais, evocações e quaisquer criaturas vivas, tendo elas peças no tabuleiro ou não.

Geralmente, o termo se refere a [Heróis](/hero/), {{ companion }} e [Modelos](/battle/piece/dummy.md), mas em situações específicas de campanha, podem também se referir a outras criaturas.

---

## Estatísticas

---

## Reviver

> É a ação de trazer um personagem de volta à vida, geralmente após a morte ou quando o personagem foi nocauteado.

Quando um personagem morrer, não é o fim definitivo, se sua peça ainda estiver no tabuleiro ele pode ser revivido por alguns efeitos de cartas, ou por ações de outros personagens. Porém, se não for revivido, o personagem está permanentemente morto.

💀 Morto
:   É o estado de um personagem quando sua {{ hp }} é menor ou igual a 0. Neste estado, o personagem não pode agir, e todos os efeitos e cartas que o personagem possui são ignoradas.

    O personagem também é removido da fila de turnos, não tendo mais forma de jogar.

🤕 Nocauteado [!badge K.O.]
:   É o estado de um personagem quando sua {{ hp }} é exatamente 0. Neste estado, para todos os efeitos, o personagem é tratado como morto. Se o personagem não for revivido, ele revive ao final da batalha em 1 de {{ hp }}.

    !!!
    Alguns efeitos de cartas e regras de campanha podem especificar que um personagem morto deve ser tratado como nocauteado, nestes casos, se a {{ hp }} do personagem for menor que 0, o personagem fica com 0 de {{ hp }}.
    !!!

💣 Perda Total [!badge overkill]
:   É o estado de um personagem quando o valor absoluto (módulo) da sua {{ hp }} negativa é maior ou igual à sua {{ hp }} máxima positiva.

    Ele é considerado em um estado perda total, e não pode ser revivido, já que os danos ao seu corpo estão de tal forma que não há mais como reverter, e o personagem é considerado morto permanentemente.

    !!!
    Alguns efeitos de cartas e situações de campanha podem especificar que um personagem morto deve ser tratado como perda total, nestes casos, altere a {{ hp }} negativa do personagem para que seja igual ao valor necessário para estar neste estado, se o valor atual já não for o suficiente.
    !!!

    !!!
    Em adicional, se o valor absoluto (módulo) da sua {{ hp }} negativa for maior ou igual à **duas vezes** sua {{ hp }} máxima positiva, a peça deste personagem foi destruída, e portanto deve ser removida do tabuleiro.
    !!!

Quando um personagem morto é revivido, ele é adicionado ao final da fila de turnos, caso não tenha tido um turno nesta rodada ainda. Jogando na ordem normal, a partir da próxima rodada.

---




São aliados humanos que podem ser recrutados pelos Heróis para ajudá-los em suas jornadas. Eles possuem habilidades e características específicas, e podem ser usados para complementar as estratégias dos Heróis. Mas tam'bem são muito usados pelo mestre de jogo para representar NPCs (personagens não-jogadores) que interagem com os jogadores durante a campanha, como comerciantes, informantes, ou personagens de apoio, inimigos em batalhas, etc..

São os animais, bestas e monstros.

São os seres sobrenaturais, entidades, espíritos, demônios, etc.. que podem ser evocados pelos Heróis para lutar ao seu lado ou realizar ações específicas.
