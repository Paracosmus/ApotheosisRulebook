---
label: Cartilha
layout: page
---

# Cartilha

---

### Durante seu Turno

Ativar Carta
:   Custo de {{ ap }}, {{ sp }}, {{ mp }}  e/ou Essência, mais requerimentos e custos adicionais descrito na carta, se houverem

Enviar carta do {{ inv }} para a {{ table }}
:   2 de {{ ap }}
<br>

Enviar carta da {{ table }} para a {{ inv }}
:   2 de {{ ap }}
<br>

Realizar um Teste
:   2 de {{ ap }}

Interação com Objeto ou Personagem
:   2 de {{ ap }}
*   Falar com personagem
*   Mover a peça de um Objeto para uma casa vazia adjacente a ela
*   Obter um {{ item }} de uma peça Container

Despertar o {{ entity }}
:   2 de {{ sp }} e/ou {{ mp }}
*   +2 de {{ sp }} e/ou {{ mp }} no início do turno para manter o {{ entity }} desperto

Evocar
:   2 de {{ mp }}

Descansar
:   Ação total para curar 10 de VIDA e recuperar 2 de ESTAMINA, MANA e/ou ESSÊNCIA

Trocar cartas com uma Pilha de Descarte
:   Ação total

Propor Pacto
:   Ação total (_de todos os envolvidos_)

<br>
<br>

### Apenas Fora de Batalha

Adquirir {{ class }}
:   Ação total e enterrar 5 cartas de recurso do mesmo nível da carta desejada

Progredir {{ class }}
:   Ação total e enterrar 3 cartas de recurso do mesmo nível da carta desejada

Incorporar {{ entity }}
:   Ação total e enterrar 5 cartas de recurso do mesmo nível do carta desejado

Liberar {{ entity }}
:   Ação total e enterrar o seu {{ entity }}

Fabricar {{ item }}
:   Ação total e enterrar cartas de {{ item }} até que a combinação dos materiais seja igual ou superior aos materiais da carta desejada

<br>

### Apenas Durante a Batalha

Mover (por casa do tabuleiro)
:   1 de {{ ap }}
*  +1 de {{ ap }} para cada inimigo adjacente para desengajar
*  +1 de {{ ap }} para cada ALTITUDE de diferença

Ataque Normal
:   3 de {{ ap }}

    | {.compact}
    | --- | --- |
    | {{ dmg }}    | {{ str }} + {{ d1d2 }} |
    | {{ direct }} | 1                      |

