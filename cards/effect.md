# Efeito

|||{.briefing} :icon-search:
  O efeito de uma carta é um texto que descreve sua função e mecânica, explicando como jogá-la e aplicá-la durante a partida. A função do efeito é conferir habilidades adicionais à carta, comumente extrapolando as regras do jogo e permitindo interações mais complexas em busca de uma vantagem estratégica.
|||
    
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

==- <span class="fill">[<span class="keyword-activation">Ativar</span>](/cards/effect.md)</span> [!badge text="Activate" variant="ghost"]

  Efeitos que precisam ser ativados manualmente pelo jogador apenas em seu próprio turno. Quando um efeito tem esta palavra-chave, este é o efeito resolvido quando o jogador declara a ativação desta carta.

  Se a carta possuir mais de um efeito com esta palavra-chave, o jogador deve escolher qual deles irá ativar.

==- <span class="fill">[<span class="keyword-activation">Auto</span>](/cards/effect.md)</span> [!badge text="Auto" variant="ghost"]

  Efeitos ativados automaticamente, sem necessidade de ação do jogador. Quando um efeito tem esta palavra-chave, ele é ativado automaticamente em resposta a uma situação específica, ou seja, quando as condições de ativação do efeito são atendidas, mesmo quando isso ocorrer no turno de um outro personagem que não seja o que controla esta carta.

  Se várias cartas ou efeitos forem ativados em resposta a uma mesma situação, observe  prioridade de ativação.

==- <span class="fill">[<span class="keyword-activation">Permanente</span>](/cards/effect.md)</span> [!badge text="Permanent" variant="ghost"]

  Efeitos passivos, aplicados instantaneamente e que permanecem continuamente enquanto esta carta estiver em jogo. Quando um efeito tem esta palavra-chave, ele vale a partir do momento em que esta carta é colocada em jogo, não sendo considerado que foi ativado.

===

### Temporização [!badge text="Timing" variant="ghost"]

Determina o momento ou situação específica em que o efeito pode ser ativado, ou seja, quando ele entra em jogo.

Quando um efeito possuir mais de um momento de ativação, ele pode/deve ser ativado em todos os momentos listados, ou seja, sempre que qualquer um dos momentos listados ocorrer, e se o efeito tiver requerimentos de ativação, eles devem ser atendidos para cada momento em que o efeito for ativado separadamente.

==- <span class="fill">[<span class="keyword-timing">Ao Jogar</span>](/cards/effect.md)</span> [!badge text="On Play" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for colocada em jogo, ou seja, quando esta carta for para a [<span class="main"><b>MESA</b></span>](/hero/table/) ou [<span class="event"><b>CENÁRIO</b></span>](/gameplay/scenario.md), ou anexada a outra carta se possuir a palavra-chave [<span class="keyword-scope">Do Anexo</span>](/cards/effect.md).

==- <span class="fill">[<span class="keyword-timing">Ao Sair</span>](/cards/effect.md)</span> [!badge text="On Exit" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta deixar de estar em jogo, ou seja, quando esta carta sair da [<span class="main"><b>MESA</b></span>](/hero/table/).

==- <span class="fill">[<span class="keyword-timing">Ao Obter</span>](/cards/effect.md)</span> [!badge text="On Obtain" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for obtida, ou seja, quando esta carta passar a ser de seu controle, seja indo para o seu [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md), [<span class="main"><b>MESA</b></span>](/hero/table/) ou anexada a outra carta.

==- <span class="fill">[<span class="keyword-timing">Ao Revelar</span>](/cards/effect.md)</span> [!badge text="On Reveal" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for revelada, ou seja, quando esta carta for mostrada para os outros jogadores, seja do [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) ou outro local, ou quando esta carta for virada para cima na [<span class="main"><b>MESA</b></span>](/hero/table/).

==- <span class="fill">[<span class="keyword-timing">Ao Ocultar</span>](/cards/effect.md)</span> [!badge text="On Conceal" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for ocultada, ou seja, quando esta carta for virada para baixo na [<span class="main"><b>MESA</b></span>](/hero/table/) ou escondida de alguma forma dos outros jogadores, com por exemplo, deixando de estar revelada no [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md).

==- <span class="fill">[<span class="keyword-timing">Ao Consumir</span>](/cards/effect.md)</span> [!badge text="On Exhaust" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for consumida, ou seja, quando esta carta for virada de lado para utilizar suas energias e/ou pagar algum tipo de custo.

==- <span class="fill">[<span class="keyword-timing">Ao Recuperar</span>](/cards/effect.md)</span> [!badge text="On Recover" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for recuperada, ou seja, quando esta carta for virada para sua posição normal como uma forma de recuperação ou recarga de energia.

==- <span class="fill">[<span class="keyword-timing">Ao Descartar</span>](/cards/effect.md)</span> [!badge text="On Discard" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for descartada, ou seja, quando esta carta for movida para uma pilha de descarte.

==- <span class="fill">[<span class="keyword-timing">Ao Enterrar</span>](/cards/effect.md)</span> [!badge text="On Bury" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for enterrada, ou seja, quando esta carta for colocado no fundo de um baralho.

==- <span class="fill">[<span class="keyword-timing">Ao Banir</span>](/cards/effect.md)</span> [!badge text="On Banish" variant="ghost"]

  Este efeito pode/deve ser ativado quando esta carta for banida, ou seja, quando esta carta for movida para uma pilha de cartas banidas.

==- <span class="fill">[<span class="keyword-timing">Quando Testando</span>](/cards/effect.md)</span> [!badge text="When Checking" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem estiver fazendo um teste. O efeito deixara claro o momento exato do teste em que ele pode ser ativado, como por exemplo, "quando for fazer um teste", "antes de rolar os dados", "depois de rolar os dados", etc.

==- <span class="fill">[<span class="keyword-timing">Quando Atacando</span>](/cards/effect.md)</span> [!badge text="When Attacking" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem estiver realizando uma ação de ataque. O efeito deixara claro o momento exato do ataque em que ele pode ser ativado, como por exemplo, "quando for declarar um ataque", "antes de rolar os dados de ataque", "depois de rolar os dados de ataque", etc.

==- <span class="fill">[<span class="keyword-timing">Quando Atacado</span>](/cards/effect.md)</span> [!badge text="When Attacked" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem estiver sendo atacado. O efeito deixara claro o momento exato do ataque em que ele pode ser ativado, como por exemplo, "quando for declarado um ataque contra este personagem", "antes de rolar os dados de defesa", "depois de rolar os dados de defesa", etc.

==- <span class="fill">[<span class="keyword-timing">Quando Selecionado</span>](/cards/effect.md)</span> [!badge text="When Selected" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem for selecionado como alvo de uma ação.

==- <span class="fill">[<span class="keyword-timing">Quando Rolando Dados</span>](/cards/effect.md)</span> [!badge text="When Rolling" variant="ghost"]

  Este efeito pode/deve ser ativado quando um personagem estiver rolando dados, seja para um teste, ataque, ou outra situação que envolva rolar dados, não incluindo dados aleatórios. O efeito deixara claro o momento exato do rolamento em que ele pode ser ativado, como por exemplo, "antes de rolar os dados", "depois de rolar os dados", etc.

==- <span class="fill">[<span class="keyword-timing">Início da Batalha</span>](/cards/effect.md)</span> [!badge text="Start of Battle" variant="ghost"]

  Este efeito pode/deve ser ativado no início de uma batalha, antes de qualquer ação ser realizada pelos personagens.

==- <span class="fill">[<span class="keyword-timing">Final da Batalha</span>](/cards/effect.md)</span> [!badge text="End of Battle" variant="ghost"]

  Este efeito pode/deve ser ativado no final de uma batalha, após todas as ações terem sido realizadas pelos personagens e a batalha tiver sido declarada encerrada.

==- <span class="fill">[<span class="keyword-timing">Fase de Recomposição</span>](/cards/effect.md)</span> [!badge text="Reset Phase" variant="ghost"]

  Este efeito pode/deve ser ativado durante a fase de restauração, ou seja, a fase que ocorre entre o final de um ciclo e o início do próximo ciclo, onde os personagens realizam ações de manutenção e preparação para o próximo ciclo.

==- <span class="fill">[<span class="keyword-timing">Sua Fase Inicial</span>](/cards/effect.md)</span> [!badge text="Your Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do seu primeiro turno neste ciclo, antes de qualquer ação ser realizada por você.

==- <span class="fill">[<span class="keyword-timing">Sua Fase Final</span>](/cards/effect.md)</span> [!badge text="Your End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do seu último turno neste ciclo, quando você declara que encerrou suas ações deste ciclo.

==- <span class="fill">[<span class="keyword-timing">Fase Inicial do Membro do Time</span>](/cards/effect.md)</span> [!badge text="Team Member's Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do primeiro turno de personagens do seu time neste ciclo, incluindo você, antes de qualquer ação ser realizada por aquele personagem.

==- <span class="fill">[<span class="keyword-timing">Fase Final do Membro do Time</span>](/cards/effect.md)</span> [!badge text="Team Member's End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do último turno de personagens do seu time neste ciclo, incluindo você, quando aquele personagem declara que encerrou suas ações deste ciclo.

==- <span class="fill">[<span class="keyword-timing">Fase Inicial do Parceiro</span>](/cards/effect.md)</span> [!badge text="Teammate's Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do primeiro turno de um personagem do seu time neste ciclo, exceto você, antes de qualquer ação ser realizada por aquele personagem.

==- <span class="fill">[<span class="keyword-timing">Fase Final do Parceiro</span>](/cards/effect.md)</span> [!badge text="Teammate's End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do último turno de um personagem do seu time neste ciclo, exceto você, quando aquele personagem declara que encerrou suas ações deste ciclo.

==- <span class="fill">[<span class="keyword-timing">Fase Inicial do Oponente</span>](/cards/effect.md)</span> [!badge text="Opponent's Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do primeiro turno de personagens de outros times neste ciclo, antes de qualquer ação ser realizada por aquele personagem.

==- <span class="fill">[<span class="keyword-timing">Fase Final do Oponente</span>](/cards/effect.md)</span> [!badge text="Opponent's End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do último turno de personagens de outros times neste ciclo, quando aquele personagem declara que encerrou suas ações deste ciclo.

==- <span class="fill">[<span class="keyword-timing">Fase Inicial de Todos</span>](/cards/effect.md)</span> [!badge text="All Start Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no início do primeiro turno de qualquer personagem neste ciclo, antes de qualquer ação ser realizada por aquele personagem.

==- <span class="fill">[<span class="keyword-timing">Fase Final de Todos</span>](/cards/effect.md)</span> [!badge text="All End Phase" variant="ghost"]

  Este efeito pode/deve ser ativado no final do último turno de qualquer personagem neste ciclo, quando aquele personagem declara que encerrou suas ações deste ciclo.

==- <span class="fill">[<span class="keyword-timing">Fase Inicial deste Personagem</span>](/cards/effect.md)</span> [!badge text="This Character's Start Phase" variant="ghost"]

  Esta palavra-chave é usada para efeitos em cartas de [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) que se referem ao próprio personagem, ou seja, o personagem representado por esta carta, e não ao Herói que a controla, como é o caso dos demais efeitos.

  Este efeito pode/deve ser ativado no início do primeiro turno deste [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) neste ciclo, antes de qualquer ação ser realizada por ele.

==- <span class="fill">[<span class="keyword-timing">Fase Final deste Personagem</span>](/cards/effect.md)</span> [!badge text="This Character's End Phase" variant="ghost"]

  Esta palavra-chave é usada para efeitos em cartas de [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) que se referem ao próprio personagem, ou seja, o personagem representado por esta carta, e não ao Herói que a controla, como é o caso dos demais efeitos.

  Este efeito pode/deve ser ativado no final do último turno deste [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) neste ciclo, quando ele declara que encerrou suas ações deste ciclo.

===

### Limite [!badge text="Limit" variant="ghost"]

Tem a função de limitar ou controlar a quantidade de ativações de um efeito, bem como o seu tempo de duração.

Quando um efeito possuir mais de um limite, todos os limites listados devem ser seguidos para cada ativação do efeito, ou seja, o efeito só pode ser ativado se todos os limites listados puderem ser atendidos e aplicados.

==- <span class="fill">[<span class="keyword-limit">Apenas no seu Turno</span>](/cards/effect.md)</span> [!badge text="Your Turn Only" variant="ghost"]

  Este efeito pode/deve ser ativado durante o seu próprio turno, ou seja, quando for a sua vez de jogar. Ele não pode ser ativado durante o turno de outros personagens, mesmo que as condições de ativação sejam atendidas.

==- <span class="fill">[<span class="keyword-limit">Uma vez por Ciclo</span>](/cards/effect.md)</span> [!badge text="Once per Stint" variant="ghost"]

  Este efeito só pode ser ativado uma vez por ciclo, ou seja, ele só pode ser ativado uma vez durante o ciclo atual, e não pode ser ativado novamente até o início do próximo ciclo. Note que o próximo ciclo começa já durante a próxima fase de restauração.

==- <span class="fill">[<span class="keyword-limit">Uma vez por Batalha</span>](/cards/effect.md)</span> [!badge text="Once per Battle" variant="ghost"]

  Este efeito só pode ser ativado uma vez por batalha, ou seja, ele só pode ser ativado uma vez durante a batalha atual, e não pode ser ativado novamente até o início da próxima batalha.

==- <span class="fill">[<span class="keyword-limit">Ação Total</span>](/cards/effect.md)</span> [!badge text="All-In" variant="ghost"]

  Para ativar este efeito, o Herói não pode ter realizado nenhuma ação não automática durante este turno, ou seja, ele não pode ter ativado nenhuma carta, nem se mover, atacar, etc..

  Ao ser resolvido, o turno deste Herói termina imediatamente.

==- <span class="fill">[<span class="keyword-limit">Não Respondível</span>](/cards/effect.md)</span> [!badge text="No Response" variant="ghost"]

  Ao ser ativado, nenhuma outro efeito pode ser ativado em resposta a este efeito, mesmo efeitos [<span class="keyword-activation">Auto</span>](/cards/effect.md).

==- <span class="fill">[<span class="keyword-limit">Não Negável</span>](/cards/effect.md)</span> [!badge text="No Negation" variant="ghost"]

  Ao ser ativado, este efeito não pode ser negado por nenhum outro efeito, mesmo efeitos [<span class="keyword-activation">Auto</span>](/cards/effect.md).

==- <span class="fill">[<span class="keyword-limit">Residual</span>](/cards/effect.md)</span> [!badge text="Lingering" variant="ghost"]

  Este efeito permanece sendo aplicados por um tempo depois de ativados, mesmo se esta carta deixar de estar em jogo, ou seja, ele continua afetando o jogo normalmente, até que sua duração termine ou seja removido por outro efeito.

  O efeito deve indicar claramente a sua duração, ou seja, por quanto tempo ele permanecerá ativo depois de ser ativado, e isso deve ser seguido rigorosamente. Geralmente seu termino é marcado em ciclos ou momentos chave como “Até o final do turno”, “até o final da batalha”,  o início do seu próximo turno”, etc..

===

### Escopo [!badge text="Scope" variant="ghost"]

Este conjunto de palavras-chave indica de onde o efeito pode ser ativado, ou seja, o local ou situação em que ele pode ser ativado, seja para reduzir ou expandir as possibilidades de ativação do efeito

Quando um efeito possuir mais de um escopo, ele pode/deve ser ativado em todos os escopos listados, ou seja, sempre que qualquer um dos escopos listados ocorrer.

==- <span class="fill">[<span class="keyword-scope">De Qualquer Lugar</span>](/cards/effect.md)</span> [!badge text="From Anywhere" variant="ghost"]

  Este efeito pode ser ativado de qualquer lugar, ele pode ser ativado mesmo que esta carta não esteja em jogo. Pode ser ativado da mão, pilha de descarte, anexada a outra carta, etc..

  Observe que cartas no limbo são consideradas como não existentes, e portanto não podem ser ativadas.

==- <span class="fill">[<span class="keyword-scope">Da Mesa</span>](/cards/effect.md)</span> [!badge text="From Table" variant="ghost"]

  Este efeito pode ser ativado apenas se estiver na [<span class="main"><b>MESA</b></span>](/hero/table/) de um Herói. Não pode ser ativado do [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) ou [<span class="event"><b>CENÁRIO</b></span>](/gameplay/scenario.md) como esperado normalmente.

==- <span class="fill">[<span class="keyword-scope">Da Mão</span>](/cards/effect.md)</span> [!badge text="From Hand" variant="ghost"]

  Este efeito pode ser ativado apenas se estiver no [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) de um Herói. Não pode ser ativado da [<span class="main"><b>MESA</b></span>](/hero/table/) ou [<span class="event"><b>CENÁRIO</b></span>](/gameplay/scenario.md) como esperado normalmente.

==- <span class="fill">[<span class="keyword-scope">Da Pilha de Descarte</span>](/cards/effect.md)</span> [!badge text="From Discard Pile" variant="ghost"]

  Este efeito pode ser ativado apenas se estiver em uma pilha de descarte.

==- <span class="fill">[<span class="keyword-scope">Do Membro do Time</span>](/cards/effect.md)</span> [!badge text="From Team Member" variant="ghost"]

  Quando esta carta estiver na sua [<span class="main"><b>MESA</b></span>](/hero/table/), este efeito pode ser ativado por qualquer Herói do seu time, incluindo você, durante o respectivo turno daquele personagem. O Herói que ativar este efeito é responsável por arcar com os requerimentos, demais custos e consequências de ativar este efeito, e ele é o personagem afetado por este efeito, mesmo que esta carta esteja na [<span class="main"><b>MESA</b></span>](/hero/table/) de outro Herói do time, além de ser o responsável por selecionar alvos, rolar dados, etc.

==- <span class="fill">[<span class="keyword-scope">Do Anexo</span>](/cards/effect.md)</span> [!badge text="From Attachment" variant="ghost"]

  Este efeito pode ser ativado apenas se esta carta estiver anexada a outra carta, ou seja, este efeito não pode ser ativado se esta carta estiver na [<span class="main"><b>MESA</b></span>](/hero/table/), [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) ou [<span class="event"><b>CENÁRIO</b></span>](/gameplay/scenario.md).

===

### Tarefa [!badge text="Task" variant="ghost"]

Complementa a ativação do efeito, indicando uma ação adicional que deve ser realizada com esta carta ao ativar o efeito, ou seja, uma ação que deve ser realizada como parte da ativação do efeito antes da resolução do efeito. Pode incluir ações como descartar, banir, ou realizar outras ações específicas. Se a tarefa não puder ser realizada, o efeito não pode ser ativado.

Um efeito nunca possui mais de uma tarefa, mas pode possuir uma tarefa e outros requerimentos de ativação, ou seja, para ativar o efeito, o jogador deve realizar a tarefa e atender os outros requerimentos de ativação listados.

==- <span class="fill">[<span class="keyword-task">Consuma</span>](/cards/effect.md)</span> [!badge text="Exhaust" variant="ghost"]

  Consuma esta carta ao ativá-la.

==- <span class="fill">[<span class="keyword-task">Recupere</span>](/cards/effect.md)</span> [!badge text="Recover" variant="ghost"]

  Recupere esta carta ao ativá-la.

==- <span class="fill">[<span class="keyword-task">Descarte</span>](/cards/effect.md)</span> [!badge text="Discard" variant="ghost"]

  Descarte esta carta ao ativá-la.

==- <span class="fill">[<span class="keyword-task">Enterre</span>](/cards/effect.md)</span> [!badge text="Bury" variant="ghost"]

  Enterre esta carta ao ativá-la.

==- <span class="fill">[<span class="keyword-task">Bane</span>](/cards/effect.md)</span> [!badge text="Banish" variant="ghost"]

  Bane esta carta ao ativá-la.

==- <span class="fill">[<span class="keyword-task">Registre</span>](/cards/effect.md)</span> [!badge text="Register" variant="ghost"]

  Registre esta carta ao ativá-la.

===

---

## Requerimentos de Ativação [!badge text="Requirement" variant="ghost"]

Os requerimentos são entre outros, condições, estados ou custos que devem ser atendidos para que um efeito possa ser ativado. São sempre atendidos, pagos e realizados antes do efeito ser aplicado e podem ser respondidos como qualquer outra ação.

Eles são descritos em texto entre os marcadores visuais <span class="req">【</span>  <span class="req">】</span> antes do corpo principal do texto do efeito.

> <span class="req">【</span> Requerimento <span class="req">】</span>

Múltiplos requerimentos são separados por ponto e vírgula.

> <span class="req">【</span> Requerimento 1; Requerimento 2; ... <span class="req">】</span>

Os requerimentos vêm na seguinte ordem, porém isso não determina hierarquia entre eles, sendo que todos devem ser igualmente atendidos:

>>> **Custos** → `Descarte`, `consuma`, `enterre`, etc.

  São custos extras que devem ser pagos para ativar este efeito.

  > <span class="req">【</span> Custo 1; Custo 2; ... <span class="req">】</span>

  > <span class="req">【</span> **Descarte** um [<span class="item"><b>ITEM</b></span>](/cards/item.md); **Consuma** <span class="negative">2</span> de [<span class="skill"><span class="red"><b>VERMELHA</b></span>](/cards/skills.md#essência) <span class="req">】</span>

>>> **Ações** → `Selecione`, `Mova`, `Role dados`, etc.

  São ações adicionais que devem ser realizadas como parte da ativação deste efeito.

  > <span class="req">【</span> Ação 1; Ação 2; ... <span class="req">】</span>

  > <span class="req">【</span> Selecione 2 [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) no tabuleiro; Mova-se para uma casa adjacente; Role  <span class="req">】</span>

>>> **Duração** → `Até`, `Enquanto`, `Durante`

  Indica um estado ou situação que precisa existir ou ser mantida.

  > <span class="req">【</span> Até <condição>; Enquanto <condição>; Durante <condição>; ... <span class="req">】</span>

  > <span class="req">【</span> Até que esta carta seja descartada; Enquanto houverem [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) no tabuleiro; Durante o turno dos oponentes <span class="req">】</span>

>>> **Condição** → `Quando`, `Se`

  Indica um estado ou situação que precisa existir.

  > <span class="req">【</span> Quando <condição>; Se <condição>; ... <span class="req">】</span>

  > <span class="req">【</span> Quando uma [<span class="skill"><b>HABILIDADE</b></span>](/cards/skills.md) for ativada; Se você tiver uma [<span class="companion"><b>EVOCAÇÃO</b></span>](/cards/companion.md#-evocação) no [<span class="companion"><b>SUPORTE</b></span>](/hero/table/support.md) <span class="req">】</span>

>>>

!!-question Se VS Quando VS Enquanto

Desambiguação.

**Se** denota uma condição que precisa existir naquele momento para o efeito ser ativado, porém não permite que o efeito seja usado como resposta, e se quebrada após a ativação, o efeito é aplicado normalmente.
  - Ex.: <span class="req">【</span> Se você tiver uma [<span class="companion"><b>EVOCAÇÃO</b></span>](/cards/companion.md#-evocação) no [<span class="companion"><b>SUPORTE</b></span>](/hero/table/support.md) <span class="req">】</span>

**Quando** denota uma condição que precisa acontecer para o efeito ser "engatilhado". No caso, o efeito não pode ser ativado em qualquer momento, mas apenas quando aquela situação ocorrer, e se quebrada após a ativação, o efeito é aplicado normalmente.
  - Ex.: <span class="req">【</span> Quando uma [<span class="skill"><b>HABILIDADE</b></span>](/cards/skills.md) for ativada <span class="req">】</span>

**Enquanto** denota uma condição que precisa ser mantida e se quebrada durante ou depois da aplicação do efeito, o efeito encerra.
  - Ex.: <span class="req">【</span> Enquanto houverem [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) no tabuleiro <span class="req">】</span>

!!!

### Previsão [!badge text="Lookahead" variant="ghost"]

O jogador deve verificar se os requerimentos de um efeito podem ser atendidos inteiramente e simultaneamente, fazendo a previsão de que, ao atender um requerimento, isso não impedirá o atendimento dos demais requerimentos.

Por exemplo: <span class="req">【</span> **Descarte** uma carta; Se você tiver uma [<span class="companion"><b>EVOCAÇÃO</b></span>](/cards/companion.md#-evocação) no [<span class="companion"><b>SUPORTE</b></span>](/hero/table/support.md) <span class="req">】</span>

Se o Herói tiver **apenas uma** [<span class="companion"><b>EVOCAÇÃO</b></span>](/cards/companion.md#-evocação) no [<span class="companion"><b>SUPORTE</b></span>](/hero/table/support.md), para ativar este efeito, ele **não** pode descartar a própria [<span class="companion"><b>EVOCAÇÃO</b></span>](/cards/companion.md#-evocação) para atender o primeiro requerimento, pois isso quebraria o segundo requerimento, e o efeito não poderia ser ativado.

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
  (  [<span class="knowledge"><b>CONHECIMENTO</b></span>](/hero/knowledge.md) + [<span class="house"><b>INT</b></span>](/hero/attributes.md) + **5** )

  |||

  ||| **<span class="red">➜</span> Atribuição**

  Atribuições são descritas usando a seta, indicando o valor que deve ser atribuído a uma variável ou estado, como por exemplo:
  - Você precisa de [<span class="house"><b>FOR</b></span>](/hero/attributes.md) ➜ **10** (Significa que o valor de [<span class="house"><b>FOR</b></span>](/hero/attributes.md) precisa ser exatamente igual a 10)
  - Teste de _Procurar_( [<span class="house"><b>PER</b></span>](/hero/attributes.md) ➜ **6** ) (Significa que o valor mínimo neste teste é 6)

  |||

  ||| **<span class="red">✚</span> Maior ou igual**

  [<span class="house"><b>CAR</b></span>](/hero/attributes.md) **10✚** (Significa que o valor de [<span class="house"><b>CAR</b></span>](/hero/attributes.md) é 10 ou mais)

  |||

  ||| **<span class="red">–</span> Menor ou igual**

  [<span class="house"><b>INT</b></span>](/hero/attributes.md) **10–** (Significa que o valor de [<span class="house"><b>INT</b></span>](/hero/attributes.md) é 10 ou menos)

  |||

  ||| **<span class="red">✱</span> Multiplicação**

  [<span class="house"><b>FOR</b></span>](/hero/attributes.md) **✱2** (Significa que o valor de [<span class="house"><b>FOR</b></span>](/hero/attributes.md) é multiplicado por 2)

  |||

  ||| **<span class="red">➥</span> Spawn**

  ➥ [<span class="companion"><b>HUMANO</b></span>](/cards/companion.md#-humano) ➜ **2** (Adicione um [<span class="companion"><b>HUMANO</b></span>](/cards/companion.md#-humano) de nível 2 ao tabuleiro)

  |||

  ||| **<span class="red">●</span> Lista**

  Faz uma lista de informações ou textos, seja para escolha, seja para descrever uma sequência de ações, ou qualquer outra função que se encaixe melhor em formato de lista do que em formato de parágrafo.:
  ● Elemento 1
  ● Elemento 2

  |||

  ||| **<span class="red">❙</span> Separador**

  É utilizado uma barra vertical para separar informações de forma semelhante a uma tabela, tendo função apenas organizacional.
  - [<span class="knowledge"><b>ASTÚCIA</b></span>](/hero/knowledge.md#astúcia) 2 ❙ [<span class="knowledge"><b>INSTRUÇÃO</b></span>](/hero/knowledge.md#instrução) 2

  |||

===

---

## Resolução do Efeito

É chamado de resolver o efeito o ato de aplicar o efeito depois de ativado, ou seja, realizar as ações e interações descritas no texto do efeito, seguindo as regras gerais do jogo e as instruções específicas do texto do efeito.

O efeito deve ser resolvido exatamente como descrito no texto, seguindo a ordem das ações e interações conforme elas aparecem no texto, e levando em consideração as regras gerais do jogo.

Durante cada passo da resolução do efeito, os jogadores podem ativar outros efeitos em [resposta](#responder-a-um-efeito), bem como efeitos [<span class="keyword-activation">Auto</span>](/cards/effect.md).

---

## Responder a um Efeito

O ato de encadear um outro efeito em resposta a um efeito ativado é chamado de responder a um efeito, ou simplesmente, resposta.

- Apenas um efeito do tipo pode ser ativado em resposta a um efeito, seguindo a , e os efeitos [<span class="keyword-activation">Auto</span>](/cards/effect.md) podem ser ativados normalmente em resposta a um efeito, seguindo a **Prioridade de Resposta**.

TODO: Dá para liberar geral, em vez de apenas um? Os autos são todos, então seria uma regra unificada?

Quando um efeito entra em reposta a outro efeito, é iniciado uma cadeia de respostas, e outros efeitos podem ser adicionados a essa cadeia.

==- Prioridade de Resposta [!badge text="Priority" variant="ghost"]

  > "_Cada ação pode ter apenas uma reação_"

  Apenas um efeito pode ser ativado em resposta a uma mesma situação, ou seja, quando uma situação de jogo ocorre e múltiplos efeitos são ativados em resposta a ela, apenas um desses efeitos pode ser ativado, e os outros efeitos não podem ser ativados em resposta a aquela mesma situação.

  Note que, por ação, não se refere ao conjunto total, mas cada parte de uma ação em si.

  !!-
  Por exemplo, se um personagem é atacada, é feito a ação de ativar uma carta, selecionar um alvo, rolar os dados, aplicar o dano/lesão, remover a vida do alvo, etc. Cada uma dessas partes é uma ação, e cada uma delas pode ter efeitos ativados em resposta a ela, mas apenas um efeito pode ser ativado em resposta a cada parte dessa ação.

  Então, se um personagem é atacado e você tem uma carta para quando é atacado e outra para quando é selecionado como alvo, ambas podem ser ativadas, em seus respectivos momentos, sendo que "atacado" é o conjunto de ações, portanto ativa primeiro, assim que o ataque é declarado, e "selecionado como alvo" é uma parte daquela ação, portanto ativa depois, assim que o alvo é declarado.
  !!!

  1. **Cartas do Cenário**
    * Se mais de uma carta do Cenário for ativada em resposta a mesma situação, a carta a mais tempo em jogo será ativada.
  2. **Cartas de Heróis Oponentes**
    * Se mais de uma carta de Herói Oponente for ativada em resposta a mesma situação, a carta do Herói Oponente de maior Iniciativa neste ciclo será ativada.
  3. **Cartas de Heróis do Time**
    * Se mais de uma carta de Herói do Time for ativada em resposta a mesma situação, a carta do Herói de maior Iniciativa neste ciclo do Time será ativada.
  4. **Cartas do Herói (Ou Herói do Companheiro) do Turno**
    * Se mais de uma carta do Herói do Turno for ativada em resposta a mesma situação, o jogador deve escolher qual delas será ativada.
  5. **Cartas da Pilha de Descarte**
    * Se mais de uma carta da Pilha de Descarte for ativada em resposta a mesma situação, a carta mais acima na pilha será ativada.
  6. **Cartas do Mestre de Jogo**
    * Se mais de uma carta do Mestre de Jogo for ativada em resposta a mesma situação, cabe ao Mestre de Jogo escolher qual delas será ativada.

  !!!
  Note que uma carta em uma pilha de descarta controlada por um Herói são consideradas cartas do Herói, e não cartas da pilha de descarte.
  !!!

  !!!
  Quando se tratar do efeito de uma técnica de um Dummy e não de uma carta, considere o dummy na ordem acima como se ele fosse uma carta controlada por aquele jogador. Portanto o Dummy de um jogador teria precedência sobre as cartas e Demmies do Mestre de Jogo, por exemplo.
  !!!

===

### Encadeamento de Resposta

Quando vários efeitos estão encadeados, eles são resolvidos na ordem inversa à qual foram ativados, ou seja, o último efeito a ser ativado é o primeiro a ser resolvido, e o primeiro efeito a ser ativado é o último a ser resolvido. Sempre levando em consideração as mudanças de estado que podem ocorrer durante a resolução de cada efeito, e como isso pode afetar os demais efeitos na cadeia.

Quando múltiplos efeitos são ativados em resposta a uma mesma ação, eles entram na cadeia de respostas na seguinte ordem.

1. **Cartas do Cenário**
2. **Cartas de Heróis Oponentes**
3. **Cartas de Heróis do Time**
3. **Cartas do Herói (Ou Herói do Companheiro) do Turno**
4. **Cartas da Pilha de Descarte**
5. **Cartas do Mestre de Jogo**

Sendo que efeitos [<span class="keyword-activation">Auto</span>](/cards/effect.md) entram depois de efeitos [<span class="keyword-activation">Ativar</span>](/cards/effect.md) e antes de efeitos [<span class="keyword-activation">Permanente</span>](/cards/effect.md), seguindo a mesma ordem acima.

### Mudança de Estado Durante a Resolução do Efeito

#### Nos Requerimentos

Extraordinariamente, se um efeito era possível no momento da ativação da carta, mas um Encadeamento de Respostas ou outra situação de jogo fez com que os demais requerimentos de ativação do efeito fossem quebradas, a ativação do efeito é então parada, não sendo considerado que o efeito foi negado nem ativado, apenas que não é mais possível dar prosseguimento à jogada, quaisquer custos já pagos não são devolvidos.

#### Na Descrição

Extraordinariamente, se os requerimentos de um efeito já foram cumpridos e o efeito já está sendo resolvido, mas um Encadeamento de Respostas ou outra situação de jogo fez com que as condições descritas no texto do efeito fossem quebradas, o que já foi feito é mantido, mas a restante do efeito é ignorado. É considerado que o efeito foi ativado, e não negado, mas que não é mais possível dar prosseguimento à resolução do efeito.

---
