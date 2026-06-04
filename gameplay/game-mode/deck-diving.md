---
label: Deck Diving
icon: inbox-fill
order: 9
---

# Deck Diving

{{ briefing `Deck Diving` `É o modo de jogo onde os Heróis exploram baralhos em busca de cartas especiais, segredos e estratégias para avançar na aventura ou cumprir um objetivo.` }}

!!!warning
Este modo de jogo requer um narrador humano para criar e conduzir a exploração dos baralhos, proporcionando uma experiência personalizada e dinâmica para cada carta.
!!!

Neste modo, o narrador cria um conjunto de baralhos temáticos, cada um representando um ambiente, desafio ou tema específico. Cada Herói escolhe um baralho para explorar e, a cada turno, revela uma carta do topo do baralho. As cartas podem conter inimigos, armadilhas, tesouros, eventos ou segredos que os Heróis devem enfrentar ou aproveitar.

Cada objetivo tem um nível de dificuldade, que é usado para calcular os testes necessários para superar os desafios apresentados pelas cartas sem contexto, aquelas cartas que não disparam nenhuma parte narrativa.

Quando a carta do topo do baralho é revelada, o narrador descreve a cena e os desafios associados à carta usando o contexto que aquele baralho representa. Os Heróis então decidem como reagir à situação, utilizando suas habilidades, equipamentos e estratégias para superar os obstáculos apresentados pela carta.

| Naipe           | Narrativa | {.striped .compact}
| --------------- | --------- |
| {{ house }}     | Uma missão ou objetivo extra pode ser encontrado ou cumprido neste local. |
| {{ class }}     | O time tem que enfrentar um time de Heróis e/ou Dummies que representam a ideia daquela classe. |
| {{ entity }}    | Existe um Ente preso neste local que pode ser libertado ou derrotado. |
| {{ item }}      | Um item pode ser encontrado ou resgatado neste local. |
| {{ skill }}     | Uma habilidade pode ser aprendida ou utilizada neste local. |
| {{ companion }} | Um companheiro pode ser encontrado, enfrentado ou recrutado neste local. |
| {{ event }}     | Um evento pode ocorrer neste local, afetando os Heróis ou o ambiente de maneiras diversas seja de forma idêntica ao texto da carta ou customizado para o local. |

O objetivo é avançar na exploração do baralho, até que o objetivo estabelecido para quele baralho seja cumprido ou o baralho acabe.

Quando uma carta sem contexto é revelada
* Se for uma carta de ficha ela é descartada sem efeito
* Se for uma carta de recurso, é realizado um teste do ( {{ knowledge }} + {{ enr }} ➜ Dificuldade do Objetivo ✖ **10** ) para tentar obter a carta, se falhar, a carta é descartada sem efeito.

---

## Ciclo de Jogo

>>> Apresentação do Local ou Situação

  O narrador apresenta o tema geral do local ou situação representada pelo conjunto de baralhos, deixando claro o objetivo. Ele pode descrever o ambiente, os desafios e as possíveis recompensas que os Heróis podem encontrar ao explorar o baralho.

  São revelados os efeitos de objetivo, se houverem.

  ##### Wildcards

  São apresentadas as regras de wildcards, se houverem.

  A wildcard é uma carta que quando encontrada no baralho ativa uma situação específica. Narrador deve listar as wildcards para os jogadores, mas ele pode escolher não revelar o que cada wildcard representa, deixando um elemento de surpresa para os jogadores quando encontrarem uma wildcard durante a exploração do baralho.

  !!!secondary Exemplo

  _Os jogadores chegam às ruínas do Templo Esquecido, um local antigo e misterioso cheio de segredos e perigos. O objetivo é encontrar a Lira Flutuante (Carta de Item), um artefato lendário que se diz ter o poder de controlar as emoções e os elementos da natureza. Os baralhos representam diferentes áreas do templo._

  > **Efeitos de objetivo**: {{ permanent }} Todo {{ fate }} descartado em testes vale o dobro.

  !!!


>>> Apresentação das Partes do Local ou Situação

  O narrador apresenta as partes do local ou situação representada por cada baralho, explicando o que cada baralho representa e quais tipos de desafios ou recompensas os Heróis podem encontrar ao explorar cada um.

  São revelados os efeitos de baralho, se houverem.

  O baralho é então disposto em uma determinada ordem ou embaralhado aleatoriamente, dependendo da preferência do narrador ou das instruções do criador da campanha.

  !!!secondary Exemplo

  +++ Salão Principal
  _O Salão Principal é o coração do templo, onde os Heróis enfrentam os desafios iniciais e encontram pistas sobre a localização da Lira Flutuante._

  - 10x Inimigos Lv 1
  - 5x Item
  - 2x Eventos
  - 1x Wildcard (A carta Inercia representa a chegada à Câmara dos Guardiões)

  +++ Jardim Submerso
  _O Jardim Submerso é uma área alagada do templo, cheia de plantas aquáticas e criaturas perigosas. Os Heróis precisam nadar e mergulhar por esse ambiente traiçoeiro para encontrar a chave que abre a Câmara dos Guardiões._

  - 8x Inimigos Lv 2
  - 4x Item
  - 3x Habilidades com ÁGUA
  - 1x Wildcard (Chave da Câmara dos Guardiões)

  > **Efeitos de baralho**: {{ activate }} {{ allIn }} Realize um teste de Mergulho( {{ athletics }} + {{ enr }} ➜ **24** ). Se bem sucedido, o jogador pode buscar uma **wildcard** neste baralho e obtê-la. Se falhar, o Herói sofre {{ n'10' }} de {{ dmg }}.

  +++ Câmara dos Guardiões
  _Essa câmara é protegida por guardiões antigos e cheia de armadilhas mortais. Para chegar nela é preciso passar pelo Salão Principal levando a chave que está perdida no fundo do Jardim Submerso._

  - 1x Dummy (Boss fight)
  - 1x Habilidade
  - 3x Eventos Lv3 com ENCONTRO
  - 1x Wildcard (Lira Flutuante, o objetivo da missão) (colocada como a última carta do baralho)

  +++

  !!!


>>> Alocação dos Heróis

  Cada Herói escolhe qual baralho explorar, alocando-se em um dos baralhos apresentados, por padrão, não há limite de Heróis por baralho, porém efeitos de baralho podem impor restrições. Eles podem discutir entre si para decidir qual baralho é mais vantajoso ou interessante para explorar, levando em consideração suas habilidades, equipamentos e estratégias.

  Alguns objetivos podem exigir diferentes estratégias ou abordagens. Por exemplo:
  - Todos os baralhos devem ser finalizados
  - Cada baralho tem um objetivo específico
  - O objetivo da missão está em um dos baralhos e precisa ser encontrado
  - Existe um contador de tempo ou recursos que limita a quantidade de cartas que podem ser exploradas antes de cumprir o objetivo
  - Entre outros

  !!!secondary Exemplo
  _Os Heróis discutem e decidem que o Herói com habilidades de combate e resistência deve explorar o Salão Principal para enfrentar os inimigos iniciais, enquanto o Herói com habilidades de natação e mergulho deve explorar o Jardim Submerso para encontrar a chave_
  !!!

>>> Exploração

  Revelação da carta do topo do baralho, descrição da cena e dos desafios associados à carta, e decisão dos Heróis sobre como reagir à situação.

  Cada Herói, em seu respectivo turno, revela a carta do topo do baralho que está explorando. O narrador então descreve a cena e os desafios associados à carta usando o contexto que aquele baralho representa.

  !!!secondary Exemplo 1 - Combate
  _O Herói que explora o Salão Principal revela a primeira carta, que é um inimigo Lv 1. Tem início um combate entre o Herói e a carta de {{ companion }} que representa o inimigo._
  !!!

  !!!secondary Exemplo 2 - Evento
  _O Herói que explora o Jardim Submerso revela a primeira carta, que é um evento "Tempestade". O narrador decide por ativar a carta normalmente e descreve que uma tempestade repentina começa a se formar, tornando a água turbulenta e dificultando a natação, fazendo com que tentar mergulhar seja mais desafiador enquanto esta carta estiver no {{ scenario }}._
  !!!

>>> Resolução

  Os Heróis utilizam suas habilidades, equipamentos e estratégias para superar os obstáculos apresentados pela carta. O narrador determina o resultado da ação dos Heróis com base nas regras do jogo e na situação apresentada pela carta.

  A resolução de uma carta pode requerer testes de habilidade, combate, uso de recursos ou outras ações específicas, dependendo do tipo de carta e da situação apresentada. Por exemplo:
  - Combater um inimigo revelado pela carta
  - Encontrar um item representado pela carta
  - Resolver um evento ou enigma apresentado pela carta
  - Entre outros

  ||| Sucesso
  Se bem sucedida, a carta é obtida pelo Herói.
  ||| Falha
  Se falhar a carta é descartada e o Herói pode sofrer consequências, como perder recursos, receber dano ou enfrentar desafios adicionais.
  |||

  **Se a carta for uma wildcard**, o narrador ativa a situação específica associada àquela wildcard seja para sucesso ou falha.

  !!!secondary Exemplo 1 - Sucesso
  _O Herói que explora o Salão Principal enfrentou o inimigo e venceu. A carta de {{ companion }} é obtida pelo Herói, e ele avança para a próxima carta do baralho._
  !!!

  !!!secondary Exemplo 2 - Falha
  _O Herói que explora o Jardim Submerso tentou nadar através da tempestade, mas falhou no teste de Mergulho. Ele sofre {{ n'10' }} de {{ dmg }} e a carta de evento "Tempestade" **NÃO** é descartada, pois já foi enviada do topo deste baralho para o {{ scenario }}, e seu efeito continua ativo até que seja resolvido ou removido por outros meios. O Herói então pode tentar a próxima carta do baralho._
  !!!

>>> Conclusão

  O ciclo de exploração continua até que o objetivo do baralho seja cumprido ou o baralho acabe.

  Quando um baralho que ainda contem cartas é finalizado, o narrador pode escolher enviar as cartas restantes para a mão do mestre, ou descartá-las, dependendo da situação e do que fizer mais sentido para a narrativa.

  !!!secondary Exemplo 1 - Salão Principal
  _O Herói que explora o Salão Principal continua enfrentando os inimigos e avançando pelas cartas do baralho, até que finalmente encontra a wildcard "Inércia", que representa a chegada à Câmara dos Guardiões. Todas as cartas restantes neste baralho são então envidas para a mão do mestre. Agora com um caminho limpo e reconhecido, o Herói pode voltar para ajudar o seu companheiro no baralho (local) do lado._
  !!!

  !!!secondary Exemplo 2 - Jardim Submerso
  _O Herói que explora o Jardim Submerso continua enfrentando os desafios e avançando pelas cartas do baralho, o seu amigo se junto a ele e juntos eles finalmente encontram a wildcard "Chave da Câmara dos Guardiões". Ele obtém a chave juntos eles cruzam o salão principal, já concluído até o novo baralho adicionado à area do jogo... a Câmara dos Guardiões._
  !!!

  !!!secondary Exemplo 3 - Câmara dos Guardiões
  _Os Heróis enfrentam os desafios finais da Câmara dos Guardiões, incluindo o boss fight contra o Dummy, e finalmente encontram a wildcard "Lira Flutuante", cumprindo o objetivo da missão. Com a Lira Flutuante em mãos, o modo Deck Diving termina._
  !!!

>>>

---

## Dicas para o Narrador

!!-tip Dica para determinar o tempo de exploração
Uma boa fórmula para calcular o tempo em rodadas que os Heróis podem passar explorando um objetivo seria:

$$
\left( \frac{\text{Número de Cartas Total do Objetivo}}{\text{Número de Heróis Participantes}} \times \text{Constante de Controle} \right)
$$

Onde a constante de controle seria um número geralmente entre 1 e 2 que ajusta o tempo de exploração, dependendo do ritmo desejado para a aventura. Por exemplo, uma constante de controle de 1,2 pode ser usada para criar um ritmo mais desafiador e tenso, enquanto uma constante de controle de 1,8 pode ser usada para um ritmo mais relaxado e exploratório.

Exemplo: Se um objetivo tem um total de 40 cartas (2 baralhos de 20 cartas cada) e há 3 Heróis participando, usando uma constante de controle de 1,2, o cálculo seria:

$$
\left( \frac{40}{3} \times 1.2 \right) = \left( 13.333... \times 1.2 \right) = 16 \text{ rodadas}
$$
!!!

---
