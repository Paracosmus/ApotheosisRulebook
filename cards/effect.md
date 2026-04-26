---
label: Efeito
icon: code
order: 60
---

# Efeito

{{ briefing `O efeito de uma carta é um texto que descreve sua função e mecânica, explicando como jogá-la e aplicá-la durante a partida. A função do efeito é conferir habilidades adicionais à carta, comumente extrapolando as regras do jogo e permitindo interações mais complexas em busca de uma vantagem estratégica.` }}

Cada personagem pode utilizar e ativar apenas suas próprias cartas, e apenas durante o seu próprio turno. Certas cartas, porém, especificam que podem ou devem ser ativadas como resposta à uma jogada ou situação de jogo, e neste caso, elas são ativadas durante o turno de outros personagem também.

O efeito é autodescritivo e deve ser interpretado e aplicado de acordo com o texto, levando em consideração as regras gerais e mecânicas do jogo. Observe que, muitas vezes, a função de um efeito é justamente _"quebrar as regras"_, ou seja, permitir ações ou interações que normalmente não seriam possíveis dentro das regras do jogo, e isso é parte do que torna os efeitos interessantes e estratégicos. Nestes casos, o efeito é a regra, e deve ser aplicado exatamente como descrito, mesmo que isso contradiga as regras gerais do jogo, tendo o texto da carta, precedência sobre as regras gerais.

Quando um efeito contradiz as regras gerais do jogo isso é bem descrito e explicado no texto do efeito, não deixando dúvidas sobre como ele deve ser aplicado, dado que o jogador esteja familiarizado com as regras de jogo envolvidas.

O efeito é composto por três partes em seu texto:

[Palavras-Chave](#palavras-chave-de-efeito)
[Requerimentos](#requerimentos-de-ativação)
[Descrição](#descrição-do-efeito)

---

## Palavras-chave de Efeito [!badge text="Keyword" variant="ghost"]

  São palavras ou expressões específicas no início do texto, que indicam ações, condições, ou características comuns, e são utilizadas para simplificar o texto do efeito. Elas são identificadas por uma caixa de texto colorida ao redor da palavra, e cada palavra-chave tem um significado específico.

### Ativação [!badge text="Activation" variant="ghost"]

Este conjunto de palavras-chave indica o tipo de ativação do efeito, ou seja, como ele é ativado e aplicado durante a partida. Ele é importante para determinar a natureza do efeito e como ele é ativado. Este é o único tipo de palavras-chave que é obrigatória para um efeito, ou seja, todo efeito deve possuir uma palavras-chave de ativação, e apenas uma.

==- <span class="fill">{{ activate }}</span> [!badge text="Activate" variant="ghost"]

  Efeitos que precisam ser ativados manualmente pelo jogador apenas em seu próprio turno. Quando um efeito tem esta palavra-chave, este é o efeito resolvido quando o jogador declara a ativação desta carta.

  Se a carta possuir mais de um efeito com esta palavra-chave, o jogador deve escolher qual deles irá ativar.

==- <span class="fill">{{ auto }}</span> [!badge text="Auto" variant="ghost"]

  Efeitos ativados automaticamente, sem necessidade de ação do jogador. Quando um efeito tem esta palavra-chave, ele é ativado automaticamente em resposta a uma situação específica, ou seja, quando as condições de ativação do efeito são atendidas, mesmo quando isso ocorrer no turno de um outro personagem que não seja o que controla esta carta.

  Se várias cartas ou efeitos forem ativados em resposta a uma mesma situação, observe  prioridade de ativação.

==- <span class="fill">{{ permanent }}</span> [!badge text="Permanent" variant="ghost"]

  Efeitos passivos, aplicados instantaneamente e que permanecem continuamente enquanto esta carta estiver em jogo. Quando um efeito tem esta palavra-chave, ele vale a partir do momento em que esta carta é colocada em jogo, não sendo considerado que foi ativado.

===

### Temporização [!badge text="Timing" variant="ghost"]

Determina o momento ou situação específica em que o efeito pode ser ativado, ou seja, quando ele entra em jogo.

Quando um efeito possuir mais de um momento de ativação, ele pode/deve ser ativado em todos os momentos listados, ou seja, sempre que qualquer um dos momentos listados ocorrer, e se o efeito tiver requerimentos de ativação, eles devem ser atendidos para cada momento em que o efeito for ativado separadamente.

==- <span class="fill">{{ onPlay }}</span> [!badge text="On Play" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for colocada em jogo, ou seja, quando esta carta for para a {{ table }} ou {{ scenario }}, ou anexada a outra carta se possuir a palavra-chave {{ attached }}.

==- <span class="fill">{{ onExit }}</span> [!badge text="On Exit" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta deixar de estar em jogo, ou seja, quando esta carta sair da {{ table }}.

==- <span class="fill">{{ onObtain }}</span> [!badge text="On Obtain" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for obtida, ou seja, quando esta carta passar a ser de seu controle, seja indo para o seu {{ inv }}, {{ table }} ou anexada a outra carta.

==- <span class="fill">{{ onReveal }}</span> [!badge text="On Reveal" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for revelada, ou seja, quando esta carta for mostrada para os outros jogadores, seja do {{ inv }} ou outro local, ou quando esta carta for virada para cima na {{ table }}.

==- <span class="fill">{{ onConceal }}</span> [!badge text="On Conceal" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for ocultada, ou seja, quando esta carta for virada para baixo na {{ table }} ou escondida de alguma forma dos outros jogadores, com por exemplo, deixando de estar revelada no {{ inv }}.

==- <span class="fill">{{ onExhaust }}</span> [!badge text="On Exhaust" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for consumida, ou seja, quando esta carta for virada de lado para utilizar suas energias e/ou pagar algum tipo de custo.

==- <span class="fill">{{ onRecover }}</span> [!badge text="On Recover" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for recuperada, ou seja, quando esta carta for virada para sua posição normal como uma forma de recuperação ou recarga de energia.

==- <span class="fill">{{ onDiscard }}</span> [!badge text="On Discard" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for descartada, ou seja, quando esta carta for movida para uma pilha de descarte.

==- <span class="fill">{{ onBury }}</span> [!badge text="On Bury" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for enterrada, ou seja, quando esta carta for colocado no fundo de um baralho.

==- <span class="fill">{{ onBanish }}</span> [!badge text="On Banish" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for banida, ou seja, quando esta carta for movida para uma pilha de cartas banidas.

==- <span class="fill">{{ checking }}</span> [!badge text="When Checking" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem estiver fazendo um teste. O efeito deixara claro o momento exato do teste em que ele pode ser ativado, como por exemplo, "quando for fazer um teste", "antes de rolar os dados", "depois de rolar os dados", etc.

==- <span class="fill">{{ attacking }}</span> [!badge text="When Attacking" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem estiver realizando uma ação de ataque. O efeito deixara claro o momento exato do ataque em que ele pode ser ativado, como por exemplo, "quando for declarar um ataque", "antes de rolar os dados de ataque", "depois de rolar os dados de ataque", etc.

==- <span class="fill">{{ attacked }}</span> [!badge text="When Attacked" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem estiver sendo atacado. O efeito deixara claro o momento exato do ataque em que ele pode ser ativado, como por exemplo, "quando for declarado um ataque contra este personagem", "antes de rolar os dados de defesa", "depois de rolar os dados de defesa", etc.

==- <span class="fill">{{ selected }}</span> [!badge text="When Selected" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem for selecionado como alvo de uma ação.

==- <span class="fill">{{ rolling }}</span> [!badge text="When Rolling" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem estiver rolando dados, seja para um teste, ataque, ou outra situação que envolva rolar dados. O efeito deixara claro o momento exato do rolamento em que ele pode ser ativado, como por exemplo, "Quando for rolar os dados", "adicione ao valor obtidos nos dados", etc.

  - Não incluindo dados aleatórios
  - Não incluindo dados extras em caso de crítico

==- <span class="fill">{{ startOfBattle }}</span> [!badge text="Start of Battle" variant="ghost"]

  Este efeito pode/deve ser ativado no início de uma batalha, antes de qualquer ação ser realizada pelos personagens.

==- <span class="fill">{{ endOfBattle }}</span> [!badge text="End of Battle" variant="ghost"]

  Este efeito pode/deve ser ativado no final de uma batalha, após todas as ações terem sido realizadas pelos personagens e a batalha tiver sido declarada encerrada.

==- <span class="fill">{{ resetPhase }}</span> [!badge text="Reset Phase" variant="ghost"]

  Este efeito pode/deve ser ativado durante a fase de restauração, ou seja, a fase que ocorre entre o final de um ciclo e o início do próximo ciclo, onde os personagens realizam ações de manutenção e preparação para o próximo ciclo.

==- <span class="fill">{{ yourStartPhase }}</span> [!badge text="Your Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do seu primeiro turno neste ciclo, antes de qualquer ação ser realizada por você.

==- <span class="fill">{{ yourEndPhase }}</span> [!badge text="Your End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do seu último turno neste ciclo, quando você declara que encerrou suas ações deste ciclo.

==- <span class="fill">{{ teamMemberStartPhase }}</span> [!badge text="Team Member's Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do primeiro turno de personagens do seu time neste ciclo, incluindo você, antes de qualquer ação ser realizada por aquele personagem.

==- <span class="fill">{{ teamMemberEndPhase }}</span> [!badge text="Team Member's End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do último turno de personagens do seu time neste ciclo, incluindo você, quando aquele personagem declara que encerrou suas ações deste ciclo.

==- <span class="fill">{{ teammateStartPhase }}</span> [!badge text="Teammate's Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do primeiro turno de um personagem do seu time neste ciclo, exceto você, antes de qualquer ação ser realizada por aquele personagem.

==- <span class="fill">{{ teammateEndPhase }}</span> [!badge text="Teammate's End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do último turno de um personagem do seu time neste ciclo, exceto você, quando aquele personagem declara que encerrou suas ações deste ciclo.

==- <span class="fill">{{ opponentStartPhase }}</span> [!badge text="Opponent's Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do primeiro turno de personagens de outros times neste ciclo, antes de qualquer ação ser realizada por aquele personagem.

==- <span class="fill">{{ opponentEndPhase }}</span> [!badge text="Opponent's End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do último turno de personagens de outros times neste ciclo, quando aquele personagem declara que encerrou suas ações deste ciclo.

==- <span class="fill">{{ allStartPhase }}</span> [!badge text="All Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do primeiro turno de qualquer personagem neste ciclo, antes de qualquer ação ser realizada por aquele personagem.

==- <span class="fill">{{ allEndPhase }}</span> [!badge text="All End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do último turno de qualquer personagem neste ciclo, quando aquele personagem declara que encerrou suas ações deste ciclo.

==- <span class="fill">{{ thisCharacterStartPhase }}</span> [!badge text="This Character's Start Phase" variant="ghost"]

  Esta palavra-chave é usada para efeitos em cartas de {{ companion }} que se referem ao próprio personagem, ou seja, o personagem representado por esta carta, e não ao Herói que a controla, como é o caso dos demais efeitos.

  Este efeito pode/deve ser ativado no início do primeiro turno deste {{ companion }} neste ciclo, antes de qualquer ação ser realizada por ele.

==- <span class="fill">{{ thisCharacterEndPhase }}</span> [!badge text="This Character's End Phase" variant="ghost"]

  Esta palavra-chave é usada para efeitos em cartas de {{ companion }} que se referem ao próprio personagem, ou seja, o personagem representado por esta carta, e não ao Herói que a controla, como é o caso dos demais efeitos.

  Este efeito pode/deve ser ativado no final do último turno deste {{ companion }} neste ciclo, quando ele declara que encerrou suas ações deste ciclo.

===

### Limite [!badge text="Limit" variant="ghost"]

Tem a função de limitar ou controlar a quantidade de ativações de um efeito, bem como o seu tempo de duração.

Quando um efeito possuir mais de um limite, todos os limites listados devem ser seguidos para cada ativação do efeito, ou seja, o efeito só pode ser ativado se todos os limites listados puderem ser atendidos e aplicados.

==- <span class="fill">{{ yourTurn }}</span> [!badge text="Your Turn Only" variant="ghost"]

  Este efeito pode/deve ser ativado durante o seu próprio turno, ou seja, quando for a sua vez de jogar. Ele não pode ser ativado durante o turno de outros personagens, mesmo que as condições de ativação sejam atendidas.

==- <span class="fill">{{ oncePerStint }}</span> [!badge text="Once per Stint" variant="ghost"]

  Este efeito só pode ser ativado uma vez por ciclo, ou seja, ele só pode ser ativado uma vez durante o ciclo atual, e não pode ser ativado novamente até o início do próximo ciclo. Note que o próximo ciclo começa já durante a próxima fase de restauração.

==- <span class="fill">{{ oncePerBattle }}</span> [!badge text="Once per Battle" variant="ghost"]

  Este efeito só pode ser ativado uma vez por batalha, ou seja, ele só pode ser ativado uma vez durante a batalha atual, e não pode ser ativado novamente até o início da próxima batalha.

==- <span class="fill">{{ allIn }}</span> [!badge text="All-In" variant="ghost"]

  Para ativar este efeito, o Herói não pode ter realizado nenhuma ação não automática durante este turno, ou seja, ele não pode ter ativado nenhuma carta, nem se mover, atacar, etc..

  Ao ser resolvido, o turno deste Herói termina imediatamente.

==- <span class="fill">{{ noResponse }}</span> [!badge text="No Response" variant="ghost"]

  Ao ser ativado, nenhuma outro efeito pode ser ativado em resposta a este efeito, mesmo efeitos {{ auto }}.

==- <span class="fill">{{ noNegation }}</span> [!badge text="No Negation" variant="ghost"]

  Ao ser ativado, este efeito não pode ser negado por nenhum outro efeito, mesmo efeitos {{ auto }}.

==- <span class="fill">{{ lingering }}</span> [!badge text="Lingering" variant="ghost"]

  Este efeito permanece sendo aplicados por um tempo depois de ativados, mesmo se esta carta deixar de estar em jogo, ou seja, ele continua afetando o jogo normalmente, até que sua duração termine ou seja removido por outro efeito.

  O efeito deve indicar claramente a sua duração, ou seja, por quanto tempo ele permanecerá ativo depois de ser ativado, e isso deve ser seguido rigorosamente. Geralmente seu termino é marcado em ciclos ou momentos chave como “Até o final do turno”, “até o final da batalha”,  o início do seu próximo turno”, etc..

===

### Escopo [!badge text="Scope" variant="ghost"]

Este conjunto de palavras-chave indica de onde o efeito pode ser ativado, ou seja, o local ou situação em que ele pode ser ativado, seja para reduzir ou expandir as possibilidades de ativação do efeito

Quando um efeito possuir mais de um escopo, ele pode/deve ser ativado em todos os escopos listados, ou seja, sempre que qualquer um dos escopos listados ocorrer.

==- <span class="fill">{{ anywhere }}</span> [!badge text="From Anywhere" variant="ghost"]

  Este efeito pode ser ativado de qualquer lugar, ele pode ser ativado mesmo que esta carta não esteja em jogo. Pode ser ativado da mão, pilha de descarte, anexada a outra carta, etc..

  Observe que cartas no limbo são consideradas como não existentes, e portanto não podem ser ativadas.

==- <span class="fill">{{ onTable }}</span> [!badge text="From Table" variant="ghost"]

  Este efeito pode ser ativado apenas se estiver na {{ table }} de um Herói. Não pode ser ativado do {{ inv }} ou {{ scenario }} como esperado normalmente.

==- <span class="fill">{{ hand }}</span> [!badge text="From Hand" variant="ghost"]

  Este efeito pode ser ativado apenas se estiver no {{ inv }} de um Herói. Não pode ser ativado da {{ table }} ou {{ scenario }} como esperado normalmente.

==- <span class="fill">{{ discardPile }}</span> [!badge text="From Discard Pile" variant="ghost"]

  Este efeito pode ser ativado apenas se estiver em uma pilha de descarte.

==- <span class="fill">{{ team }}</span> [!badge text="From Team Member" variant="ghost"]

  Quando esta carta estiver na sua {{ table }}, este efeito pode ser ativado por qualquer Herói do seu time, incluindo você, durante o respectivo turno daquele personagem. O Herói que ativar este efeito é responsável por arcar com os requerimentos, demais custos e consequências de ativar este efeito, e ele é o personagem afetado por este efeito, mesmo que esta carta esteja na {{ table }} de outro Herói do time, além de ser o responsável por selecionar alvos, rolar dados, etc.

==- <span class="fill">{{ attached }}</span> [!badge text="From Attachment" variant="ghost"]

  Este efeito pode ser ativado apenas se esta carta estiver anexada a outra carta, ou seja, este efeito não pode ser ativado se esta carta estiver na {{ table }}, {{ inv }} ou {{ scenario }}.

===

### Tarefa [!badge text="Task" variant="ghost"]

Complementa a ativação do efeito, indicando uma ação adicional que deve ser realizada com esta carta ao ativar o efeito, ou seja, uma ação que deve ser realizada como parte da ativação do efeito antes da resolução do efeito. Pode incluir ações como descartar, banir, ou realizar outras ações específicas. Se a tarefa não puder ser realizada, o efeito não pode ser ativado.

Um efeito nunca possui mais de uma tarefa, mas pode possuir uma tarefa e outros requerimentos de ativação, ou seja, para ativar o efeito, o jogador deve realizar a tarefa e atender os outros requerimentos de ativação listados.

==- <span class="fill">{{ exhaust }}</span> [!badge text="Exhaust" variant="ghost"]

  Consuma esta carta ao ativá-la.

==- <span class="fill">{{ recover }}</span> [!badge text="Recover" variant="ghost"]

  Recupere esta carta ao ativá-la.

==- <span class="fill">{{ discard }}</span> [!badge text="Discard" variant="ghost"]

  Descarte esta carta ao ativá-la.

==- <span class="fill">{{ bury }}</span> [!badge text="Bury" variant="ghost"]

  Enterre esta carta ao ativá-la.

==- <span class="fill">{{ banish }}</span> [!badge text="Banish" variant="ghost"]

  Bane esta carta ao ativá-la.

==- <span class="fill">{{ register }}</span> [!badge text="Register" variant="ghost"]

  Registre esta carta ao ativá-la.

===

---

## Requerimentos de Ativação [!badge text="Requirement" variant="ghost"]

Os requerimentos são entre outros, condições, estados ou custos que devem ser atendidos para que um efeito possa ser ativado. São sempre atendidos, pagos e realizados antes do efeito ser aplicado e podem ser respondidos como qualquer outra ação.

Eles são descritos em texto entre os marcadores visuais {{ req '' }} antes do corpo principal do texto do efeito.

> {{ req 'Requerimento' }}

Múltiplos requerimentos são separados por ponto e vírgula.

> {{ req 'Requerimento 1; Requerimento 2; ...' }}

Os requerimentos vêm na seguinte ordem, porém isso não determina hierarquia entre eles, sendo que todos devem ser igualmente atendidos:

>>> **Custos** → `Descarte`, `consuma`, `enterre`, etc.

  São custos extras que devem ser pagos para ativar este efeito.

  > {{ req 'Custo 1; Custo 2; ...' }}

  > {{ req '**Descarte** um ' + item + '; **Consuma** ' + ( n(2) ) + ' de ' + red }}

>>> **Ações** → `Selecione`, `Mova`, `Role dados`, etc.

  São ações adicionais que devem ser realizadas como parte da ativação deste efeito.

  > {{ req 'Ação 1; Ação 2; ...' }}

  > {{ req 'Selecione 2 ' + companion + ' no tabuleiro; Mova-se para uma casa adjacente; Role ' + d2d3 }}

>>> **Duração** → `Até`, `Enquanto`, `Durante`

  Indica um estado ou situação que precisa existir ou ser mantida.

  > {{ req 'Até <condição>; Enquanto <condição>; Durante <condição>; ...' }}

  > {{ req 'Até que esta carta seja descartada; Enquanto houverem ' + companion + ' no tabuleiro; Durante o turno dos oponentes' }}

>>> **Condição** → `Quando`, `Se`

  Indica um estado ou situação que precisa existir.

  > {{ req 'Quando <condição>; Se <condição>; ...' }}

  > {{ req 'Quando uma ' + skill + ' for ativada; Se você tiver uma ' + summon + ' no ' + support }}

>>>

!!-question Se VS Quando VS Enquanto

Desambiguação.

**Se** denota uma condição que precisa existir naquele momento para o efeito ser ativado, porém não permite que o efeito seja usado como resposta, e se quebrada após a ativação, o efeito é aplicado normalmente.
  - Ex.: {{ req 'Se você tiver uma ' + summon + ' no ' + support }}

**Quando** denota uma condição que precisa acontecer para o efeito ser "engatilhado". No caso, o efeito não pode ser ativado em qualquer momento, mas apenas quando aquela situação ocorrer, e se quebrada após a ativação, o efeito é aplicado normalmente.
  - Ex.: {{ req 'Quando uma ' + skill + ' for ativada' }}

**Enquanto** denota uma condição que precisa ser mantida e se quebrada durante ou depois da aplicação do efeito, o efeito encerra.
  - Ex.: {{ req 'Enquanto houverem ' + companion + ' no tabuleiro' }}

!!!

### Previsão [!badge text="Lookahead" variant="ghost"]

O jogador deve verificar se os requerimentos de um efeito podem ser atendidos inteiramente e simultaneamente, fazendo a previsão de que, ao atender um requerimento, isso não impedirá o atendimento dos demais requerimentos.

Por exemplo: {{ req '**Descarte** uma carta; Se você tiver uma '+ summon + ' no ' + support }}

Se o Herói tiver **apenas uma** {{ summon }} no {{ support }}, para ativar este efeito, ele **não** pode descartar a própria {{ summon }} para atender o primeiro requerimento, pois isso quebraria o segundo requerimento, e o efeito não poderia ser ativado.

---

## Descrição do Efeito

Este é o texto que descreve o que o efeito faz, ou seja, a ação ou interação que ele permite ou causa. Ele é a parte mais importante do efeito, pois é onde está a função real da carta, bem como as instruções e explicações do que deve ser feito.

Deve ser interpretado e aplicado de acordo com o texto, levando em consideração as regras gerais e mecânicas do jogo.

Além disso, alguns conceitos relacionados teóricos inferidos no texto são importantes para a compreensão e aplicação dos efeitos.

==- Momento de Ativação [!badge text="Momentum" variant="ghost"]

  O momento de ativação de um efeito é o momento ou situação específica em que ele pode ser ativado, sendo este um conceito teórico que ajuda a ordenar a sequência de ativação de efeitos. Pode se confundir com o <span class="keyword-timing">timing</span>, mas são conceitos distintos.

  O momento se refere à quando em uma ação este efeito entra em jogo, ou seja, quando ele é aplicado depois de ativado. O texto ou requerimento da carta deve indicar claramente o momento de ativação do efeito através do uso adequado da linguagem, e ele pode ser classificado em três categorias:

  ||| **Antes da ação**

  Este efeito precede a ação que ele encadeou, sendo aplicado antes dela, podendo modificar ou influenciar a ação que ele encadeou.

  - Ex.: `Quando for fazer um teste`, `Quando for ser atacado`, `Quando uma carta for ser ativada`, etc.

  |||

  ||| **Durante a ação**

  É aplicado junto ao desenvolvimento da ação que ele encadeou.

  - `Em um teste você recebe...`, `Durante o seu turno você pode...`, `+1 de AGI`, etc.

  |||

  ||| **Depois da ação**

  É aplicado depois do desenvolvimento da ação que ele encadeou, não tendo como modificar ou influenciar a ação que ele encadeou, mas podendo interagir com o resultado dela.

  - Ex.: `Depois de resolver uma carta`, `Depois de ser atacado`, `Quando for selecionado como alvo`, `Quando sofrer dano`, etc.

  |||

==- Padrões de Escrita [!badge text="Writing Patterns" variant="ghost"]

  ||| **<span class="red">( )</span> Expressões**

  Operações são sempre descritos dentro de parênteses, e os valores envolvidos são descritos usando os ícones e símbolos específicos para cada tipo de valor, como por exemplo:
  (  {{ knowledge }} + {{ int }} + **5** )

  |||

  ||| **<span class="red">➜</span> Atribuição**

  Atribuições são descritas usando a seta, indicando o valor que deve ser atribuído a uma variável ou estado, como por exemplo:
  - Você precisa de {{ str }} ➜ **10** (Significa que o valor de {{ str }} precisa ser exatamente igual a 10)
  - Teste de _Procurar_( {{ per }} ➜ **6** ) (Significa que o valor mínimo neste teste é 6)

  |||

  ||| **<span class="red">✚</span> Maior ou igual**

  {{ cha }} **10✚** (Significa que o valor de {{ cha }} é 10 ou mais)

  |||

  ||| **<span class="red">–</span> Menor ou igual**

  {{ int }} **10–** (Significa que o valor de {{ int }} é 10 ou menos)

  |||

  ||| **<span class="red">✱</span> Multiplicação**

  {{ str }} **✱2** (Significa que o valor de {{ str }} é multiplicado por 2)

  |||

  ||| **<span class="red">➥</span> Spawn**

  ➥ {{ human }} ➜ **2** (Adicione um {{ human }} de nível 2 ao tabuleiro)

  |||

  ||| **<span class="red">●</span> Lista**

  Faz uma lista de informações ou textos, seja para escolha, seja para descrever uma sequência de ações, ou qualquer outra função que se encaixe melhor em formato de lista do que em formato de parágrafo.:
  ● Elemento 1
  ● Elemento 2

  |||

  ||| **<span class="red">❙</span> Separador**

  É utilizado uma barra vertical para separar informações de forma semelhante a uma tabela, tendo função apenas organizacional.
  - {{ cunning }} 2 ❙ {{ instruction }} 2

  |||

  ||| **(mín) (máx)**

  É utilizado para indicar valores mínimos e máximos que uma variável, operação ou teste pode ter, tendo função limitadora.
  - **Ex.:** Você causa {{ p '+1' }} de {{ dmg }} para cada carta no seu {{ inv }} (máx 5)
    - Significa que o valor de {{ dmg }} causado por esta carta é igual a 1 vezes a quantidade de cartas na sua mão, porém o valor máximo de {{ dmg }} extra provido por esta carta é 5, mesmo que haja mais de 5 cartas na sua mão.

  |||

===

---

## Resolução do Efeito

É chamado de resolver o efeito o ato de aplicar o efeito depois de ativado, ou seja, realizar as ações e interações descritas no texto do efeito, seguindo as regras gerais do jogo e as instruções específicas do texto do efeito.

O efeito deve ser resolvido exatamente como descrito no texto, seguindo a ordem das ações e interações conforme elas aparecem no texto, e levando em consideração as regras gerais do jogo.

Durante cada passo da resolução do efeito, os jogadores podem ativar outros efeitos em [resposta](#responder-a-um-efeito), bem como efeitos {{ auto }}.

---

## Responder a um Efeito

O ato de encadear um outro efeito em resposta a um efeito ativado é chamado de responder a um efeito, ou simplesmente, resposta.

O sistema de resolução de efeitos no Apoteose funciona através de uma Pilha Dinâmica baseada em recursividade e momentos distintos de ativação (Requerimento vs. Execução).

### Encadeamento de Resposta

>>> Carta Ativada

  Quando um efeito é ativado ele é colocado na base de uma pilha de efeitos encadeados.

  - Índice 0 (Base): A ativação inicial.
  - Considere que há um holofote na carta ativada, indicando que este é o efeito atualmente em resolução.

  > Ex.: Considere que uma carta qualquer com o seguinte texto de efeito foi ativada:
  > ---
  > {{ activate }}{{ req '**Descarte** uma carta; **Consuma** ' + ( n 2 ) + ' de ' + sp }}
  > **Cure** {{ p '25' }} de {{ hp }} e **Recupere** {{ p '2' }} de {{ mp }}.

>>> Atender os Requerimentos

  Se o efeito ativado possuir requerimentos, eles são atendidos neste momento da ativação.

  Durante o momento em que o jogador está atendendo os requerimentos de um efeito, nenhuma resposta pode ser dada.

  Se o efeito não possuir requerimentos, esta etapa é pulada.

  > Ex.: O jogador descarta uma carta e consome 2 de {{ sp }} para validar o efeito, enquanto ele faz isso, os demais jogadores devem esperar.

>>> Efeito em Espera [!badge text="Halt" variant="ghost"]

  Com todos os requerimentos atendidos, o efeito entra em estado de espera (halt).

  Neste momento, os jogadores podem ativar outros efeitos em resposta à quaisquer uma das ações feitas para validar o efeito base seguindo a regra de **Prioridade de Resposta**.

  Se nenhum outro efeito for ativado em resposta, esta etapa é pulada.

  Se uma resposta for ativada, ela é considerada uma nova ativação de carta e colocada da pilha de encadeamento no índice N+1.
  - Considere que o holofote se move para a nova carta ativada, indicando que esta é a nova carta atualmente em resolução.
  - Recursivamente, tudo que foi feito para a carta base, é feito para a carta N+1, seguindo os mesmos passos, e permitindo respostas em resposta a ela (N+2, N+3, etc).
  - Quando a carta N+1 for resolvida, o holofote volta para a carta base, e o índice N+1 é removido da pilha.
  - Os jogadores podem novamente ativar outros efeitos em resposta à quaisquer uma das ações feitas para validar o efeito base ainda seguindo a regra de **Prioridade de Resposta**.
  - Este também é o momento de ativar efeitos que são aplicados antes da ação que será resolvida no corpo do efeito. Por exemplo, se o efeito base for "Cure 25 de HP", este é o momento de ativar efeitos que são aplicados antes da cura.
    - Se o corpo do efeito apresentar uma lista de opções, como não é possível determinar qual ação será escolhida, os efeitos que podem ser aplicados antes de qualquer uma das opções não podem ser ativados.
  - Apenas quanto todos os jogadores passarem a prioridade, ou seja, não ativarem mais nenhum efeito em resposta, é que o efeito base começa a ser resolvido.

  > Ex.: O jogador ativou uma carta, descartou uma carta e consumiu 2 de {{ sp }} para validar o efeito, e agora o efeito está em espera, e os demais jogadores podem ativar outros efeitos em resposta a qualquer um desses passos, seja em resposta à ativação da carta, seja em resposta ao descarte, seja em resposta ao consumo de {{ sp }}.
  >
  > Para o caso de respostas ao corpo do efeito, do tipo de deve ser executado antes da ação que ele responde. Por exemplo, como aqueles em resposta a "quando {{ hp }} for ser curado" ou "quando {{ mp }} for ser recuperado", também devem ser ativados durante esta etapa, e não depois, pois eles são aplicados antes da ação de cura ou recuperação. Quando o corpo do efeito começar a ser resolvido, o momento de ativação desses efeitos já terá passado.

>>> Resolução

  O efeito deixa o estado de espera e é resolvido seguindo o texto do efeito.

  Os jogadores não podem ativar outros efeitos em resposta a este efeito durante a resolução, a resolução de um efeito deve ser cumprida integralmente primeiro.

  Se a carta ativada não possuir efeito, sendo apenas usada a barra de ativação, o ataque ou ação determinado pela barra é executado.

  > Ex.: O jogador ativou uma carta, descartou uma carta e consumiu 2 de {{ sp }} para validar o efeito, e agora o efeito está sendo resolvido, e os demais jogadores devem esperar tanto pela cura dos 25 de {{ hp }} quanto pela recuperação dos 2 de {{ mp }}.

>>> Responder o Corpo do Efeito

  Este Passo é exatamente igual ao passo de "Efeito em Espera", mas ocorre após a resolução do efeito, que não se encontra mais em espera e sim resolvido, ou seja, os jogadores podem ativar outros efeitos em resposta a quaisquer uma das ações feitas durante a resolução do efeito base seguindo a regra de **Prioridade de Resposta**, permitindo inclusive a entrada de novos índices na pilha de encadeamento.

  Uma vez que nenhum jogador ative mais nenhum efeito em resposta, o processo de resolução do efeito é considerado completo, e o jogo segue normalmente. A pilha de encadeamento é esvaziada, e o holofote volta para o jogo normal, indicando que não há mais nenhum efeito em resolução. O próximo passo do jogo é determinado pelo fluxo normal do jogo.

>>>

### Prioridade de Resposta

Quando um efeito entra na pilha de encadeamento é possível que várias cartas ou jogadores queiram responder a ele. Neste caso deve ser seguida a regra de prioridade de resposta para determinar qual efeito será ativado primeiro, ou seja, qual efeito entrará primeiro na pilha de encadeamento sera resolvido e então liberada para a ativação da próxima resposta.

Observe que a prioridade define apenas quem vai ativar primeiro, mas não impede que os demais jogadores possam ativar seus efeitos em resposta, ou seja, mesmo que um jogador tenha a prioridade para ativar um efeito em resposta, os demais jogadores ainda podem ativar seus efeitos em resposta a este efeito depois da reposta do primeiro ser resolvida.

Todos os efeitos do tipo {{ auto }} que são ativados em resposta a um efeito devem ser todos ativados antes de que os jogadores possam responder manualmente. Eles são ativados seguindo também a ordem de prioridade abaixo.

Uma vez que todos os efeitos {{ auto }} tenham sido ativados, resolvidos e removidos da pilha de encadeamento, os jogadores podem então responder manualmente com os efeitos {{ activate }}, também seguindo a ordem de prioridade abaixo.

1. **Cartas do Cenário**
2. **Cartas de Heróis Oponentes**
3. **Cartas de Heróis do Time**
4. **Cartas do Herói (Ou Herói do Companheiro) do Turno**
5. **Cartas da Pilha de Descarte**
6. **Cartas do Mestre de Jogo**

!!!
Note que uma carta em uma pilha de descarte ou baralho controlados por um Herói são consideradas cartas do Herói, e não cartas da pilha de descarte.
!!!

!!!
Quando se tratar do efeito de uma técnica de um Dummy e não de uma carta, considere o dummy na ordem acima como se ele fosse uma carta controlada por aquele jogador. Portanto o Dummy de um jogador teria precedência sobre as cartas e Dummies do Mestre de Jogo, por exemplo.
!!!

---

## Mudança de Estado Durante a Resolução do Efeito

### Nos Requerimentos

Extraordinariamente, se um efeito era possível no momento da ativação da carta, mas um Encadeamento de Respostas ou outra situação de jogo fez com que os demais requerimentos de ativação do efeito fossem quebradas, a ativação do efeito é então parada, não sendo considerado que o efeito foi negado nem ativado, apenas que não é mais possível dar prosseguimento à jogada, quaisquer custos já pagos não são devolvidos.

### Na Descrição

Extraordinariamente, se os requerimentos de um efeito já foram cumpridos e o efeito já está sendo resolvido, mas um Encadeamento de Respostas ou outra situação de jogo fez com que as condições descritas no texto do efeito fossem quebradas, o que já foi feito é mantido, mas a restante do efeito é ignorado. É considerado que o efeito foi ativado, e não negado, mas que não é mais possível dar prosseguimento à resolução do efeito.

---
