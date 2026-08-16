---
label: Modelo
icon: person-add
order: 40
---

# Modelo

{{ briefing `Dummy` `Se trata de uma peça no tabuleiro que não representa um personagem Herói, com ` + table + `, e nem um personagem ` + companion + `, com uma carta que o define` }}

São usado primariamente para representar personagens avulsos, sejam gerados por efeitos de carta ou pela campanha.

É comum que chefes de campanha (boss), sejam representados por Modelos que possam funcionar em suas próprias regras, permitindo ao chefe realizar ações e possuir habilidades sem a necessidade da construção de um personagem completo e complexo, dado que chefes são comumente extremamente poderosos e com suas próprias mecânicas únicas.

Outra forma comum, é para gerar personagens temporários ou voláteis gerados por efeitos de cartas, como por exemplo, o efeito de uma carta que gera um personagem aliado temporário, ou um personagem inimigo temporário.

---

## Estatísticas Adicionais

Um modelo possuí as seguintes estatísticas, em adicional às estatísticas presentes em todas as peças. Estes valores são definidos por sua carta, campanha ou método de geração, que por padrão funcionam da mesma forma que as estatísticas de outros personagens, mas podem ser modificadas por mecânicas próprias do Modelo:

- [Técnicas](/cards/technique.md)
- [Mecânicas próprias](#mecânicas-de-modelo)

---

## Técnicas de Modelo

Por não terem cartas que os representem, todas as habilidades, efeitos e capacidades de um Modelo são definidas por meio de técnicas, exatamente como feito em cartas de {{ companion }}.

Quando uma técnica de um Modelo for ativada, deve-se considerar o mesmo processo de ativação de uma técnica de {{ companion }}. Ou seja, trate como se estivesse ativando a técnica de uma carta de {{ companion }} contendo as mesmas propriedades que o Modelo.

Isso permite que respostas e reações sejam ativadas normalmente, e que o processo de ativação seja o mesmo. Por exemplo, uma carta que pode responder à ativação de uma técnica ou à ativação de uma carta de {{ companion }}, pode ser ativada normalmente em resposta à ativação de uma técnica de um Modelo.

Pelo fato de um modelo não ser, nem possuir uma carta de {{ companion }}, um efeito de resposta que causaria o descarte, ocultação, retorno ao {{ inv }}, etc., da carta não se aplica diretamente a um Modelo, neste caso, estes efeitos quando chegarem neste momento da resolução, não acontece nada nesta parte.

!!!
Extraordinariamente, quando um chefe de campanha é representado por um Modelo, o Mestre de Jogo pode manter cada técnica em segredo até que o chefe a utilize.
!!!

---

## Mecânicas de Modelo

Modelos podem possuir mecânicas próprias, que podem adicionar novas estatísticas ou modificar as já existentes, como por exemplo, uma mecânica onde o chefe possuí múltiplos turnos em uma rodada, ou uma mecânica onde seus pontos de {{ ap }} não são definidos por sua {{ agi }}, etc..

---

## Cartas Associadas

Um modelo não pode possuir cartas, pois ele não possui {{ table }}. No entanto, um modelo pode empregar efeitos iguais ou inspirados em cartas existentes.

!!!secondary Exemplo 1
  Um modelo que é um cavaleiro pode possuir um efeito parecido com o efeito da carta de {{ class }} "_Cavaleiro_".
!!!

!!!secondary Exemplo 2
  Um modelo que possui {{ skill }} e {{ item }} que existem cartas definidas para eles, pode possuir os mesmos efeitos dessas cartas.
!!!

!!!secondary Exemplo 3
  Um modelo de chefe de campanha que é um receptáculo de um {{ entity }} pode possuir o mesmo efeito daquela carta de {{ entity }}.

  > Quando um modelo for associado a um {{ entity }}, é também esperado que ele possua a propriedade **RECEPTÁCULO** por coerência. Essa propriedade é comum em {{ human }} cuja a temática seja um personagem com um {{ entity }} incorporado.
!!!

Quando um modelo é derrotado, mesmo não possuindo as cartas, o mestre pode descartar da sua mão ou de um baralho as cartas associadas àquele modelo e tornar os {{ item }} associados disponíveis para outros jogadores saquearem.

---
