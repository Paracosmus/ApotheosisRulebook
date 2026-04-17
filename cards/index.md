---
label: Cartas
icon: versions
order: 98
---

# Cartas

{{ briefing `São a base do jogo, as partículas que compõem os personagens e eventos. Cada carta possui um conjunto de informações que são utilizadas para dar função e significado.` }}

As cartas são utilizadas para representar a maioria dos elementos do jogo, como personagens, objetos, habilidades, eventos e outros aspectos temáticos. Elas são a principal forma de interação dos jogadores com o jogo, sendo utilizadas para realizar ações, tomar decisões e progredir na história.

No decorrer da partida, os jogadores coletam cartas para construir seus personagens e progredir no objetivo.

---

## Naipe

O naipe de uma carta é indicado por um ícone no canto superior direito e por uma cor distinta de cada naipe. Ele representa a função daquela carta e como ela interage com o jogo influenciando suas interações, mecânicas e sinergias com outro componentes do jogo.

Existem sete naipes de cartas, cada um com suas próprias características e mecânicas, e eles estão divididos em dois grupos, **Carta de Ficha** e **Carta de Recurso**. O grupo do naipes define a função e a mecânica em comuns para certos naipes, definindo como elas se comportam no jogo.

==- Carta de Ficha [!badge text="Sheet Card" variant="ghost"]

  > Representam características intrínsecas do personagem, como sua origem e ocupação.

  [!card layout="snap" title="House" icon="/static/img/icons/suit_house.svg"](/cards/house.md) [!card layout="snap" title="Class" icon="/static/img/icons/suit_class.svg"](/cards/class.md)
  [!card layout="snap" title="Entity" icon="/static/img/icons/suit_entity.svg"](/cards/entity.md)


  Estas cartas são cartas de composição do personagem, portando não podem ser carregadas em seu {{ inv }}. Podem estar apenas em:

  {.list-icon}
  - :icon-check-circle: No espaço apropriado designado da {{ table }} de um Herói.
  - :icon-check-circle: Baralhos
  - :icon-check-circle: Pilhas de descarte
  - :icon-check-circle: Anexo
  - :icon-check-circle: Zona extra

  Se uma situação de jogo resultar em uma Carta de Ficha estar ou ser envida para outro local que não estes, ela deve ser enviada para a pilha de descarte.

==- Carta de Recurso [!badge text="Asset Card" variant="ghost"]

  > Representam elementos que auxiliam o personagem em sua jornada, como objetos e capacidades.

  [!card layout="snap" title="Item" icon="/static/img/icons/suit_item.svg"](/cards/item.md) [!card layout="snap" title="Skill" icon="/static/img/icons/suit_skill.svg"](/cards/skills.md)

  [!card layout="snap" title="Companion" icon="/static/img/icons/suit_companion.svg"](/cards/companion.md) [!card layout="snap" title="Event" icon="/static/img/icons/suit_event.svg"](/cards/event.md)

  Estas cartas possuem um requerimento de nível mínimo de {{ knowledge }}, que um Herói precisa ter para ter esta carta em sua {{ table }}, exceto quando anexadas a uma outra carta. Se uma situação de jogo resultar nesta carta estar ou ser envida para {{ table }} de um Herói que não atenda a este requerimento, ela deve ser enviada para o {{ inv}} do mesmo.

===

---

## Nome

O nome de uma carta é a palavra ou frase que a identifica, sendo localizado em uma caixa no canto inferior da carta. Ele tem como função dar identidade à carta, além de transmitir o tema e a narrativa.

A sua função é principalmente estética, não sendo utilizado para efeitos de jogo, e pode ser localizado para diferentes idiomas.

---

## Arte

É o conjunto da ilustração da carta, o desenho artístico que a representa, com a moldura (frame). Sendo a parte mais visual e estética da carta, tendo como objetivo representar o tema, além de transmitir a atmosfera e a narrativa da carta.

### Estilo

==- Normal [!badge text="Standard" variant="ghost"]

  Este é o estilo mais comum de ilustração, onde a arte é sobreposta em um fundo branco sem bordas ou molduras definidas, mostrando a arte como um objeto destacável. Este estilo é utilizado para a maioria das cartas, proporcionando uma aparência clássica e organizada.

==- Textura [!badge text="Texture" variant="ghost"]

  Este estilo apresenta a arte sobreposta em um fundo texturizado sem bordas ou molduras definidas, geralmente com um padrão ou design que complementa a ilustração. Ele é utilizado para dar uma sensação mais tátil e visualmente interessante à carta, adicionando profundidade e riqueza à sua aparência, sendo um estilo comum.

==- Vidro [!badge text="Glass" variant="ghost"]

  Este estilo apresenta a arte sobreposta em um fundo translúcido que utiliza as cores da própria ilustração com um efeito de vidro fosco aplicado, dando a impressão de que a ilustração está sobre um vidro que a reflete. Ele é utilizado para criar um efeito visual único e elegante, destacando a arte de uma maneira sofisticada e moderna, sendo utilizado em cartas especiais de raridade {{ uncommon }} ou superior.

==- Estendida [!badge text="Full Art" variant="ghost"]

  Este estilo apresenta a arte estendida, cobrindo toda a extensão da carta, sem bordas ou molduras. Ele é utilizado para destacar a ilustração bem como apresentar um estética diferenciada, além de adicionar um fator colecionável a mais, sendo utilizado exclusivamente em cartas de raridade {{ rare }} ou superior.

===

---

## Artista

Representado pelo ícone de um pincel , o artista é o responsável pela ilustração da carta. Seu nome é creditado no canto inferior, abaixo do nome da carta.

---

## Raridade

A raridade de uma carta é indicada por uma caixinha colorida com uma letra capitalizada, no canto inferior direito. Ela influencia na qualidade da carta, geralmente com um efeito ou status melhores.

Em certos formatos de jogo, a raridade é utilizada para determinar a quantidade de cartas que podem ser incluídas.

{.clean}
| Raridade | Nome |
| -------- | ---- |
| <div class="rarity-box" style="background-color: #9E9E9E">C</div> | <span class="common">COMUM</span>       |
| <div class="rarity-box" style="background-color: #8BC34A">U</div> | <span class="uncommon">INCOMUM</span>   |
| <div class="rarity-box" style="background-color: #01579B">R</div> | <span class="rare">RARA</span>          |
| <div class="rarity-box" style="background-color: #673AB7">E</div> | <span class="epic">ÉPICA</span>         |
| <div class="rarity-box" style="background-color: #FFC400">L</div> | <span class="legendary">LENDÁRIA</span> |

!!!
Narrativamente, também é utilizada para determinar o tipo de [apoteose](/cards/entity.md#ritual-de-apoteose) realizado por um Herói.
!!!

---

## Coleção

O nome da coleção é exibido no canto inferior esquerdo da carta ao lado da barra de raridade, indicando a origem e temática do conjunto de cartas ao qual ela pertence.

Por padrão as coleções não influenciam diretamente nas regras do jogo, mas podem ser utilizadas para limitar o uso de cartas em formatos específicos.

Junto ao nome da coleção está o número indicando a posição daquela carta dentro da coleção e o total de cartas da coleção. O que é utilizado para fins de organização e identificação.

---

## Propriedades

São palavras-chave no canto inferior direito da carta e podem ser identificadas pelo ícone de um quadrado da mesma cor do naipe da carta .

As propriedades não tem função por sí só, mas podem ser utilizadas para interações entre cartas. Sendo geralmente mencionadas no efeito uma carta que interage com outras cartas com determinada propriedade.

---

## Efeito

O efeito de uma carta é um texto que descreve sua função e mecânica, explicando como jogá-la e aplicá-la durante a partida. A função do efeito é conferir habilidades adicionais à carta, comumente extrapolando as regras do jogo e permitindo interações mais complexas em busca de uma vantagem estratégica.

Cada personagem pode utilizar e ativar apenas suas próprias cartas, e apenas durante o seu próprio turno. Certas cartas, porém, especificam que podem ou devem ser ativadas como resposta à uma jogada ou situação de jogo, e neste caso, elas são ativadas durante o turno de outros personagem também.

O efeito é autodescritivo e deve ser interpretado e aplicado de acordo com o texto, levando em consideração as regras gerais e mecânicas do jogo. Observe que, muitas vezes, a função de um efeito é justamente _"quebrar as regras"_, ou seja, permitir ações ou interações que normalmente não seriam possíveis dentro das regras do jogo, e isso é parte do que torna os efeitos interessantes e estratégicos. Nestes casos, o efeito é a regra, e deve ser aplicado exatamente como descrito, mesmo que isso contradiga as regras gerais do jogo, tendo o texto da carta, precedência sobre as regras gerais.

Quando um efeito contradiz as regras gerais do jogo isso é bem descrito e explicado no texto do efeito, não deixando dúvidas sobre como ele deve ser aplicado, dado que o jogador esteja familiarizado com as regras de jogo envolvidas.

O efeito é composto por três partes em seu texto:

==- Palavras-chave de Efeito [!badge text="Keyword" variant="ghost"]

  São palavras ou expressões específicas no início do texto, que indicam ações, condições, ou características comuns, e são utilizadas para simplificar o texto do efeito. Elas são identificadas por uma caixa de texto colorida ao redor da palavra, e cada palavra-chave tem um significado específico.

  <br>

  ### Activation [!badge text="Ativação" variant="ghost"]

  {.clean}
  | Palavras-chave  | PT-BR                                      | Significado |
  | --------------- | ------------------------------------------ | ----------- |
  | {{ activate }}  | [!badge text="Ativar" variant="ghost"]     |  |
  | {{ auto }}      | [!badge text="Auto" variant="ghost"]       |  |
  | {{ permanent }} | [!badge text="Permanente" variant="ghost"] |  |

  <br>

  ### Timing [!badge text="Temporização" variant="ghost"]

  {.clean}
  | Palavras-chave                | PT-BR                                      | Significado |
  | ----------------------------- | ------------------------------------------ | ----------- |
  | {{ onPlay }}                  | [!badge text="Ao Jogar" variant="ghost"]   |  |
  | {{ onExit }}                  | [!badge text="Ao Sair" variant="ghost"]   |  |
  | {{ onObtain }}                | [!badge text="Ao Obter" variant="ghost"]  |  |
  | {{ onReveal }}                | [!badge text="Ao Revelar" variant="ghost"] |  |
  | {{ onConceal }}               | [!badge text="Ao Ocultar" variant="ghost"] |  |
  | {{ onExhaust }}               | [!badge text="Ao Esgotar" variant="ghost"] |  |
  | {{ onRecover }}               | [!badge text="Ao Recuperar" variant="ghost"] |  |
  | {{ onDiscard }}               | [!badge text="Ao Descartar" variant="ghost"] |  |
  | {{ onBury }}                  | [!badge text="Ao Enterrar" variant="ghost"] |  |
  | {{ onBanish }}                | [!badge text="Ao Banir" variant="ghost"] |  |
  | {{ checking }}                | [!badge text="Ao Verificar" variant="ghost"] |  |
  | {{ attacking }}               | [!badge text="Ao Atacar" variant="ghost"] |  |
  | {{ attacked }}                | [!badge text="Ao Ser Atacado" variant="ghost"] |  |
  | {{ selected }}                | [!badge text="Ao Ser Selecionado como Alvo" variant="ghost"] |  |
  | {{ rolling }}                 | [!badge text="Ao Rolar Dados" variant="ghost"] |  |
  | {{ startOfBattle }}           | [!badge text="Início da Batalha" variant="ghost"] |  |
  | {{ endOfBattle }}             | [!badge text="Fim da Batalha" variant="ghost"] |  |
  | {{ resetPhase }}              | [!badge text="Fase de Reset" variant="ghost"] |  |
  | {{ yourStartPhase }}          | [!badge text="Início da Sua Fase" variant="ghost"] |  |
  | {{ yourEndPhase }}            | [!badge text="Fim da Sua Fase" variant="ghost"] |  |
  | {{ teamMemberStartPhase }}    | [!badge text="Início da Fase do Membro da Equipe" variant="ghost"] |  |
  | {{ teamMemberEndPhase }}      | [!badge text="Fim da Fase do Membro da Equipe" variant="ghost"] |  |
  | {{ teammateStartPhase }}      | [!badge text="Início da Fase do Colega de Equipe" variant="ghost"] |  |
  | {{ teammateEndPhase }}        | [!badge text="Fim da Fase do Colega de Equipe" variant="ghost"] |  |
  | {{ opponentStartPhase }}      | [!badge text="Início da Fase do Oponente" variant="ghost"] |  |
  | {{ opponentEndPhase }}        | [!badge text="Fim da Fase do Oponente" variant="ghost"] |  |
  | {{ allStartPhase }}           | [!badge text="Início da Fase de Todos" variant="ghost"] |  |
  | {{ allEndPhase }}             | [!badge text="Fim da Fase de Todos" variant="ghost"] |  |
  | {{ thisCharacterStartPhase }} | [!badge text="Início da Fase deste Personagem" variant="ghost"] |  |
  | {{ thisCharacterEndPhase }}   | [!badge text="Fim da Fase deste Personagem" variant="ghost"] |  |

  <br>

  ### Limit [!badge text="Limite" variant="ghost"]

  {.clean}
  | Palavras-chave  | PT-BR                                      | Significado |
  | --------------- | ------------------------------------------ | ----------- |
  | {{ anywhere }} | [!badge text="Em Qualquer Lugar" variant="ghost"] |  |
  | {{ oncePerStint }} | [!badge text="Uma Vez por Turno" variant="ghost"] |  |
  | {{ oncePerBattle }} | [!badge text="Uma Vez por Batalha" variant="ghost"] |  |
  | {{ allIn }} | [!badge text="Tudo ou Nada" variant="ghost"] |  |
  | {{ noResponse }} | [!badge text="Sem Resposta" variant="ghost"] |  |
  | {{ noNegation }} | [!badge text="Sem Negação" variant="ghost"] |  |
  | {{ lingering }} | [!badge text="Persistente" variant="ghost"] |  |

  <br>

  ### Scope [!badge text="Escopo" variant="ghost"]

  {.clean}
  | Palavras-chave  | PT-BR                                      | Significado |
  | --------------- | ------------------------------------------ | ----------- |
  | {{ yourTurn }} | [!badge text="Apenas no Seu Turno" variant="ghost"] |  |
  | {{ onTable }} | [!badge text="Mesa" variant="ghost"] |  |
  | {{ hand }} | [!badge text="Mão" variant="ghost"] |  |
  | {{ discardPile }} | [!badge text="Monte de Descarte" variant="ghost"] |  |
  | {{ team }} | [!badge text="Membro da Equipe" variant="ghost"] |  |
  | {{ attached }} | [!badge text="Anexado" variant="ghost"] |  |

  <br>

  ### Task [!badge text="Tarefa" variant="ghost"]

  {.clean}
  | Palavras-chave  | PT-BR                                     | Significado |
  | --------------- | ----------------------------------------- | ----------- |
  | {{ exhaust }}   | [!badge text="Esgotar" variant="ghost"]   |  |
  | {{ recover }}   | [!badge text="Recuperar" variant="ghost"] |  |
  | {{ discard }}   | [!badge text="Descartar" variant="ghost"] |  |
  | {{ bury }}      | [!badge text="Enterrar" variant="ghost"]  |  |
  | {{ banish }}    | [!badge text="Banir" variant="ghost"]     |   |
  | {{ register }}  | [!badge text="Registrar" variant="ghost"] |  |

==- Requerimentos de Ativação [!badge text="Requirement" variant="ghost"]

  O efeito não pode ser ativado se qualquer um dos seus requerimentos de ativação não puderem ser atendidos, ou seja, se qualquer um dos requerimentos de ativação não for verdadeiro ou não puder ser cumprido, o efeito não é utilizável naquele momento. Os requerimentos de ativação são geralmente descritos no texto do efeito, e podem incluir custos, condições, estados ou outros requisitos que devem ser atendidos para que o efeito possa ser ativado.:

  1. **Custos** → `Descarte, Consuma, etc.`
  2. **Ações** → `Selecione, Mova`
  3. **Duração** → `Até, Enquanto, Durante`
  4. **Condição** → `Quando, Se, Então`

==- Descrição do Efeito

  Este é o texto que descreve o que o efeito faz, ou seja, a ação ou interação que ele permite ou causa. Ele é a parte mais importante do efeito, pois é onde está a função real da carta, bem como as instruções e explicações do que deve ser feito.

  Deve ser interpretado e aplicado de acordo com o texto, levando em consideração as regras gerais e mecânicas do jogo.

===

Além disso, alguns conceitos relacionados teóricos inferidos no texto são importantes para a compreensão e aplicação dos efeitos.

==- Momento de Ativação [!badge text="Momentum" variant="ghost"]

  O momento de ativação de um efeito é o momento ou situação específica em que ele pode ser ativado, sendo este um conceito teórico que ajuda a ordenar a sequência de ativação de efeitos. Pode se confundir com o <span class="keyword-timing">timing</span>, mas são conceitos distintos.

  O momento se refere à quando em uma ação este efeito entra em jogo, ou seja, quando ele é aplicado depois de ativado. O texto ou requerimento da carta deve indicar claramente o momento de ativação do efeito através do uso adequado da linguagem, e ele pode ser classificado em três categorias:

  Antes da ação -> Quando for fazer um teste, quando for atacado, quando uma carta for ser ativada, etc.

  Durante a ação -> em um teste, em um ataque, etc. (mais comuns em efeitos permanentes de bônus)

  Depois da ação -> Depois de resolver uma carta, depois de ser atacado, quando for selecionado como alvo, quando sofrer dano, etc.

===






---

### Passivo

São efeitos aplicados automaticamente de forma permanente, isso significa que este efeito dura enquanto esta carta estiver em jogo, logo, esta carta não é ativada, seu efeito é aplicado instantaneamente a partir do momento em que esta carta é colocada na {{ table }}.

!!!secondary
Ex.: Efeitos ao estilo _"{{ p'+2' }} de {{ dmg }}"_, _"{{ p'+1' }} de {{ per }}, se sua {{ per }} for menor que 8"_ e _"Este personagem não pode ser alvo de..."_, são todos efeitos passivos.
!!!

### Ativo

Efeitos que precisam ser ativados manualmente pelo jogador ou por uma condição automática, geralmente com um custo associado.

Para identificar uma carta que pode ser ativada, ela precisa possuir uma das seguintes características:

{.list-icon}
- :icon-check-circle: Ter uma _Barra de Ativação_ (presente em algumas cartas de {{ item }} e {{ skill }})
- :icon-check-circle: Ser uma carta de {{ event }}
- :icon-check-circle: Seu texto deve especificar se ela pode ou deve ser ativada, acompanhado de custos e condições, se houverem

!!!secondary
Ex.: Se um efeito diz algo como _"você pode descarte esta carta para..."_, _"Se sua {{ hp }} estiver abaixo de 5, você pode..."_, _"No início do seu turno você pode..."_ e _"Durante o turno de qualquer personagem, você pode..."_, são efeitos ativados manualmente pelo jogador, verificando ou não uma condição limitadora.
!!!

!!!secondary
Ex.: Efeitos na forma _"quando um personagem for atacado você deve..."_, _"Se você sofrer {{ dmg }} descarte uma carta."_ e _"No início do seu turno perca 1 de {{ hp }}."_, são exemplos de efeitos ativados em resposta a uma situação que foi atendida.
!!!

!!!secondary
Ex.: Se um efeito especifica uma ação que não pode ser realizada, aquela carta não pode ser ativada. Observe que é imperativo que o efeito de uma carta possa ser executado em sua completude. Por exemplo, se uma carta diz algo como _"depois de resolver este efeito, descarte uma carta do seu {{ inv }}_", e aquele personagem não tem nenhuma carta no {{ inv }} então este efeito não pode nem mesmo ser iniciado.

Extraordinariamente, se o efeito era possível no momento da ativação da carta, mas as condições mudaram durante a resolução do efeito, o efeito ainda é considerado válido e deve ser resolvido, sendo ignorando a partir da parte que não podem mais ser aplicadas. Por exemplo, se o efeito diz algo como _"depois de resolver este efeito, se você não tiver cartas no {{ inv }}, descarte uma carta do seu {{ table }}"_ e o jogador não tinha cartas no {{ inv }} quando ativou a carta, mas durante a resolução do efeito algo adicionou uma carta ao seu {{ inv }}, ele não precisa mais descartar uma carta da {{ table }}.

Em outro exemplo, se o efeito diz algo como _"depois de resolver este efeito, se você não tiver cartas no {{ inv }}, descarte uma carta do seu {{ table }}"_ e o jogador não tinha cartas no {{ inv }} quando ativou a carta, mas durante a resolução do efeito ficou também sem cartas na sua {{ table }}, ele não pode mais cumprir todas as condições de efeito, o que já foi feito é mantido, mas a restante do efeito não é ignorado.
!!!

Quando você ativar uma carta durante o turno de outro personagem, e esta carta possuir um custo em {{ ap }}, você deve pagar este custo com os pontos que receberia no seu próximo turno, começando o turno com aquela quantidade a menos de {{ ap }}. Se você não tiver {{ ap }} suficientes para pagar o custo, continue "emprestando" pontos de turnos futuros até que a carta esteja paga. Se você já tiver gastado todos os pontos do seu próximo turno, você não pode ativar aquela carta.

!!!
Observe que, todo efeito ativado manualmente ou quando o jogador pode decidir se irá ativar, é um efeito ativo, mesmo que exista uma condição para ativação ou que a ativação seja permitida apenas como resposta a uma situação de jogo.
!!!

!!!
O que difere um efeito passivos de um ativo automático é que o efeito passivo é aplicado instantaneamente ao ser colocado em jogo e permanece afetando-o durante todo o tempo em que esta carta estiver em jogo, enquanto o efeito ativo automático é ativado em resposta a uma situação específica.
!!!


### Palavras-Chave de Efeito [!badge keyword]

Alguns efeitos são descritos utilizando palavras-chave, que são abreviações de ações ou condições comuns, e são utilizadas para simplificar o texto do efeito. As palavras-chave de efeito são identificadas pela caixa de texto colorida ao redor da palavra.

##### Tipo de ativação [!badge activation]
{{ auto }}
:   Efeito ativado automaticamente, sem necessidade de ação do jogador

{{ permanent }}
:   Efeito passivo, aplicado instantaneamente e permanente enquanto esta carta estiver em jogo

{{ temp }}
:   Efeito passivo, aplicado instantaneamente e temporário, tendo sua duração definida no texto do efeito

#### Momento que o efeito pode ser ativado [!badge timing]
{{ onPlay }}
:   Quando esta carta é coloca em jogo, ou seja, quando vai para a {{ table }} de um Herói

{{ onExit }}
:   Quando esta carta é removida da {{ table }} de um Herói, ou seja, quando é descartada, enterrada, banida ou enviada para o {{ inv }}

{{ onObtain }}
:   Quando esta carta é adquirida por um Herói, ou seja, quando é comprada ou recebida de outra forma

{{ onReveal }}
:   Quando esta carta é revelada

{{ onConceal }}
:   Quando esta carta é ocultada

{{ onExhaust }}
:   Quando esta carta é exaurida, ou seja, quando é rotacionada para o lado

{{ onRecover }}
:   Quando esta carta é recuperada, ou seja, quando é rotacionada de volta para a posição normal

{{ onDiscard }}
:   Quando esta carta é descartada

{{ onBury }}
:   Quando esta carta é enterrada

{{ onBanish }}
:   Quando esta carta é banida

{{ startOfYourTurn }}
:   No início do seu turno

{{ endOfYourTurn }}
:   No final do seu turno

{{ startOfTeamTurn }}
:   No início do turno de um personagem do seu time, incluindo você

{{ endOfTeamTurn }}
:   No final do turno de um personagem do seu time, incluindo você

{{ startOfPartnersTurn }}
:   No início do turno de um personagem do seu time que não é você

{{ endOfPartnersTurn }}
:   No final do turno de um personagem do seu time que não é você

{{ startOfOpponentsTurn }}
:   No início do turno de um personagem de outro time

{{ endOfOpponentsTurn }}
:   No final do turno de um personagem de outro time

{{ startOfAllTurns }}
:   No início de todos os turnos, ou seja, no início do turno de todo personagem

{{ endOfAllTurns }}
:   No final de todos os turnos, ou seja, no final do turno de todo personagem

<span style="font-size: 0.8em">{{ startOfThisCharacterTurn }}</span>
:   No início do turno do personagem representado por esta carta de {{ companion }}

<span style="font-size: 0.8em">{{ endOfThisCharacterTurn }}</span>
:   No final do turno do personagem representado por esta carta de {{ companion }}

{{ startOfRound }}
:   No início da rodada

{{ endOfRound }}
:   No final da rodada

{{ startOfBattle }}
:   No início da batalha

{{ endOfBattle }}
:   No final da batalha

{{ checking }}
:   Quando estiver realizando um teste

{{ attacking }}
:   Quando este personagem está atacando

{{ attacked }}
:   Quando este personagem está sendo atacado

<span style="font-size: 0.9em">{{ selected }}</span>
:   Quando este personagem é selecionado como alvo de qualquer ação, incluindo ataques

{{ rolling }}
:  Quando estiver rolando dados.

#### Limite de ativações [!badge limit]
{{ oncePerTurn }}
:   Pode ser ativada apenas uma vez por turno

{{ oncePerRound }}
:   Pode ser ativada apenas uma vez por rodada

{{ oncePerBattle }}
:   Pode ser ativada apenas uma vez por batalha

{{ turnSacrifice }}
:   Para ativar esta carta, você não pode realizar nenhuma outra ação neste turno

{{ noResponse }}
:   Nenhuma carta pode ser ativada em resposta a esta carta

{{ noNegation }}
:   Esta carta não pode ser negada

#### De onde o efeito pode ser ativado [!badge scope]
{{ hand }}
:   Esta carta pode ser ativada do {{ inv }}

{{ discardPile }}
:   Esta carta pode ser ativada da pilha de descarte

{{ team }}
:   Esta carta pode ser ativada por qualquer personagem do seu time, durante o turno dele

#### Ação adicional ao ativar o efeito [!badge task]
{{ discard }}
:   Descarte esta carta após resolvê-la

{{ bury }}
:   Enterre esta carta após resolvê-la

{{ banish }}
:   Bana esta carta após resolvê-la

{{ register }}
:   Envie esta carta para o {{ scenario }} após resolvê-la, se ela já não estiver lá


#### Requerimentos de ativação [!badge requirement]
Condições, estados, ou custos adicionais que devem ser atendidos para que o efeito possa ser ativado.

!!!ghost
❰ <span class="requirement">✔Req.</span> Texto que define o requerimento ❱
❰ <span class="requirement">✔Req.</span> Req 1; Req 2 ❱
❰ <span class="requirement">✔Req.</span> Req 1; Req 2; Req 3; ... ❱
!!!

---



---






Efeitos {{ lingering }} são os únicos que permanacem em funcionando mesmo depois de a carta ser removida de jogo. Note que eles terminam geralmente em valores curtos ou variáveis como, “Até o final do turno”, “até o final da batalha”, “até o início do seu próximo turno”, etc.. Durações constantes como 3 rodadas, 5 rodadas, etc. devem ser usados contadores de tempo.