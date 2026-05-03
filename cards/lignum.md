---
label: Lignum
icon: git-branch-check
order: 10
---
{{ review() }}

# Lignum

É um conjunto de cartas de HABILIDADE interligadas. Você pode identificá-las pela presença do nome do LIGNUM antes do nome da carta, separados por um | (Barra Vertical).

Um espaço do {{ mem }} pode conter até 3 cartas de um mesmo LIGNUM. É possível ter cartas de LIGNUM diferentes no {{ mem }}, ocupando espaços diferentes, porém a soma de suas cartas de LIGNUM não pode ser superior a 9.

- {{ house }}: Sempre adicionam e/ou trabalham com o conhecimento do Lignum.
- {{ class }}: Fornecem espaços adicionais para cartas do Lignum igual ao nível da {{ class }}.
- {{ entity }}: Ao invés de serem mantidos consumindo Energia igual ao nível da carta na sua {{ startPhase }}, são mantidos consumindo 1 de Essência da cor do Lignum.
- {{ item }}: São consumidos depois de usados e não podem mais ser ativados quando consumidos. Possuem um efeito de {{ resetPhase }} para serem restaurados
- {{ skill }}: São o banco de energia do Lignum, estas são as cartas que possuem a Essência, a energia especial colorida do Lignum, usada por todas as cartas para ativar os efeitos.
- {{ companion }}: Para que as técnicas sejam usadas, os anexos precisam ser do mesmo nível e Lignum desta carta.
- {{ event }}: Uma vez por ciclo, quando estas cartas são descartadas, seja por qualquer mecânica ou efeito, você recupera uma quantidade de Essência da cor deste Lignum igual ao nível desta carta.

Todas estas situações são explicadas nos efeitos das cartas, não necessitando de memorização, mas é importante entender que cada tipo de naipe possui um tem uma função diferente dentro do Lignum, e que a interação entre elas é o que torna o Lignum um conjunto de cartas tão poderoso e versátil.

---

## Limite de Cartas

Cartas de Lignum não ocupam espaços na suas respectivas zonas na {{ table }}, mas são limitadas pelo nível do Herói. Cada Herói pode ter um número de cartas de Lignum igual ao seu nível.

Cada Herói pode ter apenas uma cópia de cada carta de um Lignum simultaneamente na sua {{ table }}.

!!!secondary Exemplo
Um Herói de nível **3** pode ter até **3** cartas de Lignum.

Se este Herói subir para o nível **4**, ele pode adicionar mais uma carta de Lignum, totalizando **4** cartas de Lignum.
!!!

---

## Essência

(TODO) Cada carta de LIGNUM possui uma essência, que é representada por uma cor. A essência de uma carta de LIGNUM é a mesma para todas as cartas do mesmo LIGNUM.

Essência é um recurso que pode também ser tratado como {{ sp }} e/ou {{ mp }}.

Quando você puder _“levantar troco”_, o troco deve ser da mesma cor ou levante {{ mp }} e/ou {{ sp }}.

{.list-icon}
* :icon-chevron-right: {{ yellow }} - Representa a essência de Lignums de natureza física, como força, resistência, objetos materiais, etc.

* :icon-chevron-right: {{ red }} - Representa a essência de Lignums de natureza expansionista, como poder, controle, dominação, atitude, etc.

* :icon-chevron-right: {{ blue }} - Representa a essência de Lignums de natureza intelectual, como conhecimento, sabedoria, estratégia, etc.

* :icon-chevron-right: {{ white }} - Representa a essência de Lignums de natureza espiritual, como fé, esperança, amor, magia branca, etc.

* :icon-chevron-right: {{ black }} - Representa a essência de Lignums de natureza destrutiva, como morte, dor, sofrimento, magia negra, etc.

Se você pagar essência em uma ativação que seja exclusiva de estamina ou mana, você ainda pode pegar o troco do overpay. Agora se a ativação requer ambas, estamina e mana, então você não pode pegar o troco desta ativação

---

## Auto-Referenciação

Cartas de Lignum podem se referenciar, ou seja, uma carta de Lignum pode ter um efeito que se aplica a outras cartas do mesmo Lignum. Por exemplo, uma carta de Lignum pode dizer:

> {{ permanent }} {{ req 'Enquanto esta carta estiver ativa' }} Todas as outras cartas de deste Lignum ganham +1 de dano.

Um efeito de carta de Lignum que se aplica a outras cartas do mesmo Lignum é chamado de efeito de apoio. Este efeitos nunca referenciam o Lignum pelo nome, mas sim por meio de auto-referenciação usando expressões como "outras cartas deste Lignum", "todas as cartas deste Lignum", "este Lignum", etc.

Quando a referência for inversa, ou seja, quando o efeito se aplica a outros Lignum, isso será indicado por expressões como "cartas de outros Lignums", "outros Lignums {{ blue }}", etc.. Isso significa que o efeito se aplica a cartas de Lignum diferentes do Lignum da carta que está causando o efeito.

Efeitos nunca se referenciam a cartas de Lignum pelo nome, portanto o nome de um Lignum nunca aparece no texto de um efeito.

---
