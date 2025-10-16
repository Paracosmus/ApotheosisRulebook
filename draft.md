---
label: Rascunhos
icon: pencil
order: 0
---

# SEM SESSÃO

É preciso encontrar e definir uma sessão adequada para cada uma das regras a seguir.
Elas estão listadas aqui como rascunho ou lembrete de suas existências.

---

## Regras

* Apenas uma carta pode ser ativada em resposta a uma ação, e nenhuma outra carta pode ser ativada como resposta à resposta. Se múltiplos jogadores tentarem uma resposta a uma mesma ação, aquele que se manifestar primeiro recebe o direito de resposta. Entende-se por “resposta”, toda ativação de carta opcional que é encadeada em decorrência de uma outra ação. Cartas que podem ser ativadas como reposta opcional são chamadas de Reativas, e são as únicas cartas com capacidade de serem ativadas no turno de outros jogadores. Para identificar uma carta Reativa, basta analisar o seu texto, que deixará claro a situação em que esta carta pode ser ativada, comumente o texto terá uma forma semelhante a “Se você for selecionado como alvo...”, “Se uma habilidade for ativada...”, etc. Ex.: “Defender = Se um personagem em uma casa adjacente for selecionado como alvo de um ataque você se torna o alvo do ataque.”. Note que efeitos Reativos necessariamente precisam ser ativados, tornando-os opcionais, se um efeito passivo obrigatório iniciar em decorrência de uma ação, este ainda é um efeito passivo e, portanto, não é considerado como uma reposta à ação.

* Uma Ativação de Carta acontece quando um jogador declara a ação de utilizar o efeito de uma carta opcional, ou seja, uma carta cujo efeito não inicia de forma automática. No momento da ativação, todos os custos determinados pelos campos apropriados da carta, bem como pelo seu efeito, devem ser pagos, e só então os outros jogadores podem declarar uma resposta, se desejarem. Note que, cartas de efeito passivo obrigatório, tem seus efeitos executados automaticamente, portando nunca são “ativadas”, neste caso diz-se que o efeito iniciou ou executou. Uma carta não pode ser ativada se o personagem não puder pagar os seus custos de ativação ou cumprir os seus requerimentos de ativação, que vão desde os valores nos campos apropriados, como distância do alvo, ou no texto da carta, como filtros de seleção de alvo.

* Se um personagem fizer uma Reação após reservar seus pontos de {{ ap }}, ele perde essa reserva e começa o próximo turno com os pontos reservados recuperados, mas perde a ação.

* Por padrão, você pode acessar cartas dos baralhos durante a batalha, porém, todo tabuleiro de batalha é considerado como sendo um local de nível 0 em tudo. Existirão cartas capazes de trabalhar com isso.

* Todo evento é descartado após ser resolvido. Quando um evento é negado, ele ainda assim é descartado.

* Quando selecionando um alvo para um ataque, você pode selecionar tanto uma peça do tabuleiro (personagens, objetos), quanto uma casa do tabuleiro (tile). Porém, apenas peças sofrem dano e recebem efeitos de aplicação de marcadores, entre outros. Selecionar um tile como alvo é útil quando se quer aplicar efeitos como EXPLOSIVO.

* Quando um texto diz por exemplo “o personagem não pode ser alvo desta carta” significa aquela unidade/cópia da carta especificamente, agora quando diz algo como “o personagem não pode ser alvo desta Habilidade” quer dizer de qualquer carta daquele nome.

* Quando a carta diz por exemplo “3 de distância / 3 away” significa que deve ser calculado a distância normal, incluindo altura e outros obstáculos, mas não áreas de domínio. Quando diz apenas “a 3 Casas do tabuleiro / 3 tiles” ou “adjacente / adjacent” significa adjacência, ou seja, considera apenas a distância de adjacência das casas, sem considerar outros fatores como altura e obstáculos. Note que o movimento em ambos os casos precisa ser possível, ou seja, obstáculos serão considerados

* Tipos de Peças: O tabuleiro pode ter alguns tipos de peças diferentes. Duas peças nunca podem ocupar a mesma casa simultaneamente.
    * Personagens: são as peças animadas controladas pelos jogadores que representam personagens.
    * Objetos: São peças inanimadas, sem donos, que servem de decoração ou obstáculo, como portas, barreiras arcanas, paredes, destrutíveis, etc. Objetos possuem {{ hp }} e uma lista de testes e resultados: Por exemplo, uma porta pode ter o teste de destrancar para que ela não seja mais um obstáculo, e de arrombar para que ela seja removida do tabuleiro
    * Container: é uma peça no tabuleiro, que serve para armazenar cartas, geralmente ITENS, como por exemplo baús, prateleiras, armários, e até corpos de personagens caídos. Personagens em casas adjacentes podem acessados o conteúdo de um container ao custo de 2 de {{ ap }}. Isso permite que eles obtenham cartas do container, de quaisquer naipes, sem pagar o valor da carta. Containers não são obstáculos, e podem ser movidos por um personagem adjacente para uma outra casa adjacente vazia ao custo de 2 de {{ ap }}

* Obstáculos: É um estado de uma peça ou casa no tabuleiro onde outras peças não podem passar pela casa ocupada, bem como ataques de linha reta. Quando uma casa do tabuleiro é um obstáculo, não há nada que se possa fazer quanto a isso, aquele tile simplesmente não é interagível. Peças podem ser obstáculos quando por exemplo são personagens de outros times ou objetos inanimados como estátuas, portas, etc.

* Regra do Loot: Quando um Herói ou Companheiro morre, suas cartas são descartadas para suas respectivas pilhas de descarte conforme diz a regra, porém, quando o loot é permitido pelo modo de jogo, cartas de ITENS devem permanecer no corpo do personagem, que agora age como um container contendo aqueles ITENS.

* Quando a AGI crescem ou diminuem no mesmo turno o que você tem de PA não muda, nem para cima nem para baixo. O PA que você começa o turno é calculado antes de resolver os efeitos, mecânicas e resultados de "no início do seu turno". (sim, se você não pagar o Ente ou similar, você continua ganhando o PA que ele dá)

* Quando um Companheiro tem sua carta substituída, ao contrario de removida da mesa, a peça dele deve ser trocada para a peça da nova carta e ele herda também a quantidade atual de HP, mesmo quando completo.

* Numa substituição de carta, a carta nova herda os contadores e anexos da carta anterior.

* Quando {{ injury }} é causada a um personagem, o resultado depois de resolver quaisquer efeitos passivos e um efeito ativo se necessário, é que o personagem `perde {{ hp }}`. Note que, alguns efeitos, podem explicitar que o personagem `perde {{ hp }}` diretamente, e não causam {{ injury }}. Geralmente são efeitos relacionados a drenagem de vida, energia vital, ou similares. {{ Injury }} é um termo genérico que se refere a qualquer dano causado a um personagem, e não necessariamente a toda forma de perder {{ vida }}.

* Quando uma carta tem uma peça que a representa no tabuleiro, essa peça tem todas as características da carta em como aplica as regras relacionadas a ela, como por exemplo se for uma peça de companheiro, o seu HP é definido pelo seu nível e seus atributos são listados na carta. Se não houver definições nas regras ou na carta para características da peça, estas características são consideradas ausentes quando possível e igual a 1 quando não for possível, como por exemplo, o HP de um item no chão é 1/1 e seus atributos são todos 1. Cada carta, pode ter apenas uma peça que a representa no tabuleiro, portando se um efeito ou mecânica diz para criar uma peça para aquela carta, se já houver uma peça representando aquela carta, este efeito ou mecânica deve ser ignorado. Se a peça de uma carta for removida do tabuleiro, uma nova peça pode ser criada por estes efeitos ou mecânicas, por outro lado, se a peça for destruída, como é no caso de Perda Total, morte de uma evocação, destruição de um objeto, etc, a carta não pode mais ser representada no tabuleiro, e uma nova peça não pode ser criada para ela. Observe que, cartas como Barreira Arcana, não criam peças para a carta, mas sim peças de objetos ou barreiras no tabuleiro, não tendo uma carta que as representem.

* Para uma carta ter qualquer efeito e fazer qualquer coisa ela precisa estar revelada. Quando trocando cartas com uma pilha de descarte, a carta cai revelada na pilha de descarte, por isso o valor dela pode ser usada mesmo estando no seu inventário.

* Cartas de ficha por padrão estão sempre levantadas. Se por algum motivo uma carta de ficha estiver deitada, isso não muda nada. (Em casos especiais, como cartas de Collegium, sua regra especial de Summus explicita regras para quando este tipo de carta de ficha está deitada, mas isso é uma exceção e não a regra geral)

* Sempre que se diz "Descarte/enterre/bana/etc. uma carta", isso significa especificamente uma carta de Recursos, a não ser que aquele efeito explicite o contrário.

* Quando uma combinação de efeitos e/ou mecânicas causar um loop infinito, o loop deve ser interrompido imediatamente assim que percebido e todas as cartas envolvidas devem ser banidas e nenhuma carta pode ser ativado em decorrência desse banimento. Se ficar claro que um dos jogadores causou o looping infinito propositalmente, ele perde a partida.

* Muitos efeitos não mencionam quando um personagem é selecionado como alvo. Note que, se um personagem, carta, etc. é alvo de um ação, significa que ele foi selecionado, mesmo que a carta não diga isso explicitamente. Por exemplo, "Reviva um personagem no tabuleiro", esse efeito claramente selecionou um personagem para reviver. Quando alguém é selecionado para uma ação, ele é chamado de "Alvo" e quem realiza a ação é chamado de "Agente".

* Quando for buscar uma carta em um baralho, pilha de descarte, ou similar, se o efeito ou mecânica não explicitar que a carta deve ser revelada, se for apenas pegar uma carta, ela é obtida oculta, porém se o efeito especificar uma característica da carta, como por exemplo "buscar uma carta de Item", ou "buscar uma carta de custo 3 ou menos", a carta deve ser revelada para que se possa verificar se ela cumpre os requisitos.

* Quando uma carta diz para pagar um custo, obviamente você só pode pagar com o que você tem disponível. No caso de VIDA por exemplo, você não pode remover pontos de vida que deixem o personagem com a vida negativa.

* Um ataque é quando um personagem realiza um "Ataque Normal" ou ativa uma carta de ITEM ou SKILL que possua DANO na sua barra de ativação. Note que ações em área que possuem dano, são ataques, mas não selecionam alvos. Efeitos como os de explosivos, que aplicam o dano da carta nos tiles adjacentes, também são considerados ataques nos adjacentes, já que o dano da barra de ativação é aplicado nos tiles adjacentes, porém, também não seleciona os tiles adjacentes como alvo.

* Observe que cartas com tasks como "descartar", "enterrar", "enviar para o cenário", "On Discard", "on Banish", etc. São resolvidas e depois enviadas para o destino, portanto, efeitos relacionados ou ativados por estas ações, devem ser resolvidos depois de resolver a carta em sí. Por exemplo, se uma carta diz "Quando esta carta for descartada, cause 2 de dano a um personagem", o efeito de causar dano deve ser resolvido antes de colcoar a carta na pilha de descarte, e só então, um efeito que verifique a pilha de descarte é ativado.

* Não existe chain link, cada ação pode ter apenas uma reação. Quando um efeito de carta, ou qualquer ação de jogo e realizado, apenas uma outra carta pode ser ativada em resposta a esta ação. Se múltiplos jogadores anunciarem uma resposta a uma mesma ação juntos ou mais ou menos ao mesmo tempo, a prioridade é [ personagem do turno -> oponentes -> parceiros ], se ambos tiverem a mesma prioridade, aquele que se manifestar primeiro recebe o direito de resposta, sendo que jogada anunciada não pode ser cancelada, portanto ele não pode ceder o lugar para outro jogador realizar a resposta. Entende-se por “resposta”, toda ativação de carta opcional que é encadeada em decorrência de uma outra ação. Cartas que podem ser ativadas como reposta opcional são chamadas de Reativas. Para identificar uma carta Reativa, basta analisar o seu texto, que deixará claro a situação em que esta carta pode ser ativada, comumente o texto terá uma forma semelhante a “Se você for selecionado como alvo...”, “Se uma habilidade for ativada...”, etc. Ex.: “Defender = Se um personagem em uma casa adjacente for selecionado como alvo de um ataque você se torna o alvo do ataque.”. Note que efeitos Reativos necessariamente precisam ser ativados, tornando-os opcionais, **se um efeito passivo obrigatório iniciar em decorrência de uma ação, este ainda é um efeito temp, permanent ou auto, e, portanto, NÃO é considerado como uma reposta à ação**.
    * _Call stack_: Quando vários efeitos de cartas começam a agir juntos, como a resposta e todos os efeitos autos engatilhados, nesse casa a ordem de resolução é:
        1. Efeitos Temp/Permanent
        2. Efeitos Auto
        3. Resposta
        4. Ação original
    * Dentro de um mesmo tier, considere que todas as cartas estão agindo ao mesmo tempo, se não for possível use a ordem [ personagem do turno -> oponentes -> parceiros -> demais personagens ]. Em último caso, desempate pela ordem de em que estão na mesa seguindo de cima para baixo da esquerda para direita (ficha primeiro). [essa é a ordem que o código vai usar]
    * _Exemplo_: Personagem A ataca o Personagem B, que tem a carta "Defender" (Reativa) e o Personagem C tem a carta "Counterattack" (Auto). A ordem de resolução será: 1. Efeitos Temp/Permanent (se houver), 2. Efeito Auto do Personagem C (Counterattack), 3. Efeito Reativo do Personagem B (Defender), 4. Ação original (Ataque do Personagem A).

* Lembre-se que uma carta attachada não está nem revelada nem ativa, mesmo quando tem um efeito attachment. O estado de uma carta anexada, é, "anexada", ela não pode ser virada, desvirada, ocultada, revelada, etc.

* Todo once per turn em Apotheosis, é um hard once per turn, ou seja, apenas uma cópia desta carta pode ser ativada, o mesmo vale para once per battle, etc.

* Rotação foi removido e a área do domínio são as 4 casas adjacentes, sendo que não se considera diagonal em nenhum caso no Apoteose, ou seja, o domínio é sempre uma cruz. A área de domínio são essas 4 casas adjacentes a certos tipos de peças no tabuleiro, sendo os personagens a mais comum, mas podendo existir em armadilhas, mecanismos, etc.. Para quê serve: Quando um personagem está na área de domínio de outro, para se mover para fora da casa, ele precisa pagar 1 de {{ ap }} extra, ou seja, se mover para fora da área de domínio custa 2 de {{ ap }}. Essa mudança tem como intuito descomplicar a vida dos personagens que fazem ataques melee, já que antes era muito custoso conseguir correr atrás de um inimigo e ainda ter PAs para atacar, dando muitas desvantagens em relação a ataques ranged, fazendo builds de melee não valerem a pena, ao mesmo tempo que mantem a dificuldade para contornar e flanquear, além disso, faz mais sentido lógico, já que não é um problema engajar em combato com alguém no campo de batalha, e sim, desengajar. Em adicional quando a área de domínio de dois personagens do mesmo time se sobrepõe, o custo para personagens de outro time saírem dalí deve stakar, no caso custa +2, +3, etc.

* **Usar Cartas e mesas de outrem**: Para todos os efeitos e para descomplicar, não existirá mais diferença entre "usar carta de outros" e "ativar cartas de outros", existirá apenas "ativar cartas de outros"
    * _Usar Carta de outro Herói como se fosse sua_
        * Você pode ativar a carta (auto, activate). Quem ativa é responsável por cumprir os requerimentos e pagar os custos.
        * Não recebe PERMANENT ou TEMPORARY effects da carta.
        * Você não pode vender, mudar de local, etc..
    * _Usar Mesa de outro Herói como se fosse sua_
        * Você pode ativar qualquer carta (auto, activate), quem ativa é responsável por cumprir os requerimentos e pagar os custos.
        * Você não recebe PERMANENT ou TEMPORARY effects das cartas
        * Se o efeito disser que você "pode" usar a mesa de outro Herói, significa que a partir do momento que você decide usar a mesa dele para uma determinada ação, você só pode usar cartas da mesa dele para aquela ação, ou seja, você não pode misturar cartas da sua mesa com cartas da mesa do outro Herói na mesma ação, portanto, use até mesmo os status como atributos e bônus passivos daquele herói durante aquela ação. O caso mais claro é (Inconsiente coletivo: onde o seu personagem joga com os status de outro personagem naquele momento)
    * Note que, quem ativa também é considerado o Herói da carta, ou seja, se ativa um item com DMG FOR+1D6, considere a força de quem ativou, se o efeito diz algo como, "você ganha +1 de HP", quem ativou ganha +1 de HP, etc.

---
