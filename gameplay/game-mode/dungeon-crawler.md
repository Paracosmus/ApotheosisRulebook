---
label: Dungeon Crawler
icon: flowchart
order: 5
---

# Modo de Dungeon Crawler

{{ briefing `Dungeon Crawler` `É o modo de jogo onde os Heróis exploram um battlemap interagindo com outras peças no tabuleiro, sejam elas personagens e objetos, onde testes e interações são realizados sobre mecânicas específicas do jogo.` }}

---

## Área do time

Para um personagem ser considerado do seu time, ele precisa, além de estar registrado como membro do seu time, estar dentro da sua área do time.

> Área do time = {{ cha }}

Deste modo, observe que é possível um personagem estar na sua área do time, sem que você esteja na área dele, e vice-versa.

### Companions

{{ companion }} devem estar dentro da área do time do seu herói. Se a qualquer momento o {{ companion }} sair da área, sua peça é removida do tabuleiro e sua carta carta é enviada para o {{ inv }} do herói.

Ao enviar uma carta de {{ companion }} para o {{ support }}, a peça daquele personagem aparece no limite da área do time do seu herói, em uma casa a escolha do jogador.

---

## Alcance Ilimitado

Ações de alcance ilimitado possuem restrição de distância neste modo de jogo. Sendo assim, o alcance máximo é determinado pela {{ per }} do personagem.

---

## Mecânicas

### Interações

Interação
:   **3** de {{ ap }}

Falar
:   **2** de {{ ap }}
*   Pode ser encadeado a qualquer ação, mesmo que no turno de outro personagem.

Teste
:   **5** de {{ ap }}


### Testes

Propagar Voz
:   **4** de propagação em {{ range }}
*   *Gritar*( {{ enr }} )
*   *Vocalização Técnica*( {{ art }} + {{ enr }} )

Escutar
:   **2** de {{ per }} em {{ range }}
*   Um som precisa ter chegado até alguma casa neste {{ range }} para ser ouvido.

Peças
:   Dificuldade do teste igual à {{ hp }} da peça
*   **Cadeado**: *Destrancar*( {{ cunning }} + {{ agi }} )
*   **Porta**: *Arrombar*( {{ str }} )
*   **Parede**: *Empurrar*( {{ str }} )

---
