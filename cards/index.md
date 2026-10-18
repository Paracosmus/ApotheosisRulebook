# Cartas

|||{.briefing} [!badge text="Card" variant="ghost"]
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

  São identificadas pelo fundo branco.

  [!card layout="snap" title="House" icon="/static/img/icons/suit_house.svg"](/cards/house.md) [!card layout="snap" title="Class" icon="/static/img/icons/suit_class.svg"](/cards/class.md)
  [!card layout="snap" title="Entity" icon="/static/img/icons/suit_entity.svg"](/cards/entity.md)

  Estas cartas são cartas de composição do personagem, portando não podem ser carregadas em seu [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md). Podem estar apenas em:

  {.list-icon}
  - :icon-check-circle: No espaço apropriado designado da [<span class="main"><b>MESA</b></span>](/hero/table/) de um Herói.
  - :icon-check-circle: Baralhos
  - :icon-check-circle: [<span class="main"><b>ENTREPOSTO</b></span>](/gameplay/stack/trading-post.md)
  - :icon-check-circle: Anexo
  - :icon-check-circle: Zona extra

  Se uma situação de jogo resultar em uma Carta de Ficha estar ou ser envida para outro local que não estes, ela deve ser enviada para o [<span class="main"><b>ENTREPOSTO</b></span>](/gameplay/stack/trading-post.md).

==- Carta de Recurso [!badge text="Asset Card" variant="ghost"]

  > Representam elementos que auxiliam o personagem em sua jornada, como objetos e capacidades.

  São identificadas por um fundo preto.

  [!card layout="snap" title="Item" icon="/static/img/icons/suit_item.svg"](/cards/item.md) [!card layout="snap" title="Skill" icon="/static/img/icons/suit_skill.svg"](/cards/skills.md)

  [!card layout="snap" title="Companion" icon="/static/img/icons/suit_companion.svg"](/cards/companion.md) [!card layout="snap" title="Event" icon="/static/img/icons/suit_event.svg"](/cards/event.md)

  Estas cartas possuem um requerimento de nível mínimo de [<span class="knowledge"><b>CONHECIMENTO</b></span>](/gameplay/knowledge.md), que um Herói precisa ter para ter esta carta em sua [<span class="main"><b>MESA</b></span>](/hero/table/), exceto quando anexadas a uma outra carta. Se uma situação de jogo resultar nesta carta estar ou ser envida para [<span class="main"><b>MESA</b></span>](/hero/table/) de um Herói que não atenda a este requerimento, ela deve ser enviada para o [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) do mesmo.

  #### Valor

  Toda carta de Recurso tem um valor, medido em um recurso próprio do seu naipe: [<span class="item"><b>ITEM</b></span>](/cards/item.md) em [<span class="item"><b>PREÇO</b></span>](/cards/item.md), [<span class="skill"><b>HABILIDADE</b></span>](/cards/skills.md) em [<span class="skill"><b>XP</b></span>](/cards/skills.md), [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) em [<span class="companion"><b>VONTADE</b></span>](/cards/companion.md) e [<span class="event"><b>EVENTO</b></span>](/cards/event.md) em [<span class="event"><b>DESTINO</b></span>](/cards/event.md).

  O valor de um [<span class="item"><b>ITEM</b></span>](/cards/item.md) é o [<span class="item"><b>PREÇO</b></span>](/cards/item.md) impresso na carta. Já o valor dos demais naipes é obtido pelo nível da carta, conforme a tabela de conversão de nível em valor abaixo.

  !!!
  Esta tabela não é exclusiva das cartas de Recurso: o jogo a usa sempre que um nível precisa ser convertido em um valor, como o bônus do nível de [<span class="knowledge"><b>CONHECIMENTO</b></span>](/gameplay/knowledge.md) nos [testes](/gameplay/check.md).
  !!!

  {.striped}
  | Nível | Valor |
  | --- | --- |
  | 0 | **0** |
  | 1 | **1** |
  | 2 | **5** |
  | 3 | **10** |
  | 4 | **20** |
  | 5 | **30** |
  | 6 | **40** |
  | 7 | **50** |
  | 8 | **60** |
  | 9 | **70** |
  | 10 | **80** |

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

==- Vidro [!badge text="Glass" variant="ghost"]

  Este estilo apresenta a arte sobreposta em um fundo translúcido que utiliza as cores da própria ilustração com um efeito de vidro fosco aplicado, dando a impressão de que a ilustração está sobre uma superfície que a reflete. Ele é utilizado para criar um efeito moderno, sendo utilizado em cartas especiais de raridade [<span class="uncommon">INCOMUM</span>](/gameplay/rarity.md) ou superior.

==- Estendida [!badge text="Full Art" variant="ghost"]

  Este estilo apresenta a arte estendida, cobrindo toda a extensão da carta, sem bordas ou molduras. Ele é utilizado para destacar a ilustração bem como apresentar um estética diferenciada, além de adicionar um fator colecionável a mais, sendo utilizado exclusivamente em cartas de raridade [<span class="rare">RARA</span>](/gameplay/rarity.md) ou superior.

===

---

## Artista

Representado pelo ícone de um pincel , o artista é o responsável pela ilustração da carta. Seu nome é creditado no canto inferior, abaixo do nome da carta.

---

## Outros Elementos

Uma carta também pode conter outros elementos, sejam eles comuns a todas as cartas ou específicos de certos naipes.

- Para informações sobre os elementos específicos de cada naipe, consulte a seção de cada um deles.
- Para informações sobre os elementos comuns a todas as cartas, consulte a seção correspondente:

[!card layout="signal"](/gameplay/effect.md) [!card layout="signal"](/gameplay/technique.md)

[!card layout="signal"](/gameplay/tag.md) [!card layout="signal"](/gameplay/collection.md)

[!card layout="signal"](/gameplay/rarity.md)  [!card layout="signal"](/cards/summus/)

---

## Ativar

Para usar uma carta você deve ativá-la, o que é feito ao pagar seu custo e cumprir seus requisitos, se houverem. O processo de ativação é o mesmo para todas as cartas, independentemente do naipe.

Por padrão cada Herói pode ativar apenas as cartas que ele controla, ou seja, as cartas que estão em seu [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md), [<span class="main"><b>MESA</b></span>](/hero/table/) ou anexadas a outras cartas que ele controla. No entanto, algumas cartas podem permitir ou exigir que o jogador ative cartas que ele não controla, como as cartas de outros jogadores ou cartas em zonas específicas como às do [<span class="event"><b>CENÁRIO</b></span>](/gameplay/stack/scenario.md).

||| Cartas em Jogo

  Quando uma carta é ativada da [<span class="main"><b>MESA</b></span>](/hero/table/), anexo ou alguma zona de jogo, ela permanece onde está e como está, a menos que uma carta ou regra do jogo diga o contrário.

||| Cartas na Mão

  Quando uma carta é ativada do [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md), a carta deve ser descartada, a menos que uma carta ou regra do jogo diga o contrário.

  Se a carta possuir uma palavra-chave de tarefa, como [<span class="keyword-task">Descarte</span>](/gameplay/effect.md) ou [<span class="keyword-task">Enterre</span>](/gameplay/effect.md), a tarefa tem precedência, e a carta deve ser enviada para onde a tarefa designar, ao invés de ser descartada.

  Observe que apenas efeitos do tipo [<span class="keyword-activation">Ativar</span>](/gameplay/effect.md) podem ser ativados do [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md). Efeitos [<span class="keyword-activation">Permanente</span>](/gameplay/effect.md) de cartas reveladas no [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) não são ativados, mas valem normalmente enquanto a carta estiver revelada.

|||

Ao declarar a ativação de uma carta, o jogador deve seguir os seguintes passos:

==- Manualmente [<span class="keyword-activation">Ativar</span>](/gameplay/effect.md)

  1. A carta deve possuir um ou mais efeitos com a palavra-chave [<span class="keyword-activation">Ativar</span>](/gameplay/effect.md) ou ter uma barra indicando o <b>DANO</b> e/ou <b>ALCANCE</b>. Se a carta não possuir nenhuma destas características, ela não pode ser ativada manualmente.
     a. Se a carta possuir mais de um efeito com a palavra-chave [<span class="keyword-activation">Ativar</span>](/gameplay/effect.md), o jogador deve escolher qual efeito ele deseja ativar.
  2. Verificar se ele cumpre os requisitos para ativar a carta.
     a. Nível de [<span class="knowledge"><b>CONHECIMENTO</b></span>](/gameplay/knowledge.md) necessário
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

==- Automaticamente [<span class="keyword-activation">Auto</span>](/gameplay/effect.md)

  1. A carta deve possuir um ou mais efeitos com a palavra-chave [<span class="keyword-activation">Auto</span>](/gameplay/effect.md).
     1. Efeitos com a palavra-chave [<span class="keyword-activation">Auto</span>](/gameplay/effect.md) são ativados automaticamente de forma obrigatória quando suas condições de ativação são atendidas.
     2. Se a carta possuir mais de um efeito com a palavra-chave [<span class="keyword-activation">Auto</span>](/gameplay/effect.md), todos os efeitos que puderem ser ativados, serão ativados automaticamente.
  2. Verificar se ele cumpre os requisitos para ativar a carta.
     1. Nível de [<span class="knowledge"><b>CONHECIMENTO</b></span>](/gameplay/knowledge.md) necessário
     2. Verificar se atende aos requisitos determinados por palavras-chave de temporização, tarefas, etc.
     3. outras condições adicionais descritas nos requerimentos do efeito.
     4. Ativações automáticas não possuem custos de ativação em [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) e/ou Energias, se a carta possuir esses custos, eles devem ser considerados para outros efeitos [<span class="keyword-activation">Ativar</span>](/gameplay/effect.md) daquela carta, e ignorados para os efeitos [<span class="keyword-activation">Auto</span>](/gameplay/effect.md).

  Estando todas as condições atendidas, o jogador deve informar a ativação da carta.

  1. Se a carta possuir um <b>ALCANCE</b> do tipo <b>DIRETO</b> ou <b>ARQUEADO</b>, o jogador deve selecionar como o alvo da carta uma peça, ou uma casa vazia do tabuleiro, dentro do alcance.
  2. Aplicar o efeito da carta, seguindo a ordem de resolução dos efeitos conforme descrito no texto da carta e as regras do jogo.
  3. Aplicar o dano da carta, se houver, ao alvo selecionado.
     1. Se a carta possuir um <b>ALCANCE</b> do tipo <b>AREA</b>, o dano é aplicado a todas as peças e casas dentro da área de efeito, sem a necessidade de selecionar um alvo específico.
     2. Observe que alguns efeitos de carta podem especificar que são aplicados após o dano, ao invés de antes, como seria o padrão.

===

---

## Estado da Carta

O estado de uma carta é a condição ou situação em que ela se encontra durante o jogo, podendo influenciar suas interações, mecânicas e sinergias com outros componentes do jogo.

==- <span class="fill">Jogável</span> [!badge text="Playable" variant="ghost"]

  São as cartas cujos efeitos são considerados na partida: estão valendo ou podem ser ativados.

  * Cartas reveladas na [<span class="main"><b>MESA</b></span>](/hero/table/) dos Heróis.
  * Cartas reveladas no [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) dos Heróis.
  * Cartas ocultas no [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) dos Heróis que possuam efeitos [<span class="keyword-scope">Da Mão</span>](/gameplay/effect.md) ou [<span class="keyword-scope">De Qualquer Lugar</span>](/gameplay/effect.md).
    * Apesar de serem consideradas jogáveis, apenas os efeitos [<span class="keyword-scope">Da Mão</span>](/gameplay/effect.md) e [<span class="keyword-scope">De Qualquer Lugar</span>](/gameplay/effect.md) podem/devem ser usados.
  * Cartas que possuem efeitos [<span class="keyword-scope">Do Anexo</span>](/gameplay/effect.md) ou [<span class="keyword-scope">De Qualquer Lugar</span>](/gameplay/effect.md) anexadas a cartas reveladas.
    * Apesar de serem consideradas jogáveis, apenas os efeitos [<span class="keyword-scope">Do Anexo</span>](/gameplay/effect.md) e [<span class="keyword-scope">De Qualquer Lugar</span>](/gameplay/effect.md) podem/devem ser usados.
  * Cartas reveladas no [<span class="event"><b>CENÁRIO</b></span>](/gameplay/stack/scenario.md).
  * Cartas reveladas em [montes de cartas](/gameplay/stack/index.md), conforme o uso do monte.
    * Quando o uso do monte é **Sempre**, todos os efeitos são considerados, exceto os que uma palavra-chave de escopo prende a outro lugar, como [<span class="keyword-scope">Da Mesa</span>](/gameplay/effect.md), [<span class="keyword-scope">Da Mão</span>](/gameplay/effect.md) e [<span class="keyword-scope">Do Anexo</span>](/gameplay/effect.md).
    * Quando o uso do monte é **Com palavra-chave**, apesar de serem consideradas jogáveis, apenas os efeitos [<span class="keyword-scope">De Qualquer Lugar</span>](/gameplay/effect.md) e [<span class="keyword-scope">Da Pilha</span>](/gameplay/effect.md) podem/devem ser usados.
  * Casos Especiais
    * Alguns [<span class="summus"><b>SUMMUS</b></span>](/cards/summus/) estabelecem condições específicas para serem jogáveis, como estar em uma zona específica ou possuir um estado específico.

==- <span class="fill">Não Jogável</span> [!badge text="Unplayable" variant="ghost"]

  São as cartas cujo o efeito não está disponível ou não é de conhecimento público.

  A carta não ser jogável significa apenas que seu efeito não está disponível, os demais aspectos da carta, como energias, valor, peça no tabuleiro, etc., devem ser tratados normalmente.

  * Cartas ocultas na [<span class="main"><b>MESA</b></span>](/hero/table/) dos Heróis.
  * Cartas ocultas no [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) dos Heróis, exceto as que possuam efeitos [<span class="keyword-scope">Da Mão</span>](/gameplay/effect.md) ou [<span class="keyword-scope">De Qualquer Lugar</span>](/gameplay/effect.md).
  * Cartas ocultas no [<span class="event"><b>CENÁRIO</b></span>](/gameplay/stack/scenario.md).
  * Cartas anexadas:
    * Quando estão anexadas a cartas ocultas.
    * Quando não possuem efeitos [<span class="keyword-scope">Do Anexo</span>](/gameplay/effect.md) ou [<span class="keyword-scope">De Qualquer Lugar</span>](/gameplay/effect.md).
  * Cartas ocultas em montes de cartas.
  * Cartas em montes de cartas cujo uso é **Nunca**, como as cartas banidas.
  * Casos Especiais
    * Alguns efeitos de carta podem tornar outras cartas não jogáveis, seja permanentemente ou temporariamente.
    * Alguns [<span class="summus"><b>SUMMUS</b></span>](/cards/summus/) estabelecem condições específicas para não serem jogáveis, como estar em uma zona específica ou possuir um estado específico.

  Em alguns casos, cartas reveladas não jogáveis podem ser colocadas de cabeça para baixo para indicar seu estado.

  !!!
  Cartas no Limbo são desconsideradas, portanto não são consideradas jogáveis nem não jogáveis.
  !!!

==- <span class="fill">Revelada</span> [!badge text="Revealed" variant="ghost"]

  Toda carta de face para cima é considerada revelada, sendo de conhecimento público de todos os jogadores.

  _Anexos são desconsiderados._

==- <span class="fill">Oculta</span> [!badge text="Hidden" variant="ghost"]

  Toda carta de face para baixo ou não revelada no [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) é considerada oculta, sendo de conhecimento privado do jogador que a controla.

  Os demais jogadores devem ter conhecimento da existência de cartas ocultas, mas não de suas informações, como nome, arte, efeitos, etc.. Portanto, eles podem ver que elas estão na [<span class="main"><b>MESA</b></span>](/hero/table/), ou mesmo contar quantas cartas outro jogador tem no [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md).

  _Anexos são desconsiderados._

==- <span class="fill">Restaurada</span> [!badge text="Restored" variant="ghost"]

  Toda carta na posição vertical é considerada restaurada, estando em seu estado natural.

  _Anexos são desconsiderados._

==- <span class="fill">Consumida</span> [!badge text="Exhausted" variant="ghost"]

  Toda carta na posição horizontal é considerada consumida, estando em um estado alterado.

  _Anexos são desconsiderados._

==- <span class="fill">Anexada</span> [!badge text="Attached" variant="ghost"]

  Toda carta que esteja anexada a outra carta.

==- <span class="fill">Exilada</span> [!badge text="Exiled" variant="ghost"]

  Toda carta no Limbo.

===

---
