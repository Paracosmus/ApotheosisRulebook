---
label: Cartas
icon: versions
order: 99
expanded: true
---

# Cartas

Assim como está no nome, as cartas são a base do jogo de APOTHEOSIS, personages e eventos são construídos a partir delas. Cada carta possui um conjunto de informações que são utilizadas para dar função e significado ao jogo.

No decorrer da partida, os jogadores coletam cartas para construir seus personagens e progredir no objetivo.

São utilizados sete naipes de cartas com funções e mecânicas próprias, divididos em dois grupos, que também podem ser identificados pelo layout em que estão dispostos as informações na carta.

**Cartas de Ficha**
:   {{ house }} | {{ class }} | {{ entity }}
    > São utilizadas para representar características intrínsecas do personagem, como sua origem e ocupação.

    **Uso**: Estas cartas podem estar apenas eu seus respectivos baralhos, pilhas de descarte, anexadas, {{ hand }}, ou no espaço apropriado designado da {{ table }} de um Herói. Se uma situação de jogo resultar nesta carta estar ou ser envida para outro local que não estes, ela deve ser enviada para a pilha de descarte.

**Cartas de Recurso**
:   {{ item }} | {{ skill }} | {{ companion }} | {{ event }}
    > São utilizadas para representar elementos que auxiliam o personagem em sua jornada, como objetos e capacidades.

    **Uso**: Estas cartas possuem um requerimento de nível mínimo de {{ knowledge }}, que um Herói precisa ter para ter esta carta em sua {{ table }}, exceto quando anexadas a uma outra carta. Se uma situação de jogo resultar nesta carta estar ou ser envida para {{ table }} de um Herói que não atenda a este requerimento, ela deve ser enviada para o {{ inv}} do mesmo.

---

## Efeito

O efeito de uma carta é um texto que descreve sua função e mecânica, explicando como jogá-la e aplicá-la durante a partida. A função do efeito é conferir habilidades adicionais à carta, comumente extrapolando as regras do jogo e permitindo interações mais complexas em busca de uma vantagem estratégica.

Cada personagem pode utilizar e ativar apenas suas próprias cartas, e apenas durante o seu próprio turno. Certas cartas, porém, especificam que podem ou devem ser ativadas como resposta à uma jogada ou situação de jogo, e neste caso, elas são ativadas durante o turno de outros personagem também.

O efeito de cada carta está disponível para o jogador de duas formas.

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

## Propriedades

São palavras-chave no canto inferior direito da carta e podem ser identificadas pelo ícone de um quadrado da mesma cor do naipe da carta .

As propriedades não tem função por sí só, mas podem ser utilizadas para interações entre cartas. Sendo geralmente mencionadas no efeito uma carta que interage com outras cartas com determinada propriedade.

---

## Raridade

A raridade de uma carta é indicada por uma barra colorida no canto inferior esquerdo. Ela influencia na qualidade da carta, geralmente com um efeito ou status melhores.

Também é utilizada para determinar o tipo de [apoteose](/cards/entity.md#ritual-de-apoteose) realizado por um Herói, e em certos formatos de jogo, a raridade é utilizada para determinar a quantidade de cartas que podem ser incluídas.

<style>

    .rarity-bar {
        width: 35px;
        height: 12px;
        background-color: #BDBDBD;
        display: inline-block;
    }

</style>

* <div class="rarity-bar" style="background-color: #9E9E9E"></div> <span class="common">COMUM</span>
* <div class="rarity-bar" style="background-color: #8BC34A"></div> <span class="uncommon">INCOMUM</span>
* <div class="rarity-bar" style="background-color: #01579B"></div> <span class="rare">RARA</span>
* <div class="rarity-bar" style="background-color: #673AB7"></div> <span class="epic">ÉPICA</span>
* <div class="rarity-bar" style="background-color: #FFC400"></div> <span class="legendary">LENDÁRIA</span>

---

## Coleção

O nome da coleção é exibido no canto inferior esquerdo da carta ao lado da barra de raridade, indicando a origem e temática do conjunto de cartas ao qual ela pertence.

Por padrão as coleções não influenciam diretamente nas regras do jogo, mas podem ser utilizadas para limitar o uso de cartas em formatos específicos.

---

## Ilustração

A ilustração da carta é o desenho que a representa, sendo a parte mais visual e estética da carta e tem como objetivo representar o tema, além de transmitir a atmosfera e a narrativa da carta.

### Full Art

Algumas cartas possuem a arte estendida, que cobre toda a extensão da carta, sem bordas ou molduras. Este estilo de arte é utilizado para destacar a ilustração bem como apresentar um estética diferenciada além de adicionar um fator colecionável a mais.

---

## Artista

Representado pelo ícone de um pincel , o artista é o responsável pela ilustração da carta. Seu nome é creditado no canto inferior.

---
