---
label: Campanha
icon: checklist
order: 80
---

# Campanha

{{ briefing `São histórias pré-definidas que guiam os jogadores através de uma série de missões e desafios utilizando as cartas e mecânicas do jogo.` }}

Envolvem uma narrativa contínua, onde os jogadores participam de uma série de aventuras interconectadas. Elas podem incluir missões, eventos e desafios que se desenrolam ao longo do tempo, permitindo que os jogadores desenvolvam seus personagens e explorem o mundo de forma mais profunda e imersiva.

São criadas e escritas previamente, traçando objetivos, narrativas, história, mundo, cronologia, e outros aspectos que compõem o cenário de jogo. As campanhas podem ser jogadas em sessões únicas ou em várias sessões, dependendo do tamanho.

---

## Criar Campanhas

Campanhas podem ser publicadas oficialmente pelos criadores do jogo ou empresas licenciadas, ou podem ser criadas por jogadores e mestres de jogo para uso em suas próprias sessões, ou para compartilhar ou comercializar livremente, sem a necessidade de licenciar ou pagar royalties aos criadores do jogo, desde que não haja violação de direitos autorais ou propriedade intelectual, e que sejam respeitadas as diretrizes de uso estabelecidas pelos criadores do jogo e pela legislação aplicável.

Portanto, ao escrever uma campanha, ela se torna propriedade intelectual e autoral do seu respectivo autor, bem como sendo ele o único responsável legal pelo seu conteúdo.

---

## Onde Acontece

Toda campanha tem um cenário específico onde a história se desenrola, que pode ser um mundo fictício, uma cidade, uma região ou qualquer outro ambiente imaginário. O cenário é descrito em detalhes, incluindo sua geografia, cultura, história e outros aspectos relevantes para a narrativa.

!!!
Consulte a seção [Região](/lore/world.md#região).
!!!

---

## Missões

É recomendado que toda campanha tenha um objetivo final claro, que pode ser alcançado através de uma série de missões ou etapas. Cada missão deve ter seus próprios objetivos, desafios e recompensas, contribuindo para o progresso da história ou desenvolvimento dos personagens.

---

## Efeitos de Campanha

Campanhas podem incluir efeitos especiais, como bônus ou penalidades para os personagens, mudanças no ambiente de jogo, ou outras mecânicas que afetam a jogabilidade. Esses efeitos podem ser temporários ou permanentes, e devem ser claramente definidos e comunicados aos jogadores quando foram ativados ou inativados, sendo que, não é necessário revelá-los antes do momento em que eles são ativados.

Os efeitos de campanha funcionam exatamente como qualquer outro efeito, seguindo as mesmas regras e mecânicas estabelecidas no jogo. Porém, eles não estão ligados a uma carta específica, e sim à campanha como um todo.

Durante a campanha, será determinado quando um efeito está ativo ou inativo. Quando ativos, eles são tratados de forma semelhante às cartas no {{ scenario }}, porém sem uma carta associada, e assim como no {{ scenario }}, os efeitos de campanha estão disponíveis e são aplicados à todos os personagens.

- Efeitos {{ activate }} podem ser ativados por qualquer personagem no seu turno ou quando as condições para sua ativação forem atendidas.
- Efeitos {{ auto }} são ativados automaticamente quando as condições para sua ativação forem atendidas.
- Quando um efeito for respondido de forma que resulte no descarte da carta ou semelhante, deve-se apenas ignorar esta parte.

!!!secondary Exemplo 1 - _Bônus de Ataque em Missão Específica_
Em uma campanha, pode haver um efeito de campanha que concede um bônus de +1 para todas as jogadas de ataque durante a missão "Invasão do Castelo". Esse efeito estaria ativo durante toda a missão, e todos os personagens se beneficiariam dele enquanto estiver ativo.
!!!

!!!secondary Exemplo 2 - _Uma Maldição Narrativa Convertida em Jogo_
Em uma campanha onde durante a noite uma maldição afeta todos os animais e eles ficam loucos e agressivos.

> {{ permanent }} {{ req 'Quando Noite, Meia-Noite, ou Madrugada' }} {{ creature }} infligem {{ p '+10' }} de {{ dmg }}.
!!!

!!!secondary Exemplo 3 - _Sistema de Sobrevivência_
Em uma campanha onde existem um sistema de fome, sede, e sono.

> {{ auto }} {{ resetPhase }} Adicione {{ n '1' }} **❂CONTADOR DE FOME**, {{ n '1' }} **❂CONTADOR DE SEDE** e {{ n '1' }} **❂CONTADOR DE SONO**, a sua {{ house }}.

> {{ permanent }} Você recebe bônus de {{ n '-1' }} em **Testes** e {{ dmg }} para cada **❂CONTADOR DE FOME**, **❂CONTADOR DE SEDE** e **❂CONTADOR DE SONO** na sua {{ house }}.

> {{ activate }} {{ req 'Quando um ' + cook + ' for ativado' }} Remova um **❂CONTADOR DE FOME** da sua {{ house }}.

> {{ activate }} {{ req 'Descarte uma **ÁGUA**' }} Remova um **❂CONTADOR DE SEDE** da sua {{ house }}.

> {{ activate }} {{ req 'Quando _Descansar_' }} Remova **3** **❂CONTADOR DE SONO** da sua {{ house }}.
!!!

Desta forma, é possível adicionar modularmente sistemas especiais para a campanha, baseados nas necessidades da narrativa e do cenário, sem a necessidade de criar cartas específicas para cada efeito, e sem a necessidade de criar regras ou mecânicas adicionais para lidar com esses efeitos, já que eles seguem as mesmas regras e mecânicas estabelecidas no jogo.

Por esta razão, o uso de efeitos de campanha é mais simples do que de [Mecânicas de Campanha](#mecânicas-de-campanha), que exigem a criação de regras e mecânicas adicionais para lidar com seus efeitos, e são mais complexas de implementar e equilibrar.

Se precisar escolher entre as duas, use efeitos de campanha sempre que possível, e reserve as Mecânicas de Campanha para situações onde os efeitos de campanha sejam limitados ou insuficientes para transmitir a narrativa, sensação ou funcionamento almejado.

---

## Mecânicas de Campanha

Mecânicas de campanha são regras ou modificações especiais que se aplicam a toda a campanha, e que afetam a jogabilidade de forma significativa. Elas podem incluir regras adicionais para os personagens, o cenário, ou outros aspectos do jogo, e geralmente são mais elaboradas e complexas do que os efeitos de campanha.

Quando uma campanha inclui mecânicas de campanha, elas devem ser claramente definidas e comunicadas aos jogadores antes do início da campanha, para que eles possam entender como elas afetam a jogabilidade e se preparar adequadamente.

O criador da campanha tem liberdade para criar e implementar as mecânicas de campanha que desejar, observando a compatibilidade com os formatos e variantes alvos dessa campanha. Apesar de poderem fazer modificações significativas na jogabilidade, observe que o objectivo não é criar um novo formato de jogo, apenas complementar o existente com uma necessidade narrativa ou temática desta campanha específica.

!!!secondary Exemplo - _Mecânica de Loucura_
1. Durante a campanha do gênero terror, os personagens podem ser afetados por uma condição de loucura, que representa o impacto psicológico das experiências traumáticas e estressantes que eles enfrentam durante a campanha. A condição de loucura é representada por uma barra horizontal para que representa a sanidade do time como um todo. A barra começa no valor 0 e pode variar de -5 (insano) a +5 (são).

1. O Mestre de jogo concede pontos positivos ou negativos aos personagens conforme se desenrolam os eventos da campanha, e o valor da barra é atualizado de acordo. Por exemplo, se os personagens enfrentarem uma situação traumática, o Mestre de jogo pode conceder pontos negativos à barra, indicando que o time está ficando mais insano. Por outro lado, se os personagens conseguirem superar um desafio difícil ou encontrar um momento de alívio cômico, o Mestre de jogo pode conceder pontos positivos à barra, indicando que o time está ficando mais são.

1. O valor da barra deve ser adicionado a todo teste realizado por membros do time.
!!!

Como observador no exemplo acima, as Mecânicas de Campanha são demasiadas elaboradas para serem representadas por efeitos de campanha sem que esses efeitos fossem excessivamente longos e detalhados, além de terem uma liberdade completa de modificar, remover e/ou adicionar regras. Em adicional, os efeitos jogam estritamente conforme as regras, não permitindo a intervenção ou gestão do Mestre de Jogo como no caso exemplificado.

---
