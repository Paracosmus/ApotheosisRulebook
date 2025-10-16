---
label: Formatos
icon: project
order: 9
---

# Formatos

Os formatos de jogo são regras que definem como a partida será jogada, e quais cartas podem ser utilizadas.

Cada formato possui suas próprias diretrizes e restrições, e podem ser utilizados para criar partidas mais equilibradas ou desafiadoras.

Segue abaixo alguns dos formatos de jogo mais comuns em APOTEOSE CARD GAME.

!!!
É comum que os formatos tenham limites para o uso de certas cartas que podem não funcionar bem ou prejudicar o jogo naquelas regras. Esse limite Inclui a soma das cópias na  **MESA**, {{ inv }} e anexos daquele personagem.
!!!

---

==- Padrão

É o formato de jogo mais comum, onde as regras são definidas pela campanha ou pelos jogadores, e não possuem restrições específicas.

!!!
Comumente, este formato é composto por uma campanha cooperativa com um narrador, estória e objetivos específicos.
!!!

===

---


==- Lagvig

> **Lagvig** – do nórdico (_"lag" lei ou regras_ + _"víg" luta ou combate_) → Combate sob a lei

É um grupo de formatos de batalha comum em batalhas competitivas, com regras específicas geralmente definidos por uma carta chamada _Arcofluxo_, onde cada jogador possui um baralho composto por cartas de recurso.

#### Limite de 3 cópias por Herói
* Cartas de raridade {{ common }}
    * Cartas de raridade {{ uncommon }}
    * Cartas de raridade {{ rare }}

#### Limite de 1 cópia por Herói
* Cartas de raridade {{ epic }}
    * Cartas de raridade {{ legendary }}

#### Proibido o uso
* Cartas da coleção ‘_Proibida_’

As batalhas lagvig são geralmente organizadas em uma liga estruturada e organizada chamada Leiker.

> **Leiker** - do nórdico (_"leikr" jogo ou competição_) → Era um termo genérico dos vikings para diferentes tipos de jogos, competições e duelos. Podia envolver atividades físicas, desafios de força, agilidade ou estratégia.

===


==- Batalha Pokémon

#### 👥 Estrutura de Times
Cada time pode ter até 3 jogadores.
Cada jogador deve ter pelo menos 1 companheiro ativo no início de cada rodada.
Cada time pode manter até 3 companheiros ativos simultaneamente no campo.
Quando 6 companheiros de um mesmo time forem derrotados, o time perde.


#### 🧬 Companheiros e Evoluções
Cada time escolhe:
6 companheiros de Nível 1 (iniciam no suporte, deitados).
Até 3 companheiros de Nível 2 (reservados para evoluções).
Até 1 companheiro de Nível 3 (também reservado para evolução).

#### 📈 Regras de Evolução
Para evoluir um companheiro o companheiro deve sacrificar seu turno e descartar:
Do Nível 1 → 2:  2 de Vontade
Do Nível 2 → 3:  3 de Vontade

#### 🎲 Mapa e Cartas no Campo
O campo é um mapa quadriculado (ex: 11x11).
Para as batalhas é criado um baralho do local composto por 30 cartas e

No início de cada rodada, 5 cartas aparecem aleatoriamente no mapa, podendo ser:
Vontade
Destino ou
Item Consumível

Ao final da rodada as cartas não coletadas voltam para o baralho do local.


#### 📦 Coleta e Anexos
Um companheiro deve ir até a célula da carta e gastar:
1 Ponto de Ação (PA) para anexá-la a si ou enviá-la ao inventário compartilhado do time.
Cartas anexadas não podem ser removidas.
Todos os anexos são coringa: não importa o tipo, apenas a quantidade necessária para ativar efeitos ou evoluções.

#### 💀 Salvação Divina
1x por rodada por companheiro, o treinador pode:
Descartar cartas de Destino do inventário cujo a soma de seus níveis, equivalentes ao nível do companheiro,
Para impedir sua morte, mantendo-o com 1 de PV.

#### 🌀 Destino e Cartas Especiais
Algumas cartas de Destino possuem efeitos ativáveis.
Se estiverem no inventário, qualquer companheiro pode ativá-las durante sua vez, sem custo.

#### 🍭 Efeitos Tolos
Cartas com efeitos tolos são permitidas.

[00:00, 04/05/2025] Raphael Arthur: Obs: o inventário é do time
[00:01, 04/05/2025] Raphael Arthur: Quando um companheiro evolui ele herda o dano tomado, então se ele tinha 3/5 PV enquanto nível 1, quando evoluir para o nível 2 ele fica com 8/10 PV

[00:11, 04/05/2025] Bruno: A parte dos anexos eu achei desnecessário. No caso elas são coringas porque seria muito difícil conseguir extamente os anexos que aquela carta precisa, mas nesse caso não seria melhor liberar logo para poder usar todos os moves sem ter anexos?
[00:12, 04/05/2025] Bruno: Porque como o foco é batalha de companheiros, ninguem vai querer companheiro que precisa de anexo de toda forma mesmo
[00:12, 04/05/2025] Raphael Arthur: é melhor mesmo

===


==- Batalha Campal

É um formato de batalha onde os jogadores se enfrentam em um campo de batalha terrestre, com regras específicas para o combate e a movimentação, na intensão de simular uma batalha em grande escala entre exércitos.

===


==- Batalha Naval

É um formato de batalha onde os jogadores se enfrentam em um campo de batalha aquático, com regras específicas para o combate e a movimentação, na intensão de simular uma batalha entre frotas navais.

Neste formato, o tabuleiro do jogo é adaptado para simular um campo de batalha aquático, e as cartas de recurso são utilizadas para representar navios, armas, tripulantes e outros elementos navais.

---

#### Navios
São cartas de {{ companion }} com a propriedade **Navio (Ship)** e o efeito **Unidade (Unit)**. Neste formato, os navios estão sujeitos a regras específicas de jogo aqui descritas.

Os 7 atributos de um {{ companion }} são transpostos em cada navio da seguinte forma:

| Atributo  | Navio               | Descrição | {.compact}
| ---       | ---                 | ---       |
| {{ enr }} | **Casco**           | Resistência do navio a ataques. Segue a mesma regra de {{ dmg }} do formato _Padrão_ |
| {{ str }} | **Carga**           | Quantidade de carga que o navio pode carregar |
| {{ agi }} | **Velocidade**      | Número máximo de _Contadores de Velocidade_. O número de _Contadores de Velocidade_ que o navio tem define com quanto {{ ap }} o navio começa o seu turno |
| {{ per }} | **Alcance**         | Iniciativa e distância máxima que o navio pode atacar |
| {{ int }} | **Manobrabilidade** | Número de vezes que o navio pode rotacionar por turno |
| {{ cha }} | **Tripulação**      | Número máximo de _Contadores de Tripulação_. Quando o navio não tem mais tripulação, ele não pode jogar |
| {{ spt }} | **Canhões**         | Valor adicionado aos ataques do navio |

---

#### Tabuleiro
* Por padrão todas as casas do tabuleiro são consideradas do tipo {{ aqua }}.
* E em certos mapas podem haver casas na terra, que não são acessíveis as peças de jogo, com prias, costas ou ilhas.

---

#### Peças
* Utilizam-se peças de tabuleiro para representar os navios e as unidades navais em combate.
* É criada uma peça para cada navio, com base em uma carta de navio com a propriedade **Navio**.
* Regras de {{ hp }}, {{ dmg }}, {{ injury }} e efeitos de companheiros são aplicados a cada peça, como se fossem peças de cartas de {{ companion }}.

---

#### Vento
* No início do combate, é rolado um dado de 6 lados para determinar a direção do vento, que pode afetar a movimentação e o ataque dos navios.
    * 1 → O mestre de jogo escolhe a direção do vento
    * 2 → Norte
    * 3 → Leste
    * 4 → Sul
    * 5 → Oeste
    * 6 → Os jogadores escolhem a direção do vento

---

#### Movimentação
* Cada navio tem uma quantidade de pontos de {{ ap }} igual a sua **Velocidade**, que neste formato são utilizados exclusiva mente para movimentação.
    * 1 de {{ ap }} → Mover 1 casa a favor do vento
    * 2 de {{ ap }} → Mover 1 casa perpendicular ao vento
    * 3 de {{ ap }} → Mover 1 casa contra o vento
* É possível rotaciona o navio uma número limitado de vezes por turno. Uma vez que o navio é rotacionado, ele não pode rotacionar novamente neste turno até que se mova pelo menos 1 casa.

---

#### Ataque
* Os navios atacam em apenas de lado para o alvo e se utiliza as regras padrões de cálculo de {{ dmg }}.
* O {{ range }} do ataque é do tipo {{ direct }} e se utiliza as regras padrões de cálculo de distância.
* O navio pode atacar apenas uma vez por turno, sem custos em {{ ap }}, e seu turno encerra após o ataque.
    * **Round Shot**: Canhões + {{ d1d6 }}
    * **Grape Shot**: Canhões + {{ d1d2 }}; Além da {{ hp }}, o alvo perde tripulação igual à {{ injury }}; Este ataque nunca deixa um navio com menos de 1 de tripulação
    * **Chain Shot**: O alvo perde {{ n"1" }} _Contador de Velocidade_; Este ataque não causa {{ dmg }}
    * **Abalroar**: Se ao se mover, a seu navio terminar em uma casa do tabuleiro cuja à sua frente esteja outro navio, se o valor de **Carga** do seu navio for maior que a do outro, você pode colidir com ele e causar {{ n"2" }} de {{ injury }}
    * **Abordar**: Ambos os navios rolam uma competição de ( _Contadores de Tripulação_ + {{ d1d6 }} ), quem perder, perde {{ n"2" }} de **Tripulação**; Em caso de empate, os dois perdem {{ n"1" }} de Tripulação; Se um navio ficar com 0 de tripulação durante uma abordagem, ele passa para o controle do outro time.
* Ataques pelas costas causam {{ n"+3" }} de {{ dmg }}
* Se a {{ hp }} de um navio chegar a 0 ou menos, ele é considerado afundado e retirado do campo de batalha; Ao final da batalha, o time vencedor pode coletar metade da carga dos navios afundados

---

#### Reparar
O Navio pode ser reparado em estaleiros, pagando em {{ price }} por ponto restaurado, utilizando {{ item }} ou Carga.

| Reparo      | Custo | {.compact}
| ---         | ---   |
| Tripulantes | $100  |
| Casco       | $50   |
| Velas       | $25   |

---

#### Cargas
Cada tipo de carga tem um valor de carga específico, que pode ser utilizado para comprar melhorias ou reparar o navio.

| Carga   | Valor  | {.compact}
| ---     | ---    |
| Madeira | $50    |
| Rum     | $100   |
| Chá     | $150   |
| Tabaco  | $200   |
| Açúcar  | $250   |

---

#### Melhorias
Melhorias no navio podem ser adicionados na forma de {{ marker }}.

Cada navio pode ter até 3 melhorias. Sendo que uma vez adicionada a melhoria, ela não pode ser removida.

Melhorias são compradas em estaleiros, pagando com cargas específicas.

| Nome               | Marcador     | Preço                               | Efeito | {.compact}
| ---                | ---          | ---                                 | ---    |
| Cirurgião de Bordo | Quadrado     | 3 de Chá                            | Sacrificar o turno  para recuperar 1 de tripulação |
| Quartermestre      | Triângulo    | 3 de Tabaco                         | {{ p"+2" }} de Tripulação |
| Construtor         | Escudo       | 5 de Madeira                        | Tem que remover o shield primeiro (tem que reparar o navio completamente para recuperar o shild) |
| Carpinteiro        | Coração      | 3 de Madeira                        | Sacrificar o turno para recuperar 1d2 de vida |
| Homem de Armas     | Impacto      | 4 de Rum                            | {{ p"+2" }} em abordagens |
| Sentinela          | Mira         | 3 de Açúcar                         | {{ p"+1" }} de alcance para os canhões |
| Piloto             | Estrela      | 1 de Açúcar e 2 de Tabaco           | {{ p"+1" }} de Velocidade e Manobrabilidade |
| Artilheiro         | Encantamento | 2 de Rum, 1 de Açúcar e 1 de Tabaco | {{ p"+2" }} de Canhões |

---

#### Navio de Comando
Além disso, o navio de comando da frota, chamado de **Naú Capitania (flagship)**, recebe uma melhoria especial, chamada de **Almirante**. Esta melhoria não conta para o limite de 3 melhorias por navio.
* O navio de comando é escolhido antes do início da batalha, e não pode ser trocado durante a batalha.
* O navio de comando recebe +{{ d1d3 }} em todas as rolagens de dados.
* Se o navio de comando for afundado, os navios do outro time recebem {{ n"+2" }} em todas as rolagens de dados

===

---
