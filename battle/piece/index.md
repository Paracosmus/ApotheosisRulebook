!!!danger
Esta seção ainda não foi completamente revisada. Algumas informações podem estar desatualizadas ou incompletas, e a formatação pode não estar finalizada.
!!!
    
# Peça

A batalha acontece em um tabuleiro quadriculado. O tabuleiro pode conter paredes ou casas com diferentes níveis de altura. Cada casa possui um tipo de [terreno](/battle/board.md#terreno).

- [<span class="hp"><b>VIDA</b></span>](/hero/#vida)
- [<span class="main"><b>AÇÃO</b></span>](/hero/#ação)
- [Atributos](/gameplay/attributes.md)
- [Propriedades](/gameplay/tag.md)

---

## Criar uma Peça

Uma peça é criada com a [<span class="hp"><b>VIDA</b></span>](/hero/#vida) cheia, igual à sua [<span class="hp"><b>VIDA</b></span>](/hero/#vida) máxima. Isso acontece só quando a peça ainda não existe: uma peça que sai do tabuleiro e volta é a mesma peça, e mantém a [<span class="hp"><b>VIDA</b></span>](/hero/#vida) que tinha.

---

## Sair do Tabuleiro

Uma peça que sai do tabuleiro guarda o seu estado, como [<span class="hp"><b>VIDA</b></span>](/hero/#vida) e [<span class="main"><b>MARCADOR</b></span>](/gameplay/marker.md). Quando volta ao tabuleiro, ela volta exatamente como estava, exceto pelo seu lugar na [fila de turnos](/battle/stint.md#entrar-e-sair-da-fila-de-turnos).

!!!
Isso impede, por exemplo, que um [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) seja retirado da [<span class="main"><b>MESA</b></span>](/hero/table/) e recrutado de novo para recuperar sua [<span class="hp"><b>VIDA</b></span>](/hero/#vida) ou se livrar de [<span class="main"><b>MARCADOR</b></span>](/gameplay/marker.md).
!!!

---

## Curar

Apenas personagens podem ser curados. Um objeto nunca é curado.

A cura nunca deixa a [<span class="hp"><b>VIDA</b></span>](/hero/#vida) de um personagem acima da sua [<span class="hp"><b>VIDA</b></span>](/hero/#vida) máxima.

---

# **Tipos**

## Personagem

É uma peça no tabuleiro com turno e ações controladas por um jogador

### Herói

### **Companheiro**

### **Dummy**

Personagem que não está ligado a um Herói ou [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md), criado pela campanha ou por efeitos; suas características são definidas pelo que o criou.

## **Objeto**

Não são personagens: não têm turno, não interagem, etc.

Destruído: São removidos do tabuleiro quando sua [<span class="hp"><b>VIDA</b></span>](/hero/#vida) chega a 0 (destruídos)

Objetos não podem ser curados (reparados)

## **Container**

É um estado de uma peça que a torna um armazém de cartas. Os personagens podem interagir com ele quando estão a 1 de distância, pagando 2 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) para obter uma carta armazenada nele.

As cartas armazenadas em um contêiner são [não jogáveis](/cards/index.md#estado-da-carta): nenhum de seus efeitos ou bônus é considerado.

Personagens mortos são contêineres dos quais outros jogadores podem obter suas cartas de [<span class="item"><b>ITEM</b></span>](/cards/item.md)

Objetos podem ser definidos como contêineres por algum efeito ou mecânica

Quando um [<span class="item"><b>ITEM</b></span>](/cards/item.md) é dropado, é adicionada uma peça naquela casa do tabuleiro, que é um contêiner que permite obter os [<span class="item"><b>ITEM</b></span>](/cards/item.md) que foram dropados ali

Containers nunca bloqueiam trajetória de ataques, sendo considerados baixos demais para isso.
