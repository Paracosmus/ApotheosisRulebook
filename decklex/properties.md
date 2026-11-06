# Propriedades

Uma propriedade é um valor do jogo que um efeito pode modificar. A função declara a propriedade com `{ "Modifier": "<nome>" }` e altera a variável de mesmo nome, como `$hero_level`. Veja [Função do efeito](function.md) e [Variáveis](variables.md).

Toda propriedade é calculada para um herói de cada vez. O limite é aplicado ao valor final, depois de todos os efeitos.

---

## Herói

| Nome                | O que modifica                 | Bônus que formam `$base`                                                                 | Limite              | {.compact}
| ---                 | ---                            | ---                                                                                      | ---                 |
| `hero_level`        | O nível do herói               | O nível de cada carta da [<span class="main"><b>FICHA</b></span>](/hero/table/sheet.md): [<span class="house"><b>CASA</b></span>](/cards/house.md) e [<span class="class"><b>CLASSE</b></span>](/cards/class.md)                           | De **1** a **10**   |
| `hero_endurance`    | [<span class="house"><b>CONSTITUIÇÃO</b>](/gameplay/attributes.md)                | O bônus de [<span class="house"><b>CONSTITUIÇÃO</b>](/gameplay/attributes.md) de cada carta revelada que conta na sua zona (abaixo)          | No mínimo **1**     |
| `hero_strength`     | [<span class="house"><b>FORÇA</b>](/gameplay/attributes.md)                 | O mesmo, com o bônus de [<span class="house"><b>FORÇA</b>](/gameplay/attributes.md)                                                    | No mínimo **1**     |
| `hero_agility`      | [<span class="house"><b>AGILIDADE</b>](/gameplay/attributes.md)                  | O mesmo, com o bônus de [<span class="house"><b>AGILIDADE</b>](/gameplay/attributes.md)                                                     | No mínimo **1**     |
| `hero_perception`   | [<span class="house"><b>PERCEPÇÃO</b>](/gameplay/attributes.md)               | O mesmo, com o bônus de [<span class="house"><b>PERCEPÇÃO</b>](/gameplay/attributes.md)                                                  | No mínimo **1**     |
| `hero_intelligence` | [<span class="house"><b>INTELIGÊNCIA</b>](/gameplay/attributes.md)             | O mesmo, com o bônus de [<span class="house"><b>INTELIGÊNCIA</b>](/gameplay/attributes.md)                                                | No mínimo **1**     |
| `hero_charisma`     | [<span class="house"><b>CARISMA</b>](/gameplay/attributes.md)                 | O mesmo, com o bônus de [<span class="house"><b>CARISMA</b>](/gameplay/attributes.md)                                                    | No mínimo **1**     |
| `hero_spiritual`    | [<span class="house"><b>ESPIRITUAL</b>](/gameplay/attributes.md)                | O mesmo, com o bônus de [<span class="house"><b>ESPIRITUAL</b>](/gameplay/attributes.md)                                                   | No mínimo **1**     |
| `hero_health`       | A [<span class="hp"><b>VIDA</b></span>](/hero/#vida) máxima              | **10** vezes cada parte de `hero_endurance`, efeitos incluídos                            | Nenhum              |
| `hero_<conhecimento>` | O nível do herói num [<span class="knowledge"><b>CONHECIMENTO</b></span>](/gameplay/knowledge.md) | **+1** para cada vez que uma [<span class="class"><b>CLASSE</b></span>](/cards/class.md) revelada na [<span class="main"><b>FICHA</b></span>](/hero/table/sheet.md) lista o conhecimento | No mínimo **0**     |

### Bônus de atributo por zona

| Zona        | Cartas que contam                             | {.compact}
| ---         | ---                                           |
| [<span class="main"><b>FICHA</b></span>](/hero/table/sheet.md) | [<span class="house"><b>CASA</b></span>](/cards/house.md) e [<span class="class"><b>CLASSE</b></span>](/cards/class.md)                     |
| [<span class="item"><b>EQUIPAMENTO</b></span>](/hero/table/equipment.md) | [<span class="item"><b>ITEM</b></span>](/cards/item.md)                                    |
| [<span class="skill"><b>MEMENTO</b></span>](/hero/table/memento.md)   | [<span class="skill"><b>HABILIDADE</b></span>](/cards/skills.md)                                   |
| [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md)   | [<span class="item"><b>ITEM</b></span>](/cards/item.md), [<span class="skill"><b>HABILIDADE</b></span>](/cards/skills.md) e [<span class="event"><b>EVENTO</b></span>](/cards/event.md)         |

### Conhecimentos

| Nome                  | Conhecimento        | {.compact}
| ---                   | ---                 |
| `hero_faith`          | [<span class="knowledge"><b>FÉ</b></span>](/gameplay/knowledge.md#fé)         |
| `hero_cooperation`    | [<span class="knowledge"><b>COOPERAÇÃO</b></span>](/gameplay/knowledge.md#cooperação)   |
| `hero_practice`       | [<span class="knowledge"><b>PRÁTICA</b></span>](/gameplay/knowledge.md#prática)      |
| `hero_defense`        | [<span class="knowledge"><b>DEFESA</b></span>](/gameplay/knowledge.md#defesa)       |
| `hero_athletics`      | [<span class="knowledge"><b>ATLETISMO</b></span>](/gameplay/knowledge.md#atletismo)     |
| `hero_instruction`    | [<span class="knowledge"><b>INSTRUÇÃO</b></span>](/gameplay/knowledge.md#instrução)   |
| `hero_arcane`         | [<span class="knowledge"><b>ARCANO</b></span>](/gameplay/knowledge.md#arcano)        |
| `hero_elemental`      | [<span class="knowledge"><b>ELEMENTAL</b></span>](/gameplay/knowledge.md#elemental)     |
| `hero_cunning`        | [<span class="knowledge"><b>ASTÚCIA</b></span>](/gameplay/knowledge.md#astúcia)       |
| `hero_art`            | [<span class="knowledge"><b>ARTE</b></span>](/gameplay/knowledge.md#arte)           |
| `hero_transmutation`  | [<span class="knowledge"><b>TRANSMUTAÇÃO</b></span>](/gameplay/knowledge.md#transmutação) |
| `hero_dimensional`    | [<span class="knowledge"><b>DIMENSIONAL</b></span>](/gameplay/knowledge.md#dimensional)   |
| `hero_vital`          | [<span class="knowledge"><b>VITAL</b></span>](/gameplay/knowledge.md#vital)         |
| `hero_mental`         | [<span class="knowledge"><b>MENTAL</b></span>](/gameplay/knowledge.md#mental)        |

!!!
`hero_defense` é o conhecimento [<span class="knowledge"><b>DEFESA</b></span>](/gameplay/knowledge.md#defesa), não um atributo de defesa.
!!!
