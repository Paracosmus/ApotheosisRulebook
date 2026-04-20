# Cartas

|||{.briefing} :icon-search:
  São a base do jogo, as partículas que compõem os personagens e eventos. Cada carta possui um conjunto de informações que são utilizadas para dar função e significado.
|||
    
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

  Estas cartas são cartas de composição do personagem, portando não podem ser carregadas em seu [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md). Podem estar apenas em:

  {.list-icon}
  - :icon-check-circle: No espaço apropriado designado da [<span class="main"><b>MESA</b></span>](/hero/table/) de um Herói.
  - :icon-check-circle: Baralhos
  - :icon-check-circle: Pilhas de descarte
  - :icon-check-circle: Anexo
  - :icon-check-circle: Zona extra

  Se uma situação de jogo resultar em uma Carta de Ficha estar ou ser envida para outro local que não estes, ela deve ser enviada para a pilha de descarte.

==- Carta de Recurso [!badge text="Asset Card" variant="ghost"]

  > Representam elementos que auxiliam o personagem em sua jornada, como objetos e capacidades.

  [!card layout="snap" title="Item" icon="/static/img/icons/suit_item.svg"](/cards/item.md) [!card layout="snap" title="Skill" icon="/static/img/icons/suit_skill.svg"](/cards/skills.md)

  [!card layout="snap" title="Companion" icon="/static/img/icons/suit_companion.svg"](/cards/companion.md) [!card layout="snap" title="Event" icon="/static/img/icons/suit_event.svg"](/cards/event.md)

  Estas cartas possuem um requerimento de nível mínimo de [<span class="knowledge"><b>CONHECIMENTO</b></span>](/hero/knowledge.md), que um Herói precisa ter para ter esta carta em sua [<span class="main"><b>MESA</b></span>](/hero/table/), exceto quando anexadas a uma outra carta. Se uma situação de jogo resultar nesta carta estar ou ser envida para [<span class="main"><b>MESA</b></span>](/hero/table/) de um Herói que não atenda a este requerimento, ela deve ser enviada para o [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) do mesmo.

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

  Este estilo apresenta a arte sobreposta em um fundo translúcido que utiliza as cores da própria ilustração com um efeito de vidro fosco aplicado, dando a impressão de que a ilustração está sobre uma superfície que a reflete. Ele é utilizado para criar um efeito moderno, sendo utilizado em cartas especiais de raridade [<span class="uncommon">INCOMUM</span>](/cards/rarity.md) ou superior.

==- Estendida [!badge text="Full Art" variant="ghost"]

  Este estilo apresenta a arte estendida, cobrindo toda a extensão da carta, sem bordas ou molduras. Ele é utilizado para destacar a ilustração bem como apresentar um estética diferenciada, além de adicionar um fator colecionável a mais, sendo utilizado exclusivamente em cartas de raridade [<span class="rare">RARA</span>](/cards/rarity.md) ou superior.

===

---

## Artista

Representado pelo ícone de um pincel , o artista é o responsável pela ilustração da carta. Seu nome é creditado no canto inferior, abaixo do nome da carta.

---

## Outros Elementos

Uma carta também pode conter outros elementos, sejam eles comuns a todas as cartas ou específicos de certos naipes.

- Para informações sobre os elementos específicos de cada naipe, consulte a seção de cada um deles.
- Para informações sobre os elementos comuns a todas as cartas, consulte a seção correspondente:

[!card layout="signal"](/cards/effect.md) [!card layout="signal"](/cards/technique.md)

[!card layout="signal"](/cards/tag.md) [!card layout="signal"](/cards/collection.md)

[!card layout="signal"](/cards/rarity.md)  [!card layout="signal"](/cards/summus/)

---

## Ativar

Para usar uma carta você deve ativá-la, o que é feito ao pagar seu custo e cumprir seus requisitos, se houverem. O processo de ativação é o mesmo para todas as cartas, independentemente do naipe.

Por padrão cada Herói pode ativar apenas as cartas que ele controla, ou seja, as cartas que estão em seu [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md), [<span class="main"><b>MESA</b></span>](/hero/table/) ou anexadas a outras cartas que ele controla. No entanto, algumas cartas podem permitir ou exigir que o jogador ative cartas que ele não controla, como as cartas de outros jogadores ou cartas em zonas específicas como às do [<span class="event"><b>CENÁRIO</b></span>](/gameplay/scenario.md).

||| Cartas em Jogo

  Quando uma carta é ativada da [<span class="main"><b>MESA</b></span>](/hero/table/), anexo ou alguma zona de jogo, ela permanece onde está e como está, a menos que uma carta ou regra do jogo diga o contrário.

||| Cartas na Mão

  Quando uma carta é ativada do [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md), a carta deve ser descartada, a menos que uma carta ou regra do jogo diga o contrário.

  Se a carta possuir uma palavra-chave de tarefa, como [<span class="keyword-task">Descarte</span>](/cards/effect.md) ou [<span class="keyword-task">Enterre</span>](/cards/effect.md), a tarefa tem precedência, e a carta deve ser enviada para onde a tarefa designar, ao invés de ser descartada.

  Observe que apenas efeitos do tipo [<span class="keyword-activation">Ativar</span>](/cards/effect.md) podem ser ativados do [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md).

|||

Ao declarar a ativação de uma carta, o jogador deve seguir os seguintes passos:

==- Manualmente [<span class="keyword-activation">Ativar</span>](/cards/effect.md)

  1. A carta deve possuir um ou mais efeitos com a palavra-chave [<span class="keyword-activation">Ativar</span>](/cards/effect.md) ou ter uma barra indicando o <b>DANO</b> e/ou <b>ALCANCE</b>. Se a carta não possuir nenhuma destas características, ela não pode ser ativada manualmente.
     a. Se a carta possuir mais de um efeito com a palavra-chave [<span class="keyword-activation">Ativar</span>](/cards/effect.md), o jogador deve escolher qual efeito ele deseja ativar.
  2. Verificar se ele cumpre os requisitos para ativar a carta.
     a. Nível de [<span class="knowledge"><b>CONHECIMENTO</b></span>](/hero/knowledge.md) necessário
     a. Pontos [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) necessários
     a. Custos adicionais do naipe, como energias
     a. Verificar se atende aos requisitos determinados por palavras-chave de temporização, tarefas, etc.
     a. outras condições adicionais descritas nos requerimentos do efeito.

  Estando todas as condições atendidas, o jogador pode declarar a ativação da carta.

  1. O Herói deve pagar o custo da carta, se houver, e cumprir os requisitos necessários para ativar a carta.
  2. Se a carta possuir um <b>ALCANCE</b> do tipo <b>DIRETO</b> ou <b>ARQUEADO</b>, o jogador deve selecionar como o alvo da carta uma peça, ou uma casa vazia do tabuleiro, dentro do alcance.
  3. Aplicar o efeito da carta, seguindo a ordem de resolução dos efeitos conforme descrito no texto da carta e as regras do jogo.
  4. Aplicar o dano da carta, se houver, ao alvo selecionado.
     1. Se a carta possuir um <b>ALCANCE</b> do tipo <b>AREA</b>, o dano é aplicado a todas as peças e casas dentro da área de efeito, sem a necessidade de selecionar um alvo específico.
     2. Observe que alguns efeitos de carta podem especificar que são aplicados após o dano, ao invés de antes, como seria o padrão.

  ==- Automaticamente [<span class="keyword-activation">Auto</span>](/cards/effect.md)

  1. A carta deve possuir um ou mais efeitos com a palavra-chave [<span class="keyword-activation">Auto</span>](/cards/effect.md).
     1. Efeitos com a palavra-chave [<span class="keyword-activation">Auto</span>](/cards/effect.md) são ativados automaticamente de forma obrigatória quando suas condições de ativação são atendidas.
     2. Se a carta possuir mais de um efeito com a palavra-chave [<span class="keyword-activation">Auto</span>](/cards/effect.md), todos os efeitos que puderem ser ativados, serão ativados automaticamente.
  2. Verificar se ele cumpre os requisitos para ativar a carta.
     1. Nível de [<span class="knowledge"><b>CONHECIMENTO</b></span>](/hero/knowledge.md) necessário
     2. Verificar se atende aos requisitos determinados por palavras-chave de temporização, tarefas, etc.
     3. outras condições adicionais descritas nos requerimentos do efeito.
     4. Ativações automáticas não possuem custos de ativação em [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) e/ou Energias, se a carta possuir esses custos, eles devem ser considerados para outros efeitos [<span class="keyword-activation">Ativar</span>](/cards/effect.md) daquela carta, e ignorados para os efeitos [<span class="keyword-activation">Auto</span>](/cards/effect.md).

  Estando todas as condições atendidas, o jogador deve informar a ativação da carta.

  1. Se a carta possuir um <b>ALCANCE</b> do tipo <b>DIRETO</b> ou <b>ARQUEADO</b>, o jogador deve selecionar como o alvo da carta uma peça, ou uma casa vazia do tabuleiro, dentro do alcance.
  2. Aplicar o efeito da carta, seguindo a ordem de resolução dos efeitos conforme descrito no texto da carta e as regras do jogo.
  3. Aplicar o dano da carta, se houver, ao alvo selecionado.
     1. Se a carta possuir um <b>ALCANCE</b> do tipo <b>AREA</b>, o dano é aplicado a todas as peças e casas dentro da área de efeito, sem a necessidade de selecionar um alvo específico.
     2. Observe que alguns efeitos de carta podem especificar que são aplicados após o dano, ao invés de antes, como seria o padrão.

===

---
