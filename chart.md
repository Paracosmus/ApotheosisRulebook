---
label: Cartilha
layout: page
---

# Cartilha

## Durante seu Turno

Ativar Carta
:   Custo de {{ ap }} e/ou Energia ({{ sp }}, {{ mp }} e/ou **Essência**), além dos requerimentos e custos adicionais descritos na carta, se houver

Enviar carta do {{ inv }} para a {{ table }}
:   **2** de {{ ap }}
<br>

Enviar carta da {{ table }} para o {{ inv }}
:   **2** de {{ ap }}
<br>

Interagir com Objeto ou Personagem
:   **2** de {{ ap }}
*   Falar com personagem
*   Mover a peça de um Objeto para uma casa vazia adjacente a ela
*   Obter um {{ item }} de uma peça do tipo Container

Despertar o {{ entity }}
:   **Consumir** Energia igual ao nível do {{ entity }}
*   {{ n '+' }} **Consumir** Energia igual ao nível do {{ entity }} para mantê-lo desperto

Evocar uma {{ summon }}
:   **2** de {{ mp }} por nível do {{ companion }} a ser evocado

Descansar
:   Ação total para curar {{p'10'}} de {{ hp }} e recuperar {{p'2'}} de **Energia**

Trocar cartas com a Pilha de Descarte
    - _Comprar {{ item }}_
    - _Aprender {{ skill }}_
    - _Recrutar {{ companion }}_
    - _Colher {{ event }}_
:   Ação total
<br><br><br><br><br><br>

Propor/Fechar Pacto
:   Ação total (_de todos os envolvidos_)

<br>
<br>

## Apenas Fora de Batalha

Realizar um Teste
:   **2** de {{ ap }}

Adquirir {{ class }}
:   Ação total e enterrar {{n 5}} cartas de recurso do mesmo nível da carta desejada

Progredir {{ class }}
:   Ação total e enterrar {{n 3}} cartas de recurso do mesmo nível da carta desejada

Incorporar {{ entity }}
:   Ação total e enterrar {{n 5}} cartas de recurso do mesmo nível da carta desejada

Liberar {{ entity }}
:   Ação total e descartar o seu {{ entity }}

Fabricar {{ item }}
:   Ação total e enterrar cartas de {{ item }} até que a combinação dos materiais seja igual ou superior aos materiais da carta desejada

<br>

## Apenas Durante uma Batalha

Mover (por casa do tabuleiro)
:   **1** de {{ ap }}
*  {{n '+1'}} de {{ ap }} para desengajar de cada inimigo adjacente
*  {{n '+1'}} de {{ ap }} para cada {{ alt }} de diferença

Ataque Normal
:   **3** de {{ ap }}

    | {{ dmg }}    | {{ str }} + {{ d1d2 }} | {.compact}
    | ------------ | ---------------------- |
    | {{ direct }} | 1                      |
