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

É recomendado que toda campanha tenha um objetivo final claro, que pode ser alcançado através de uma série de missões ou etapas. Cada missão deve ter seus próprios objetivos, desafios e recompensas, contribuindo para o progresso da história e o desenvolvimento dos personagens.

---

## Efeitos de Campanha

Campanhas podem incluir efeitos especiais, como bônus ou penalidades para os personagens, mudanças no ambiente de jogo, ou outras mecânicas que afetam a jogabilidade. Esses efeitos podem ser temporários ou permanentes, e devem ser claramente definidos e comunicados aos jogadores quando foram ativados ou inativados, sendo que, não é necessário revelá-los antes do momento em que eles são ativados.

Os efeitos de campanha funcionam exatamente como qualquer outro efeito, seguindo as mesmas regras e mecânicas estabelecidas no jogo. Porém, eles não estão ligados a uma carta específica, e sim à campanha como um todo.

Durante a campanha, será determinado quando um efeito está ativo ou inativo. Quando ativos, eles são tratados de forma semelhante às cartas no {{ scenario }}, porém sem uma carta associada, e assim como no {{ scenario }}, os efeitos de campanha estão disponíveis e são aplicados à todos os personagens.

- Efeitos {{ activate }} podem ser ativados por qualquer personagem no seu turno ou quando as condições para sua ativação forem atendidas.
- Efeitos {{ auto }} são ativados automaticamente quando as condições para sua ativação forem atendidas.

!!!secondary Exemplo 1
Em uma campanha, pode haver um efeito de campanha que concede um bônus de +1 para todas as jogadas de ataque durante a missão "Invasão do Castelo". Esse efeito estaria ativo durante toda a missão, e todos os personagens se beneficiariam dele enquanto estiver ativo.
!!!

!!!secondary Exemplo 2
Em uma campanha onde durante a noite uma maldição afeta todos os animais e eles ficam loucos e agressivos.

> {{ permanent }} {{ req 'Quando Noite, Meia Noite, ou Madrugada' }} {{ creature }} causam {{ p '+10' }} de {{ dmg }}.
!!!

!!!secondary Exemplo 3
Em uma campanha onde existem mecânicas de fome, sede, e sono.

> {{ auto }} {{ resetPhase }} Adicione {{ n '1' }} **❂CONTADOR DE FOME**, {{ n '1' }} **❂CONTADOR DE SEDE** e {{ n '1' }} **❂CONTADOR DE SONO**, a sua {{ house }}.

> {{ permanent }} Você recebe bônus de {{ n '-1' }} em **Testes** e {{ dmg }} para cada **❂CONTADOR DE FOME**, **❂CONTADOR DE SEDE** e **❂CONTADOR DE SONO** na sua {{ house }}.

> {{ activate }} {{ req 'Descarte um **CONSUMÍVEL**' }} Remova um **❂CONTADOR DE FOME** da sua {{ house }}.

> {{ activate }} {{ req 'Descarte uma **ÁGUA**' }} Remova um **❂CONTADOR DE SEDE** da sua {{ house }}.

> {{ activate }} {{ req 'Quando _Descansar_' }} Remova **3** **❂CONTADOR DE SONO** da sua {{ house }}.
!!!

---
