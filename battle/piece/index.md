---
label: Peça
icon: person
order: 90
---
{{ review() }}

# Peça

A batalha acontece em um tabuleiro quadriculado de 11x11 casas. No tabuleiro, podem conter casas bloqueadas ou com diferentes níveis de altura. Cada casa possui um tipo de [terreno](/battle/board.md#terreno).

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

# **Tipos**

## Personagem

É uma peça no tabuleiro com turno e ações controladas por um jogador

### Herói

### **Companheiro**

### **Dummy**

Personagem que não está ligado a um Herói ou COMPANHEIRO, criados pela campanha ou efeitos de cartas, suas características são definidas pelo que o criou.

## **Objeto**

Não são personagens: Não tem turno, não interage, etc.

Destruído: São removidos do tabuleiro quando sua VIDA chega a 0 (destruído)

Objetos não podem ser curados (reparados)

## **Container**

É um estado de uma peça que torna ela um armazem de cartas. Os personagens podem interagir com eles quando a 1 de distância pagando 2 de  AÇÃO para obter uma carta armazenada neles.

As cartas armazenadas em um contêiner são [não jogáveis](/cards/index.md#estado-da-carta): nenhum de seus efeitos ou bônus é considerado.

Personagens mortos são containers que outros jogadores podem obter suas cartas de item

Objetos podem ser definidos como containers por algum efeito ou mecânica

Quando um ITEM é dropado, é adicionado uma peça naquela casa do tabuleiro que é um container que permite obter os itens que foram dropados alí

Containers nunca bloqueiam trajetória de ataques, sendo considerados baixos demais para isso.