!!!danger
Esta seção ainda não foi completamente revisada. Algumas informações podem estar desatualizadas ou incompletas, e a formatação pode não estar finalizada.
!!!
    
# Batalha Naval

É um formato de batalha onde os jogadores se enfrentam em um campo de batalha aquático, com regras específicas para o combate e a movimentação, na intensão de simular uma batalha entre frotas navais.

Neste formato, o tabuleiro do jogo é adaptado para simular um campo de batalha aquático, e as cartas de recurso são utilizadas para representar navios, armas, tripulantes e outros elementos navais.

---

#### Navios
São cartas de [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) com a propriedade **Navio (Ship)** e o efeito **Unidade (Unit)**. Neste formato, os navios estão sujeitos a regras específicas de jogo aqui descritas.

Os 7 atributos de um [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) são transpostos em cada navio da seguinte forma:

| Atributo  | Navio               | Descrição | {.compact}
| ---       | ---                 | ---       |
| [<span class="house"><b>CON</b></span>](/hero/attributes.md) | **Casco**           | Resistência do navio a ataques. Segue a mesma regra de <b>DANO</b> do formato _Padrão_ |
| [<span class="house"><b>FOR</b></span>](/hero/attributes.md) | **Carga**           | Quantidade de carga que o navio pode carregar |
| [<span class="house"><b>AGI</b></span>](/hero/attributes.md) | **Velocidade**      | Número máximo de _Contadores de Velocidade_. O número de _Contadores de Velocidade_ que o navio tem define com quanto [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) o navio começa o seu turno |
| [<span class="house"><b>PER</b></span>](/hero/attributes.md) | **Alcance**         | Iniciativa e distância máxima que o navio pode atacar |
| [<span class="house"><b>INT</b></span>](/hero/attributes.md) | **Manobrabilidade** | Número de vezes que o navio pode rotacionar por turno |
| [<span class="house"><b>CAR</b></span>](/hero/attributes.md) | **Tripulação**      | Número máximo de _Contadores de Tripulação_. Quando o navio não tem mais tripulação, ele não pode jogar |
| [<span class="house"><b>ESP</b></span>](/hero/attributes.md) | **Canhões**         | Valor adicionado aos ataques do navio |

---

#### Tabuleiro
* Por padrão todas as casas do tabuleiro são consideradas do tipo <b>AQUA</b>.
* E em certos mapas podem haver casas na terra, que não são acessíveis as peças de jogo, com prias, costas ou ilhas.

---

#### Peças
* Utilizam-se peças de tabuleiro para representar os navios e as unidades navais em combate.
* É criada uma peça para cada navio, com base em uma carta de navio com a propriedade **Navio**.
* Regras de [<span class="hp"><b>VIDA</b></span>](/hero/#vida), <b>DANO</b>, <b>LESÃO</b> e efeitos de companheiros são aplicados a cada peça, como se fossem peças de cartas de [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md).

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
* Cada navio tem uma quantidade de pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) igual a sua **Velocidade**, que neste formato são utilizados exclusiva mente para movimentação.
    * 1 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) → Mover 1 casa a favor do vento
    * 2 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) → Mover 1 casa perpendicular ao vento
    * 3 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) → Mover 1 casa contra o vento
* É possível rotaciona o navio uma número limitado de vezes por turno. Uma vez que o navio é rotacionado, ele não pode rotacionar novamente neste turno até que se mova pelo menos 1 casa.

---

#### Ataque
* Os navios atacam em apenas de lado para o alvo e se utiliza as regras padrões de cálculo de <b>DANO</b>.
* O <b>ALCANCE</b> do ataque é do tipo <b>DIRETO</b> e se utiliza as regras padrões de cálculo de distância.
* O navio pode atacar apenas uma vez por turno, sem custos em [<span class="main"><b>AÇÃO</b></span>](/hero/#ação), e seu turno encerra após o ataque.
    * **Round Shot**: Canhões + 
    * **Grape Shot**: Canhões + ; Além da [<span class="hp"><b>VIDA</b></span>](/hero/#vida), o alvo perde tripulação igual à <b>LESÃO</b>; Este ataque nunca deixa um navio com menos de 1 de tripulação
    * **Chain Shot**: O alvo perde <span class="negative">1</span> _Contador de Velocidade_; Este ataque não causa <b>DANO</b>
    * **Abalroar**: Se ao se mover, a seu navio terminar em uma casa do tabuleiro cuja à sua frente esteja outro navio, se o valor de **Carga** do seu navio for maior que a do outro, você pode colidir com ele e causar <span class="negative">2</span> de <b>LESÃO</b>
    * **Abordar**: Ambos os navios rolam uma competição de ( _Contadores de Tripulação_ +  ), quem perder, perde <span class="negative">2</span> de **Tripulação**; Em caso de empate, os dois perdem <span class="negative">1</span> de Tripulação; Se um navio ficar com 0 de tripulação durante uma abordagem, ele passa para o controle do outro time.
* Ataques pelas costas causam <span class="negative">+3</span> de <b>DANO</b>
* Se a [<span class="hp"><b>VIDA</b></span>](/hero/#vida) de um navio chegar a 0 ou menos, ele é considerado afundado e retirado do campo de batalha; Ao final da batalha, o time vencedor pode coletar metade da carga dos navios afundados

---

#### Reparar
O Navio pode ser reparado em estaleiros, pagando em [<span class="item"><b>PREÇO</b></span>](/cards/item.md) por ponto restaurado, utilizando [<span class="item"><b>ITEM</b></span>](/cards/item.md) ou Carga.

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
Melhorias no navio podem ser adicionados na forma de [<span class="main"><b>MARCADOR</b></span>](/gameplay/characters/#marcadores).

Cada navio pode ter até 3 melhorias. Sendo que uma vez adicionada a melhoria, ela não pode ser removida.

Melhorias são compradas em estaleiros, pagando com cargas específicas.

| Nome               | Marcador     | Preço                               | Efeito | {.compact}
| ---                | ---          | ---                                 | ---    |
| Cirurgião de Bordo | Quadrado     | 3 de Chá                            | Sacrificar o turno  para recuperar 1 de tripulação |
| Quartermestre      | Triângulo    | 3 de Tabaco                         | <span class="positive">+2</span> de Tripulação |
| Construtor         | Escudo       | 5 de Madeira                        | Tem que remover o shield primeiro (tem que reparar o navio completamente para recuperar o shild) |
| Carpinteiro        | Coração      | 3 de Madeira                        | Sacrificar o turno para recuperar 1d2 de vida |
| Homem de Armas     | Impacto      | 4 de Rum                            | <span class="positive">+2</span> em abordagens |
| Sentinela          | Mira         | 3 de Açúcar                         | <span class="positive">+1</span> de alcance para os canhões |
| Piloto             | Estrela      | 1 de Açúcar e 2 de Tabaco           | <span class="positive">+1</span> de Velocidade e Manobrabilidade |
| Artilheiro         | Encantamento | 2 de Rum, 1 de Açúcar e 1 de Tabaco | <span class="positive">+2</span> de Canhões |

---

#### Navio de Comando
Além disso, o navio de comando da frota, chamado de **Naú Capitania (flagship)**, recebe uma melhoria especial, chamada de **Almirante**. Esta melhoria não conta para o limite de 3 melhorias por navio.
* O navio de comando é escolhido antes do início da batalha, e não pode ser trocado durante a batalha.
* O navio de comando recebe + em todas as rolagens de dados.
* Se o navio de comando for afundado, os navios do outro time recebem <span class="negative">+2</span> em todas as rolagens de dados

---
