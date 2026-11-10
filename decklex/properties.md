---
label: Propriedades
icon: list-unordered
order: 95
---

# Propriedades

Uma propriedade é um valor do jogo que um efeito pode modificar. A função declara a propriedade com `{ "Modifier": "<nome>" }` e altera a variável de mesmo nome, como `$hero_level`. Veja [Função do efeito](function.md) e [Variáveis](variables.md).

Toda propriedade é calculada para um herói de cada vez. O limite é aplicado ao valor final, depois de todos os efeitos.

---

## Herói

| Nome                | O que modifica                 | Bônus que formam `$base`                                                                 | Limite              | {.compact}
| ---                 | ---                            | ---                                                                                      | ---                 |
| `hero_level`        | O nível do herói               | O nível de cada carta da {{ sheet }}: {{ house }} e {{ class }}                           | De **1** a **10**   |
| `hero_endurance`    | {{ endurance }}                | O bônus de {{ endurance }} de cada carta revelada que conta na sua zona (abaixo)          | No mínimo **1**     |
| `hero_strength`     | {{ strength }}                 | O mesmo, com o bônus de {{ strength }}                                                    | No mínimo **1**     |
| `hero_agility`      | {{ agility }}                  | O mesmo, com o bônus de {{ agility }}                                                     | No mínimo **1**     |
| `hero_perception`   | {{ perception }}               | O mesmo, com o bônus de {{ perception }}                                                  | No mínimo **1**     |
| `hero_intelligence` | {{ intelligence }}             | O mesmo, com o bônus de {{ intelligence }}                                                | No mínimo **1**     |
| `hero_charisma`     | {{ charisma }}                 | O mesmo, com o bônus de {{ charisma }}                                                    | No mínimo **1**     |
| `hero_spiritual`    | {{ spiritual }}                | O mesmo, com o bônus de {{ spiritual }}                                                   | No mínimo **1**     |
| `hero_health`       | A {{ hp }} máxima              | **10** vezes cada parte de `hero_endurance`, efeitos incluídos                            | No mínimo **10**    |
| `hero_max_action_points` | O máximo de pontos de {{ ap }} | Cada parte de `hero_agility` e de `hero_level`, efeitos incluídos             | No mínimo **3**     |
| `hero_restored_action_points` | Os pontos de {{ ap }} recebidos na {{ resetPhase }} | Cada parte de `hero_agility`, efeitos incluídos                 | De **3** a **25**   |
| `hero_<conhecimento>` | O nível do herói num {{ knowledge }} | **+1** para cada vez que uma {{ class }} revelada na {{ sheet }} lista o conhecimento | No mínimo **0**     |

### Bônus de atributo por zona

| Zona        | Cartas que contam                             | {.compact}
| ---         | ---                                           |
| {{ sheet }} | {{ house }} e {{ class }}                     |
| {{ equip }} | {{ item }}                                    |
| {{ mem }}   | {{ skill }}                                   |
| {{ inv }}   | {{ item }}, {{ skill }} e {{ event }}         |

### Conhecimentos

| Nome                  | Conhecimento        | {.compact}
| ---                   | ---                 |
| `hero_faith`          | {{ faith }}         |
| `hero_cooperation`    | {{ cooperation }}   |
| `hero_practice`       | {{ practice }}      |
| `hero_defense`        | {{ defense }}       |
| `hero_athletics`      | {{ athletics }}     |
| `hero_instruction`    | {{ instruction }}   |
| `hero_arcane`         | {{ arcane }}        |
| `hero_elemental`      | {{ elemental }}     |
| `hero_cunning`        | {{ cunning }}       |
| `hero_art`            | {{ art }}           |
| `hero_transmutation`  | {{ transmutation }} |
| `hero_dimensional`    | {{ dimensional }}   |
| `hero_vital`          | {{ vital }}         |
| `hero_mental`         | {{ mental }}        |

!!!
`hero_defense` é o conhecimento {{ defense }}, não um atributo de defesa.
!!!
