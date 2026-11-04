---
label: Peça
icon: person
order: 90
---
{{ review() }}

# Peça

A batalha acontece em um tabuleiro quadriculado. O tabuleiro pode conter paredes ou casas com diferentes níveis de altura. Cada casa possui um tipo de [terreno](/battle/board.md#terreno).

- {{ hp }}
- {{ ap }}
- [Atributos](/gameplay/attributes.md)
- [Propriedades](/gameplay/tag.md)

---

## Criar uma Peça

Uma peça é criada com a {{ hp }} cheia, igual à sua {{ hp }} máxima. Isso acontece só quando a peça ainda não existe: uma peça que sai do tabuleiro e volta é a mesma peça, e mantém a {{ hp }} que tinha.

---

## Sair do Tabuleiro

Uma peça que sai do tabuleiro guarda o seu estado, como {{ hp }} e [marcadores](/gameplay/marker.md). Quando volta ao tabuleiro, ela volta exatamente como estava, exceto pelos pontos de {{ ap }} e pelo seu lugar na [ordem dos turnos](/battle/turn.md#entrar-e-sair-da-ordem-dos-turnos).

!!!
Isso impede, por exemplo, que um {{ companion }} seja retirado da {{ table }} e recrutado de novo para recuperar sua {{ hp }} ou se livrar de marcadores.
!!!

---

## Curar

Apenas personagens podem ser curados. Um objeto nunca é curado.

A cura nunca deixa a {{ hp }} de um personagem acima da sua {{ hp }} máxima.

---

# **Tipos**

## Personagem

É uma peça no tabuleiro com turno e ações controladas por um jogador

### Herói

### **Companheiro**

### **Dummy**

Personagem que não está ligado a um Herói ou COMPANHEIRO, criado pela campanha ou por efeitos de cartas; suas características são definidas pelo que o criou.

## **Objeto**

Não são personagens: não têm turno, não interagem, etc.

Destruído: São removidos do tabuleiro quando sua VIDA chega a 0 (destruídos)

Objetos não podem ser curados (reparados)

## **Container**

É um estado de uma peça que a torna um armazém de cartas. Os personagens podem interagir com ele quando estão a 1 de distância, pagando 2 de AÇÃO para obter uma carta armazenada nele.

As cartas armazenadas em um contêiner são [não jogáveis](/cards/index.md#estado-da-carta): nenhum de seus efeitos ou bônus é considerado.

Personagens mortos são contêineres dos quais outros jogadores podem obter suas cartas de item

Objetos podem ser definidos como contêineres por algum efeito ou mecânica

Quando um ITEM é dropado, é adicionada uma peça naquela casa do tabuleiro, que é um contêiner que permite obter os itens que foram dropados ali

Containers nunca bloqueiam trajetória de ataques, sendo considerados baixos demais para isso.
