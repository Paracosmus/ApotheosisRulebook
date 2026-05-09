---
label: Teste
icon: checkbox
order: 35
---

# Teste

{{ briefing `Check` `Um teste é uma ação realizada por um personagem para determinar se ele consegue ou não alcançar um determinado objetivo ou superar um desafio.` }}

Este é um dos elementos fundamentais deste sistema de RPG. Em termos de jogo, um teste é uma mecânica que envolve a rolagem de dados ou a comparação de valores para determinar o sucesso ou falha de uma ação específica. Os testes são usados para resolver situações em que o resultado não é garantido, como tentar abrir uma porta trancada, persuadir um NPC, ou resistir a um ataque.

Quando interpretando, o personagem não tem controle total sobre o resultado de suas ações, e os testes são uma forma de introduzir um elemento de incerteza e desafio. O resultado de um teste pode ser influenciado por diversos fatores, como as habilidades do personagem, as circunstâncias da situação, e a dificuldade da tarefa.

Desta forma, os jogadores não podem simplesmente declarar que seus personagens conseguem ou fizeram algo, sendo necessário realizar um teste para determinar o sucesso ou falha da ação.

---

## Realizando um Teste

Quando a narração da ação de um personagem, seja por parte dos jogadores ou por parte do Mestre, chegar a um ponto onde a mera declaração dos resultados daquela ação não forem suficientes, óbvios ou justos, é necessário realizar um teste.

Primariamente, cabe ao jogador descrever como o personagem sobre seu controle está realizando a ação. Dado a descrição fornecida, o jogador então diz qual será a forma que ele vai jogar este teste, ou seja, qual {{ knowledge}} e Atributo ele irá usar para realizar aquele teste e o Mestre arbitra se esta forma é apropriada ou não, tendo ele a palavra final sobre a forma do teste conforme a descrição, bem como fornecer opções de como realizar o teste ao jogador, se necessário.

Não cabe ao Mestre censurar ou orientar as ideias dos jogadores. Se o jogador decidir por uma forma que o mestre julgar mais complexa ou difícil, ele não deve impedir, e apenas ajustar a dificuldade. Sendo a jogada válida, o Mestre deve aceitar a forma escolhida pelo jogador, mesmo que seja diferente do que ele tinha em mente inicialmente.

Uma vez definida a forma do teste, o Mestre então decide qual a dificuldade lógica para aquele teste, com base nas informações privilegiadas que ele possui.

!!!secondary Exemplo
Para destrancar uma porta, o Mestre sabe qual a complexidade e qualidade da fechadura, o que pode influenciar na dificuldade do teste.

Para persuadir um NPC, o Mestre conhece a real personalidade e motivações do NPC, o que pode influenciar na dificuldade do teste.
!!!

É esperado que um jogador experiente e criativo saiba escolher o conhecimento para um teste, e que o Mestre seja flexível e aberto a essas escolhas, desde que façam sentido dentro da narrativa e do contexto do jogo.

Não existe forma "correta" ou "errada" de fazer um teste, a criatividade e a narrativa são os elementos mais importantes, e o sistema tem função apenas de emular e medir a ação narrada.

!!!secondary Exemplo
Um teste de _Corrida_ é geralmente realizado com ( {{ athletics }} + {{ agi }} ), enquanto um teste de _Persuasão_ geralmente é realizado com ( {{ cunning }} + {{ cha }} ), etc..

Porém, o jogador pode contra-argumentar que nesta situação ele está tentando "_convencer um NPC que é atleta, a não abandonar o esporte_", e portanto ele vai usar ( {{ athletics }} + {{ int }} ) para um teste de _Persuasão_, ao explicar que irá usar seus conhecimentos de {{ athletics }} combinado com lógica ({{ int }}) para apoiar sua tentativa de convencimento do NPC.

O Mestre então, julga a dificuldade do teste com base na forma. Ele pode decidir que para persuadir o alvo por mentiras e manipulações, o teste de _Persuasão_ tradicional é mais difícil, mas para persuadir o alvo por meio de argumentos lógicos sobre um tema que o NPC ama, o teste de _Persuasão_ alternativo é mais fácil, ou vice-versa, dependendo do contexto da situação.

Assim, um jogador experiente ou criativo consegue adaptar a forma de realizar uma ação para as capacidades de seu personagem, e um teste que tradicionalmente seria realizado com um conhecimento específico que talvez o seu personagem nem possua, pode ser realizado com outro conhecimento que ele domina, desde que o jogador consiga justificar sua escolha de forma coerente.
!!!

!!!
É comum que jogadores novos ou inexperientes tenham dúvidas sobre qual conhecimento escolher para um teste, e isso é esperado. O importante é que eles se sintam confortáveis em fazer uma escolha e que o Mestre e demais jogadores estejam dispostos a orientar e explicar as opções disponíveis. O Mestre pode sugerir uma forma específica com base na descrição da ação ou situação, mas deve sempre estar aberto a ouvir as sugestões dos jogadores e considerar suas ideias.
!!!

O teste é composto de **7** elementos, descritos na seguinte notação:

> _Nome_( {{ knowledge }} + **Atributo** + **Modificadores** + **Bônus** ➜ **Dificuldade** )
>
> O sétimo elemento é o dado rolado, mas ele não é expresso na notação do teste.
> ---
> * Ex. 1: _Escalar_( {{ athletics }} + {{ str }} ➜ **12** )
> * Ex. 2: _Caçar_( {{ practice }} + {{ per }} - {{ n '3'}} ➜ **16** )
> * Ex. 3: _Memória_( {{ int }} + {{ p '10'}} ➜ **20** )

==- Nome

  O nome do teste é uma descrição breve e clara da ação que o personagem está tentando realizar, e tem função apenas narrativa, não influenciando diretamente na mecânica do teste. O nome do teste deve ser escrito em itálico para diferenciá-lo de outros elementos do teste.

  O teste recebe um nome para facilitar a referência e a compreensão do que está sendo testado, tanto para os jogadores quanto para o Mestre. O nome do teste deve ser escolhido de forma a refletir a ação ou objetivo específico que o personagem está tentando alcançar, e deve ser claro o suficiente para que todos os participantes do jogo possam entender rapidamente do que se trata.

  Os nomes costumam ser breves e autoexplicativos, como _Destrancar_, _Persuasão_, _Resistir a Veneno_, _Levantar Peso_, etc., mas podem ser mais elaborados ou criativos, dependendo da situação e da preferência dos jogadores e do Mestre.

  !!!
  Observe que não existem proficiências ou perícias neste sistema, e o nome do teste não tem função mecânica, ou seja, não existe um teste de _Acrobacia_ ou um teste de _Furtividade_ que sejam realizados com um conhecimento específico, por exemplo.
  !!!

==- Conhecimento

  O {{ knowledge }} do teste é a base para determinar de qual área do conhecimento este teste faz parte.

  Como já explicado, não existe um {{ knowledge }} certo ou predeterminado para cada teste que possa surgir durante o jogo, mas existem alguns conhecimentos que são mais comumente associados a certos tipos de testes. Cabe ao jogador que controla o personagem dizer quando, como e de que forma ele irá realizar aquele teste, e isso inclui a escolha do conhecimento que ele acredita ser mais relevante para aquela situação, sendo que o Mestre tem a palavra final sobre a escolha.

  Se o personagem tem o {{ knowledge }} determinado para o teste, ele recebe um bônus no teste relacionado ao seu nível de {{ knowledge }}.

  {.striped}
  | Nível do {{ knowledge }} | Bônus |
  | --- | --- |
  | 0 | 0  |
  | 1 | 1  |
  | 2 | 5  |
  | 3 | 10 |

  > Para o nível **4** em diante, o bônus é de {{ p '+10' }} para cada nível adicional, ou seja, nível 4 = 20, nível 5 = 30, etc..

  !!!
  Em testes que envolvem o uso de cartas, como uma espada, ou uma magia, por padrão deve-se usar o conhecimento da carta (Livre, se não tiver). Porém, assim como em qualquer outro teste, o jogador pode advogar por uma forma diferente.
  !!!

  ##### Teste Sem Conhecimento

  Existem também os testes de conhecimento **Livre**, que são aqueles testes onde não é possível ou não faz sentido associar um conhecimento específico, e portanto o personagem não recebe nenhum bônus de conhecimento para realizar aquele teste.

  !!!secondary Exemplo
  _Resistir a Veneno_: um personagem inconsciente está resistindo a uma substância nociva em seu organismo. Seria um teste **Livre** de {{ enr }}, onde os demais bônus são aplicados, mas nenhum {{ knowledge }} é associado.
  !!!

==- Atributo

  Junto ao {{ knowledge }}, este elemento dá a forma ao teste, sendo escolhido com base na descrição fornecida pelo jogador que controla o personagem que realiza o teste.

  O Atributo escolhido para o teste deve ser aquele que melhor representa a capacidade ou característica do personagem que está sendo testada naquela situação específica. Assim como o {{ knowledge }}, o Atributo é escolhido pelo jogador, mas o Mestre tem a palavra final sobre a escolha, e pode sugerir ou exigir um Atributo específico com base na descrição da ação ou situação.

==- Modificadores

  São todos os [benefícios e penalidades](/gameplay/modifiers.md) provenientes de cartas afetando o teste.

  É comum que personagens tenham cartas e efeitos que forneçam bônus para certos tipos de testes, como bônus para testes de {{ arcane }}, ou bônus para testes de {{ per }}, etc., e esses bônus são modificadores para o teste.

==- Bônus

  São todos os [bônus](/gameplay/bonus.md) ou penalidades provenientes regras e de fatores externos, como o ambiente, a situação, as condições do personagem, etc.

  !!!secondary Exemplo
  Um personagem que cresceu em um ambiente montanhoso pode receber um bônus em um teste de "_encontrar uma caverna nas montanhas_".

  Um personagem que trabalhava como ferreiro pode receber um bônus em um teste de "_forjar uma arma_".

  Um personagem que está sob pressão ou estresse pode receber uma penalidade em um teste de "_concentração_".
  !!!

  Os bônus são separados da dificuldade do teste, pois eles representam fatores que influenciam o desempenho de um dos personagens tentando realizar o teste, enquanto a dificuldade representa o desafio ou obstáculo como um todo.

  Os bônus podem tornar um teste mais fácil ou mais difícil, mas não alteram a dificuldade em si para outros personagens.

  !!!secondary Exemplo
  Uma parede molhada aumenta a dificuldade de um teste de escalada para todos os personagens que tentarem escalá-la, portanto a dificuldade do teste de escalada para aquela parede é aumentada.

  Porém, se um dos personagens tentando escalar aquela parede estiver levando muito peso em equipamentos, enquanto outro está levando alguém nas costas, e um terceiro não está levando nada. Os bônus e penalidades individuais serão aplicados de acordo com a situação de cada personagem.
  !!!

==- Dado

  O teste é resolvido por meio de uma rolagem de [dados](/gameplay/die.md), onde o jogador rola um dado de 6 faces ({{ e1d6 }}) e soma o resultado ao total do {{ knowledge }}, Atributo, Modificadores e Bônus para obter o resultado final do teste.

  Se o teste for de um {{ knowledge }} que o personagem não possui, ele deve rolar {{ d1d3 }}.

  Na rolagem do dado do teste, leva-se em conta a regra de [rolagem perfeita](/gameplay/die.md#dados-extras-rolagem-perfeita).

  !!!
  Observe que dados adicionais providos por cartas ou outros efeitos são considerados Modificadores, e não são considerados dados do teste. Um efeito que modifique o dado do teste irá especificar isso claramente.
  !!!

==- Dificuldade

  A dificuldade do teste é o valor que o resultado final do teste deve alcançar ou superar para que o teste seja bem sucedido. A dificuldade é determinada pelo Mestre com base na descrição da ação ou situação, e pode ser influenciada por diversos fatores, como a complexidade da tarefa, as condições ambientais, a resistência do alvo, a forma escolhida pelo jogador, etc.

  A dificuldade é um elemento fundamental para determinar o nível de desafio de um teste, e deve ser escolhida de forma a refletir a dificuldade real da ação ou situação que está sendo testada. Dificuldades mais baixas indicam tarefas mais fáceis, enquanto dificuldades mais altas indicam tarefas mais difíceis.

  ##### Teste Oculto

  Em alguns casos, o Mestre pode optar por manter a dificuldade e/ou o nome de um teste ocultos dos jogadores, revelando-os apenas após a rolagem do teste, ou mesmo nunca revelando-os.

  Isso pode ser usado para criar suspense, surpresa ou incerteza em situações onde os jogadores não têm informações suficientes para avaliar a dificuldade da tarefa ou sequer se ela é possível, bem como quando o teste envolve um elemento secretos da narrativa ou descobertas.

  Uma verificação se algum personagem percebeu um objeto relevante, se lembrou ou notou algo, etc.. Também é útil quando não é possível para os personagens saberem se o teste escolhido realmente funcionaria, por exemplo, quando tentando tirar uma informação de um NPC e o Mestre não pode revelar se ele realmente sabe tem aquela informação, pois isso entregaria partes da narrativa.

  ##### Teste de Qualidade

  Em alguns casos, não faz sentido ou não é necessário estabelecer uma dificuldade para um teste, e portanto o teste é considerado como uma medida de competência. Nesses casos o valor obtido no teste é tratado como a **qualidade** da ação.

  !!!secondary Exemplo
  Um teste de _Construir Abrigo_ pode ser considerado um teste de qualidade, onde o resultado do teste determina a qualidade do abrigo construído, e não se o personagem conseguiu ou não construir o abrigo.
  !!!

===

---

## Sucesso e Falha

Um teste é considerado um sucesso quando o resultado final do teste é igual ou superior à dificuldade estabelecida para aquele teste.

Por outro lado, um teste é considerado uma falha quando o resultado final do teste é inferior à dificuldade estabelecida.

### Nível de Sucesso

Também conhecido como *"acerto crítico"*, um sucesso crítico é quando o resultado de um teste é tão alto que o personagem tem um sucesso extraordinário, superando as expectativas normais. Isso pode resultar em efeitos adicionais ou benefícios além do sucesso padrão.

Quando um personagem sucede em um teste, é considerado um *Sucesso de nível 0*. O que geralmente significa que o personagem conseguiu alcançar o objetivo ou superar o desafio, sem efeitos adicionais além do sucesso em si.

Daí em diante, para cada vez que o personagem supera a dificuldade em uma quantidade igual à dificuldade, o sucesso se torna mais impressionante, recebendo um nível adicional de sucesso, podendo resultar em efeitos adicionais ou benefícios além do sucesso padrão.

!!!secondary Exemplo
Se a dificuldade de um teste for **10**, um resultado de **10** ou mais seria considerado um <u>sucesso de nível 0</u>. Se o resultado for **20** ou mais, seria um <u>sucesso de nível 1</u>. Se o resultado for **30** ou mais, seria um <u>sucesso de nível 2</u>, e assim por diante.
!!!

Para cada nível adicional de sucesso, o personagem pode receber um benefício adicional, como um bônus em um teste subsequente ou uma vantagem narrativa. Cabe ao Mestre determinar quais benefícios adicionais são apropriados para cada nível de sucesso, com base na situação e na narrativa do jogo.

Excepcionalmente, testes muito fáceis (dificuldade 10 ou menos) não permitem níveis adicionais de sucesso, por serem considerados tarefas triviais, onde o sucesso é esperado e não há espaço para um sucesso extraordinário.

### Nível de Falha

Também conhecido como *"erro crítico"*, uma falha crítica é quando o resultado de um teste é tão baixo que o personagem falha de maneira catastrófica, resultando em consequências negativas significativas. Isso pode incluir danos adicionais, perda de recursos, ou outras penalidades graves.

Quando um personagem falha em um teste, é considerado uma *Falha de nível 0*. O que geralmente significa apenas que o personagem não conseguiu alcançar o objetivo ou superar o desafio, sem consequências adicionais além da falha em si.

Se o personagem obtiver um resultado inferior ou igual à metade da dificuldade, é uma *Falha de nível 1*. Daí em diante, para cada 5 pontos abaixo da metade da dificuldade, a falha crítica se torna ainda mais grave, recebendo mais um nível de falha, podendo resultar em consequências ainda mais severas.

!!!secondary Exemplo
Se a dificuldade de um teste for **24**, um resultado de **23** ou menos seria considerado uma <u>falha de nível 0</u>. Se o resultado for **12** ou menos, seria uma <u>falha de nível 1</u>. Se o resultado for **7** ou menos, seria uma <u>falha de nível 2</u>, e assim por diante.
!!!

### Repetição de Teste

Algumas situações podem levar o jogador a crer que ele tem a oportunidade de tentar realizar um teste mais de uma vez, seja para tentar melhorar o resultado, ou para tentar alcançar o sucesso após uma falha. **Isto é terminantemente proibido**, a menos que o Mestre explicitamente justifique o porquê da repetição ser permitida ou necessária naquele caso.

#### Repetição de Sucesso

Quando um personagem sucede em um teste, ele não precisa mais realizar aquele teste caso ele volte a acontecer. Por exemplo, se ele já foi bem sucedido em destrancar a porta de uma casa, ele não precisa mais realizar um teste para destrancar aquela mesma porta, se ele já foi bem sucedido escalando uma muralha, ele não precisa mais realizar um teste para escalar aquela mesma muralha.

Considera-se que o personagem já tem o conhecimento, experiência, confiança e habilidade para realizar aquela ação, e portanto não há necessidade de realizar o teste novamente.

#### Repetição de Falha

Quando um personagem falhar em um teste, aquele teste está bloqueado para ele. Falhar em um teste, significa que o personagem já tentou tudo que estava ao seu alcance para realizar aquela ação, não há mais nada que possa ser feito, e o próprio personagem está convencido disto, pois na primeira tentativa ele deu o seu melhor e percebeu que não sabe ou não consegue realizar a ação.

Se o personagem não conseguiu destrancar a porta de uma casa, ele não pode mais tentar destrancar aquela mesma porta, se ele falhou em tentar escalar uma muralha, ele não pode mais tentar escalar aquela mesma muralha.

#### Reteste

Sendo este um jogo de progressão de personagem, dado uma passagem de tempo de <u>pelo menos 1 dia</u>, combinado com uma <u>mudança na construção do personagem</u>, como mudança de {{ class }}, uma carta que possa ser advogada como bônus significativo, ou a aquisição de {{ knowledge }}, isso deve ser interpretado como uma mudança expressiva no personagem, permitindo uma nova tentativa.

---

## Testes em Série

Em algumas situações, a ação descrita pelo jogador pode envolver a realização de uma série de testes relacionados, onde o resultado de um teste pode influenciar ou determinar o próximo teste a ser realizado.

Nestes casos, o Mestre pode estabelecer uma série de testes, onde cada teste subsequente é condicionado ao resultado do teste anterior. O resultado de cada teste na sequência pode afetar a dificuldade, os modificadores, ou mesmo a forma do próximo teste. Falhar em um teste na sequência resulta em uma falha da ação inteira.

!!!secondary Exemplo 1
_O personagem quer extrair uma informação do taverneiro, porém o taverneiro desconfiado, não engaja na conversa com o personagem._
> _Iniciar Conversa_( {{ cha }} ➜ **10** )
> _Persuadir_( {{ cunning }} + {{ int }} ➜ **14** )

Neste caso, se falhar no primeiro teste, o personagem não consegue iniciar a conversa, e portanto não tem a oportunidade de realizar o teste de persuasão.

Porém, se obtiver um sucesso de nível 2 por exemplo, o taverneiro poderia ficar muito engajado e interessado na conversa, abaixando sua guarda com o personagem. Fornecendo assim um bônus para o personagem no próximo teste.
!!!

!!!secondary Exemplo 2
_O personagem quer escalar um muro e depois saltar do muro para o telhado de uma construção._
> _Escalar Muro_( {{ athletics }} + {{ str }} ➜ **14** )
> _Saltar para o Telhado_( {{ agi }} ➜ **10** )

Neste caso, se falhar no primeiro teste, o personagem não consegue escalar o muro, e portanto não tem a oportunidade de realizar o teste de salto para o telhado.

Porém, se obter um sucesso de nível 1 por exemplo, o personagem poderia escalar o muro verticalmente e horizontalmente obtendo uma posição ideal para saltar no telhado, diminuindo assim a dificuldade do segundo teste, que já havia sido estabelecida.
!!!

---

## Teste Composto

É comum que a ação ação descrita pelo jogador envolva uma ou mais ações que a lógica dita que requerem o uso de múltiplos conhecimentos.

Um teste composto é um teste que envolve a realização de múltiplos testes individuais, onde cada teste representa uma parte ou aspecto diferente da ação descrita pelo jogador. O resultado final do teste composto é determinado por meio da combinação dos resultados dos testes individuais, de acordo com as regras estabelecidas para o teste composto em questão.

Diferente de uma sequência de testes, onde cada teste subsequente é condicionado ao resultado do teste anterior e a falha em um teste pode impedir a realização dos testes subsequentes, em um teste composto todos os testes são realizados independentemente, e o resultado final é uma combinação dos resultados individuais.

!!!secondary Exemplo
_O personagem quer realizar um ataque de espada, onde ele precisa acertar uma das falhas na armadura do alvo e matá-lo._
> _Acertar Falha da Armadura_( {{ per }} ) + _Matar Alvo_( {{ str }} ) ➜ **28**

Neste caso, o estrago final causado é determinado por quão bem o personagem encaixou o golpe na falha da armadura, bem como pela força e habilidade do personagem ao tentar matar o alvo, sendo que o Mestre expos que 28 causaria a morte do alvo.
!!!

!!!secondary Exemplo
_O personagem quer correr de uma ponta a outra de uma corda bamba o mais rápido possível e sem cair._
> _Equilíbrio_( {{ agi }} ) + _Correr_( {{ athletics }} + {{ agi }} )

Neste caso, a velocidade de travessia é determinado pela composição do equilíbrio e velocidade do personagem.
!!!

---

## Teste em Conjunto

Um teste em que múltiplos personagens estão envolvidos, colaborando para alcançar um objetivo comum.

O resultado de um teste em conjunto é determinado por meio da comparação dos resultados individuais dos personagens envolvidos, ou pela soma dos resultados individuais, dependendo do contexto e da natureza do teste.

Cada jogador descreve e realiza o teste para seu personagem, individualmente, sendo que se possível dado a situação, cada envolvido pode fazer o teste da sua própria forma.

### Teste em Conjunto de Resultado Combinado

Em um teste combinado, os resultados individuais dos personagens envolvidos são somados para determinar o resultado final do teste. Este tipo de teste é comum em situações onde os personagens estão colaborando para alcançar um objetivo comum, como levantar um objeto pesado ou defender uma posição contra um ataque, de forma que a soma das ações conjuntas dos envolvidos adicionam integralmente para o objetivo final.

!!!secondary Exemplo 1
_Puxar Objeto_: vários personagens estão tentando puxar um objeto pesado, e o resultado final do teste é a soma dos resultados individuais de cada personagem, representando a força combinada dos personagens para puxar o objeto.
!!!

!!!secondary Exemplo 2
_Corrida de Revesamento_: vários personagens estão participando de uma corrida de revezamento, e o resultado final do teste é a soma dos resultados individuais de cada personagem, representando o tempo total da equipe para completar a corrida.
!!!

### Teste em Conjunto de Maior Resultado

Em um teste de maior resultado, o resultado final do teste é determinado pelo maior resultado individual entre os personagens envolvidos. Este tipo de teste é comum em situações onde o sucesso do teste depende do desempenho do melhor membro do grupo, como em uma competição ou desafio onde apenas o melhor desempenho é relevante para o resultado final.

### Teste em Conjunto de Menor Resultado

Em um teste do menor resultado, o resultado final do teste é determinado pelo menor resultado individual entre os personagens envolvidos. Este tipo de teste é comum em situações onde a ação ou objetivo depende do desempenho de todos os envolvidos, de forma que o sucesso do teste depende do desempenho do membro mais fraco do grupo.

!!!secondary Exemplo 1
_Velocidade de Viagem_: vários personagens estão viajando juntos tentando chegar a um destino o mais rápido possível. O personagem mais lento do grupo é quem dita o ritmo da viagem, já que o grupo não pode deixar ninguém para trás.
!!!

!!!secondary Exemplo 2
_Invasão Furtiva_: vários personagens estão tentando realizar uma invasão furtiva de um quartel. Se qualquer um dos personagens não for furtivo o suficiente, os guardas do local vão detectar o grupo so movendo pelo terreno.
!!!

---

## Competição

Em uma competição, os personagens envolvidos estão competindo entre si para alcançar um objetivo específico, e o resultado é determinado por meio da comparação dos resultados de testes realizados pelas partes envolvidas.

É comum em situações onde os personagens estão competindo por um recurso limitado, em uma corrida, um duelo, etc..

Sendo que uma competição pode envolver varias partes, seja essas partes personagens individuais ou grupos de personagens, usando o resultado do testes em conjunto para a comparação da competição.

Uma competição usa a seguinte notação:

> _Nome_( {{ knowledge }} + **Atributo** + **Modificadores** + **Bônus**  ✖  {{ knowledge }} + **Atributo** + **Modificadores** + **Bônus** )
> ---
> * Ex. 1: _Luta de Box_( {{ athletics }} + {{ str }} ✖ {{ athletics }} + {{ enr }} )
> * Ex. 2: _Acertar Pedrada_( {{ per }} ✖ {{ agi }} )

!!!secondary Exemplo 1 - Teste Simples
_Luta de Box_: dois personagens estão competindo em uma luta de boxe, e o resultado do teste de cada personagem é comparado para determinar quem venceu a luta, com base em quem teve o maior resultado. Pode se realizar um teste de competiçao por round se preferirem uma luta longa, onde em cada round os jogadores descrevem suas ações e estratégias para aquele round, determinando assim a forma do teste de cada round.
!!!

!!!secondary Exemplo 2 - Teste Composto
_Duelo_: dois personagens estão competindo em um duelo de saque de arma e tiro estilo velho oeste. É feito um teste de {{ agi }} para sacar a arma, e o personagem que tiver o maior resultado consegue sacar primeiro, e então tem a oportunidade de realizar um teste de {{ per }} para atirar no oponente, se ele não obtiver o mínimo determinado pelo mestre para acertar, o outro personagem então também tem a oportunidade de realizar um teste de {{ per }} para atirar.
!!!

!!!secondary Exemplo 3 - Teste em Conjunto
_Cabo de Guerra_: dois grupos de personagens estão participando de um cabo de guerra, o resultado do Teste em Conjunto de Valor Combinado de cada grupo é comparada para decidir qual grupo venceu a competição.

_Corrida de Revesamento_: vários grupos de personagens estão participando de uma corrida de revezamento, o resultado do Teste em Conjunto de Valor Combinado de cada grupo é comparada para decidir qual grupo venceu a corrida.
!!!

### Empate

Quando os competidores envolvidos obtêm o mesmo resultado, é considerado um empate. O que geralmente significa que nenhum dos competidores conseguiu superar o outro. O mestre deve avaliar a situação e decidir o que significa um empate.

!!!secondary Exemplo 1 - Os dois perdem
Em um _Duelo de Tiro_ pode significar que ambos foram baleados.
!!!

!!!secondary Exemplo 2 - Os dois empatam
Em um _Luta de Box_ pode significar que ninguém conseguiu acertar um golpe significativo.
!!!

---

## Recursos em Testes

Personagens podem adicionar cartas de recurso em testes, para melhorar as condições do teste, para receber bônus adicionais, para tentar garantir o sucesso do teste, ou para evitar a falha do teste.

Para isso, o jogador deve descartar uma quantidade de cartas de recurso do {{ inv }} do Herói, ou do anexo do {{ companion }}, podendo combinar diferentes recursos para um mesmo teste, sendo que cada tipo de recurso tem uma função diferente, e deve ser usado em um momento específico do teste, como descrito a seguir.

Se o recurso descartado for do mesmo {{ knowledge }} do teste (incluindo Livre), ele adiciona o dobro do se valor. Um recurso de ( {{ arcane }} ➜ **2** ) de valor igual a **5**, para um teste de {{ arcane }}, contaria como **10**.

Acompanhe o seguinte exemplo:

> _O personagem está tentando destrancar a porta de uma loja._
> _Destrancar_( {{ cunning }} + {{ agi }} ➜ **14** )

==- <span class="fill">{{ xp }}</span> [!badge Antes de realizar o teste]

  > O personagem vai usar as experiências vividas para superar o desafio do teste. Garantindo que, pelo conhecimento adquirido, ele sabe exatamente o que fazer para superar o desafio.

  Descarte um a quantidade de {{ xp }} maior ou igual a dificuldade do teste para garantir o sucesso do teste, não sendo mais necessário realizar a rolagem.

  !!!secondary Exemplo
  Se a dificuldade do teste for **14**, e o jogador descartar uma {{ skill }} de nível 2 e outra de nível 3, totalizando **15** de {{ xp }}, o teste é automaticamente bem sucedido, sem necessidade de rolar os dados.

  _O personagem já viu aquele modelo de fechadura antes, e sabe exatamente os macetes de como destrancá-la._
  !!!

==- <span class="fill">{{ fate }}</span> [!badge Antes de rolar os dados]

  > O personagem vai usar o destino, a sorte, o acaso ou a benção dos deuses para facilitar o teste.

  Descarte uma quantidade de {{ fate }} para diminuir a dificuldade do teste naquela quantidade.

  !!!secondary Exemplo
  Se a dificuldade do teste for **14**, e o jogador descartar {{ fate }} de valor **5**, a dificuldade do teste passa a ser **9**.

  _O personagem tem uma sorte incrível, ou os deuses estão do seu lado, logo que começa a testar as combinações ele percebe que uma falha na fabricação da fechadura vai facilitar o seu trabalho._
  !!!

==- <span class="fill">{{ will }}</span> [!badge Depois de rolar os dados]

  > O personagem vai usar sua força de vontade, determinação, coragem ou fanatismo para superar o desafio do teste.

  Descarte uma quantidade de {{ will }} para somar ao valor obtido na rolagem do teste naquela quantidade.

  !!!secondary Exemplo
  Se o resultado do teste for **12**, e o jogador descartar 3 cartas de {{ companion }} de nível 1, totalizando **3** de {{ will }}, o resultado final do teste passa a ser **15**.

  _O personagem emprega uma vontade enorme, muito esforço e determinação, motivado por um ideal, uma causa, um objetivo ou um medo, para abrir essa tranca._
  !!!

==- <span class="fill">{{ price }}</span> [!badge For falhar no teste]

  > Também chamado de _"comprar o teste"_, esta é uma última medida caso o personagem esteja prestes a falhar no teste, logo após rolar os dados e obter o resultado final, ele então, usando a filosofia de que "_dinheiro não resolve apenas se for pouco_", vai usar seus recursos financeiros para tentar comprar o sucesso do teste.

  Descarte uma quantidade de {{ price }} igual à dificuldade do teste ✱ 10.

  Esta é a única forma de uso de recurso em teste que <u>nem sempre está disponível</u>, já que depende do contexto da situação e da narrativa do jogo, e o Mestre tem a palavra final sobre quando esta opção está disponível ou não, valendo ao jogador advogar uma forma de _"comprar o teste"_.

  !!!secondary Exemplo 1 - Fechadura
  _Destrancar_: _o personagem não consegue destrancar a porta da loja, decidido, ele atravessa a rua e contrata um competente e discreto chaveiro que aceita o trabalho._
  !!!

  !!!secondary Exemplo 2
  _Obter Informação_: um personagem está tentando obter uma informação de um informante, mas o teste de persuasão falhou, e o informante se recusa a fornecer a informação. O personagem então suborna o informante, fazendo uma proposta financeira tão alta que é irrecusável.
  !!!

  !!!secondary Exemplo 3
  _Transportar Peso_: um personagem está tentando transportar um objeto pesado, mas o teste de força falhou, e ele não consegue levantar o objeto. O personagem então contrata um transeunte, pagando uma quantia exorbitante que faz aquele personagem parar tudo que está fazendo para ganhar aquele dinheiro.
  !!!

  !!!secondary Exemplo 4
  _Queda Livre_: um personagem está caindo de uma altura significativa. Ele tenta um teste de _Acrobacia_ para agarrar em um galho de árvore, mas falha, e ele não consegue se segurar. Os jogadores chegam a conclusão que não tem como pagar este teste, a lógica da situação não permite, e o personagem acaba caindo.
  !!!

  !!!
  Note que ao usar {{ price }} o teste não se torna um teste de _Negociação_, _Suborno_, _Corrupção_ ou semelhantes. Estes são testes tradicionais realizados da forma padrão para fazer acordos.

  Esta é uma mecânica de jogo que representa uma oferta final desesperada, onde o personagem está disposto a pagar um preço exorbitante para garantir o sucesso do teste, e não uma negociação normal onde o personagem tenta obter um preço justo.
  !!!

===

Uma vez usado um ou mais recursos em um teste, o narrador ou o jogador deve explicar de qual forma aquela utilização de recurso se encaixa na narrativa da ação, e como o personagem está usando aquele recurso para tentar superar o desafio do teste. O uso de recursos deve ser integrado à narrativa e não apenas uma mecânica de jogo, para que faça sentido dentro do contexto da situação.

Apenas o personagem que está realizando o teste pode usar recursos para aquele teste, isso inclui {{ companion }}, que <u>devem usar seus próprios anexos</u>.

---

## Advogar

O jogador pode advogar por um teste, o que significa que ele pode argumentar que um teste específico deve ser realizado para resolver uma situação, mesmo que as regras não especifiquem isso diretamente. O mestre tem a autoridade final para decidir se o teste é apropriado e como ele deve ser conduzido.

Advogar não só é permitido como é encorajado, pois promove a criatividade e a narrativa colaborativa entre os jogadores e o mestre. É claro que os jogadores devem entender a diferença entre advogar e discutir. O momento de advogar não é um momento para "fazer valer" a sua ideia de como as coisas deveriam ser, mas sim um momento para tentar convencer o mestre ao seu favor ou contra o oponente.

Isso inclui também, argumentar a favor de bônus positivos ou negativos em um teste, com base na narrativa ou nas circunstâncias do jogo, bem como com base nas cartas na sua mesa que poderiam influenciar na capacidade ou desempenho do personagem.

Uma vez que o argumento tenha sido apresentado, o mestre aceita ou rejeita a proposta no ato, determinando o bônus recebido, se houver, e a dificuldade do teste, se necessário, sendo esta a palavra final e não podendo ser contestada.

!!!secondary Exemplo 1 - {{ class }}
_O personagem está fazendo um teste para encontrar onde um livro está na biblioteca._

Ele advoga que ele tem a classe de _Bibliotecário_, e portanto tem um conhecimento especializado em encontrar livros, o que lhe dá um bônus no teste, e o mestre aceita o argumento, concedendo o bônus relacionado ao nível da classe.
!!!

!!!secondary Exemplo 2 - {{ item }}
_O personagem está fazendo um teste para escalar um paredão de pedras._

Ele advoga que ele tem a carta _Corda_, e portanto tem um item que pode ajudá-lo a escalar o paredão, o que lhe dá um bônus no teste, e o mestre aceita o argumento, concedendo um bônus específico para aquele item.
!!!

!!!secondary Exemplo 3 - {{ skill }}
_O personagem está tentando acender uma fogueira._

Ele advoga que ele tem a carta _Bola de Fogo_, e portanto o teste que seria de ( {{ practice }} + {{ str }} ) para acender a fogueira, pode ser realizado com ( {{ arcane }} + {{ spt }} ) para usar a magia de fogo para acender a fogueira, e o mestre aceita o argumento, permitindo que o teste seja realizado com {{ arcane }} ao invés de {{ practice }}, porém o jogador deve adicionalmente pagar custo de {{ mp }} relacionados à carta.
!!!

Qualquer carta na mesa de um personagem pode ser usada como argumento para obter bônus em um teste, cabe ao Mestre e jogadores estarem atentos a tais cartas.

---
