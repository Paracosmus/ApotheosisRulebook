---
label: Ações de jogo
icon: zap
order: 112
---
# Ações de jogo
> As ações que um `Command` faz

Uma ação de jogo muda a partida: move uma carta, revela uma carta, move uma peça. Um efeito faz uma ação com a instrução [Command](statements.md#command).

Uma ação é um objeto JSON. O campo `type` diz qual é a ação, e os campos dela ficam ao lado dele. Um campo opcional pode ficar de fora.

```json
{ "type": "SendPlaycard", "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6", "to": "9b2e4c1a-7d3f-4e8b-a6c5-1f0d2e3b4a59" }
```

!!!
Esta página lista só as ações que um efeito pode fazer. As ações do Mestre do Jogo, como criar cartas, pilhas, times, heróis e tabuleiros, ou pôr um herói em cena, são recusadas quando vêm de um efeito.
!!!

---

## Formatos dos campos

| Formato         | Como escrever                                                                                                       | {.compact}
| ---             | ---                                                                                                                 |
| Id              | O id do objeto na partida, um texto como `"3fa85f64-5717-4562-b3fc-2c963f66afa6"`.                                  |
| Zona            | Uma pilha: `{ "Stack": "<id da pilha>" }`. Uma zona de um herói: `{ "Equipment": "<id do herói>" }`, e da mesma forma `House`, `Class1`, `Class2`, `Class3`, `Entity`, `Extra`, `Memento`, `Support` e `Inventory`. Anexada a uma carta: `{ "Attachment": "<id da carta>" }`. Guardada num objeto: `{ "Storage": "<id do objeto>" }`. |
| Posição         | `"Top"`, `"Bottom"`, `"Random"` ou `{ "Index": 2 }`, contado a partir do topo, começando em **0**.                    |
| Peça            | Um herói: `{ "Character": { "Hero": "<id>" } }`. Um companheiro: `{ "Character": { "Companion": "<id da carta>" } }`. Um dummy: `{ "Character": { "Dummy": "<id>" } }`. Um objeto: `{ "Object": "<id>" }`. |

---

## Cartas

| `type`            | Campos                         | O que faz                                                    | {.compact}
| ---               | ---                            | ---                                                          |
| `MovePlaycard`    | `id`, `to`, `position`         | Move a carta para a zona `to`, na posição `position`.         |
| `SendPlaycard`    | `id`, `to`                     | Põe a carta no topo da pilha `to`.                            |
| `DiscardPlaycard` | `id`                           | Põe a carta no topo do {{ tradingPost }}.                     |
| `BuryPlaycard`    | `id`, `to`                     | Põe a carta no fundo da pilha `to`.                           |
| `BanishPlaycard`  | `id`                           | Põe a carta no topo de {{ banished }}.                        |
| `ExilePlaycard`   | `id`                           | Põe a carta no topo do [limbo](/gameplay/limbo.md).           |
| `RevealPlaycard`  | `id`                           | Revela a carta, sem movê-la.                                  |
| `HidePlaycard`    | `id`                           | Esconde a carta, sem movê-la.                                 |
| `ConsumePlaycard` | `id`                           | Consome a carta, sem movê-la.                                 |
| `RecoverPlaycard` | `id`                           | Recupera a carta, sem movê-la.                                |
| `DrawFromStack`   | `from`, `to`                   | Move a carta do topo da pilha `from` para a zona `to`.        |

---

## Peças

| `type`              | Campos                          | O que faz                                                                    | {.compact}
| ---                 | ---                             | ---                                                                          |
| `CreatePiece`       | `source`                        | Cria a peça, fora de qualquer tabuleiro.                                     |
| `DeletePiece`       | `source`, `cards_to` (opcional) | Apaga a peça e a tira de todo tabuleiro, junto com as peças que ela criou. As cartas guardadas nela vão para a pilha `cards_to`, ou são apagadas sem ela. |
| `SpawnPiece`        | `source`, `board`, `position`   | Põe a peça no tabuleiro `board`, na casa de número `position`.               |
| `DestroyPiece`      | `source`, `board`               | Tira a peça do tabuleiro `board`. A peça continua existindo.                 |
| `MovePiece`         | `source`, `board`, `position`   | Move a peça para a casa de número `position` do tabuleiro `board`.           |
| `ChangePieceHealth` | `source`, `amount`              | Soma `amount` à {{ hp }} da peça. Um número negativo tira {{ hp }}. Um personagem nunca passa da {{ hp }} máxima. |
