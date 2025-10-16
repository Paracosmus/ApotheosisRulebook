---
label: Peças
icon: squirrel
order: 3
---

# Peças

A batalha acontece em um tabuleiro quadriculado de 11x11 casas. No tabuleiro, podem conter casas bloqueadas ou com diferentes níveis de altura. Cada casa possui um tipo de terreno (grama, terra, água, lama, areia etc.).

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

Personagens mortos são containers que outros jogadores podem obter suas cartas de item

Objetos podem ser definidos como containers por algum efeito ou mecânica

Quando um ITEM é dropado, é adicionado uma peça naquela casa do tabuleiro que é um container que permite obter os itens que foram dropados alí

Containers nunca bloqueiam trajetória de ataques, sendo considerados baixos demais para isso.