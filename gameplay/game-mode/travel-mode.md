---
label: Modo de Viagem
icon: milestone
order: 30
---

# Modo de Viagem

{{ briefing `É um modo utilizado quando o grupo se desloca de um local do mapa da região para outro local distante, sem que seja necessário jogar todos os momentos de uma longa viagem.` }}

Geralmente, esse método é utilizado para deslocamentos de grandes distâncias, como ir de uma cidade para a cidade vizinha, viajar pelos mares entre portos ou atravessar uma cadeia de montanhas, entre outros.

O tempo de duração de uma viagem é medido em períodos do dia, e pode variar dependendo da distância entre os locais, condições das estradas, meios de transporte utilizados, e outros fatores.

Durante a viagem, o grupo pode enfrentar eventos e desafios específicos relacionados ao deslocamento, como encontros aleatórios, condições climáticas adversas, ou efeitos de cartas que podem ser ativados durante a viagem.

---

## Iniciando uma Viagem

Uma viagem começa quando o grupo anuncia que irá se deslocar para outro local no mapa.

{.list-icon}
- 🕦 Verifique a distância em [períodos do dia](/gameplay/time.md#período-do-dia) entre o local atual e o local de destino. Este será o tempo inicial necessário para a viagem, caso não haja interrupções. O mapa da região, geralmente fornecido pela campanha, contém esses valores.

- 👣 Aplique quaisquer modificadores de tempo de viagem, geralmente causados pela situação das estradas ou do percurso, por condições de campanha, meios de transporte, efeitos de cartas etc., e então determine o tempo total de viagem.

- 🗺️ O grupo então entra no _"modo de viagem"_, e suas regras específicas de jogo são aplicadas.

---

## Durante a Viagem

O grupo pode realizar apenas ações coletivas no modo de viagem, ou seja, as ações tomadas durante a viagem devem ser decididas e realizadas por todo o grupo, e não por personagens individualmente:

\:icon-move-to-end: **Continuar**: O grupo dá continuidade à viagem, seguindo o percurso determinado.
:   - Avance para o próximo período do dia.
    - Revele a carta do topo do {{ sanctuary }}. A carta é ativada, se possível. O efeito da carta é aplicado a todos os personagens do grupo e deve ser resolvido. Se, pelo efeito da carta, ela for enviada para um personagem em vez de ser descartada, apenas um personagem é escolhido para recebê-la.
    - O contador de tempo de viagem é **reduzido** em {{ p 1 }}. Se o contador de tempo de viagem chegar a 0, a viagem é considerada concluída e o grupo chega ao destino.

\:icon-dash: **Pausar**: O grupo interrompe a viagem para descansar, explorar ou realizar outras atividades.
:   - Nesse caso, o contador de tempo de viagem é mantido, e o grupo pode jogar seus respectivos turnos normalmente, seguindo as regras do [[story-mode|Modo Narrativo]] e considerando o local do caminho em que se encontram.
    - Para cada 4 rodadas pausadas, deve-se avançar o período do dia uma vez, mesmo quando essas rodadas acontecerem em pontos diferentes desta viagem.

\:icon-move-to-start: **Retornar**: O grupo decide voltar pelo percurso percorrido.
:   - Avance para o próximo período do dia.
    - Revele a carta do topo do {{ sanctuary }}. A carta é ativada, se possível. O efeito da carta é aplicado a todos os personagens do grupo e deve ser resolvido. Se, pelo efeito da carta, ela for enviada para um personagem em vez de ser descartada, apenas um personagem é escolhido para recebê-la.
    - O contador de tempo de viagem é **incrementado** em {{ n 1 }}. Se o contador de tempo de viagem chegar ao valor inicial, a viagem é considerada concluída e o grupo retorna ao local de origem.

!!!
Algumas campanhas e objetivos podem modificar as ações disponíveis durante o modo de viagem, como permitir que o grupo encontre recursos, mude de rota ou destino, enfrente desafios ou eventos específicos.

Também podem determinar o que acontece no momento em que uma carta do topo do {{ sanctuary }} é ativada pela viagem, substituindo essa mecânica por outra específica.
!!!

!!!
Observe que algumas cartas de {{ event }} podem requerer condições específicas de viagem, como distância, tempo, local, entre outras, para serem ativadas.
!!!

---

## Fim da Viagem

Ao chegar ao destino, avance para o próximo período do dia, e o modo de viagem se encerra, retornando ao modo narrativo.

O grupo deve resolver quaisquer efeitos ou eventos que possam ocorrer ao chegar no novo local, como recompensas, resolver efeitos de cartas ou enfrentar desafios específicos do local.

---

## Viagem Rápida

Uma viagem rápida é uma mecânica que permite ao grupo se deslocar instantaneamente entre locais, sem a necessidade de jogar o modo de viagem.

Essa opção de viagem não fica disponível livremente e só se torna acessível por meio de efeitos de cartas ou de condições estabelecidas pela campanha, como viajar com caravanas mercantes, passagens de navios e trens, entre outras.

Quando uma viagem rápida é realizada, o grupo deve:
- Resolver quaisquer efeitos de cartas e condições de campanha relacionados ao [início](#iniciando-uma-viagem) de uma viagem ou viagem rápida.
- Calcular normalmente o tempo necessário para a viagem e seus modificadores.
- O período do dia é avançado de acordo com o tempo de viagem, e o grupo chega ao novo local sem a necessidade de jogar o modo de viagem.
- Resolver quaisquer efeitos de cartas e condições de campanha relacionados ao [fim](#fim-da-viagem) de uma viagem ou viagem rápida.

---
