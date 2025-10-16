---
label: Cartilha
layout: page
---

# Cartilha

---

### Durante seu Turno

Ativar Carta
:   Custo de {{ ap }}, {{ sp }} e/ou {{ mp }} descrito na carta, se houver

Enviar carta do {{ inv }} para a {{ table }}
:   2 de {{ ap }}
    .

Enviar carta da {{ table }} para a {{ inv }}
:   2 de {{ ap }}
    .

Realizar um Teste
:   2 de {{ ap }}

Interação com Objeto ou Personagem
:   2 de {{ ap }}
*   Falar com personagem
*   Mover a peça de um objeto para uma casa vazia adjacente a ela
*   Obter um {{ item }} do objeto

Despertar o {{ entity }}
:   2 de {{ sp }} e/ou {{ mp }}
*   E 2 de {{ sp }} e/ou {{ mp }} no início do turno para manter o {{ entity }} desperto

Evocar
:   2 de {{ mp }}

Descansar
:   Sacrificar o turno para recuperar 1 de {{ hp }}, {{ sp }} e {{ mp }}

Evoluir {{ companion }}
:   [!badge variant="secondary" text="Apenas no turno daquele companheiro"]
    O {{ companion }} sacrifica o seu turno e descarta 3 de {{ xp }}

Trocar cartas com uma Pilha de Descarte
:   Sacrificar o turno

<br>
<br>

### Apenas Fora de Batalha

Adquirir {{ class }}
:   Sacrificar o turno e descartar 5 cartas de recurso do mesmo nível da carta desejada

Progredir {{ class }}
:   Sacrificar o turno e descartar 3 cartas de recurso do mesmo nível da carta desejada

Incorporar {{ entity }}
:   Sacrificar o turno e descartar 5 cartas de recurso do mesmo nível do carta desejado

Liberar {{ entity }}
:   Sacrificar o turno e enterrar o seu {{ entity }}

Fabricar {{ item }}
:   Sacrificar o turno e descartar cartas de {{ item }} cuja combinação dos materiais seja igual ou superior aos materiais da carta desejada

<br>

### Apenas Durante a Batalha

Mover (por casa do tabuleiro)
:   1 de {{ ap }}
*  +1 de {{ ap }} para cada inimigo adjacente (exceto quando o inimigo está de costas para aquela casa do tabuleiro (_Área de Domínio_))
*  +1 de {{ ap }} para cada {{ alt }} de diferença

Ataque Normal
:   3 de {{ ap }}

    | {.compact}
    | --- | --- |
    | {{ dmg }}    | {{ str }} + {{ d1d2 }} |
    | {{ direct }} | 1                      |

Propor Pacto
:   3 de {{ ap }}
