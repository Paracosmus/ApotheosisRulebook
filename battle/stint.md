!!!danger
Esta seção ainda não foi completamente revisada. Algumas informações podem estar desatualizadas ou incompletas, e a formatação pode não estar finalizada.
!!!
    
# Ciclo

|||{.briefing} [!badge text="Stint" variant="ghost"]
  O ciclo é o período entre uma [<span class="keyword-timing">Fase de Recomposição</span>](/gameplay/effect.md) e a próxima. Nele, os personagens jogam em rodadas, na ordem da fila de turnos, até a fila ficar vazia.
|||
    
A batalha se divide em ciclos, cada ciclo em rodadas, e cada rodada nos turnos dos personagens. Só os personagens têm turno: um objeto não age e, por isso, não tem turno.

```mermaid
flowchart TD
    inicio(["Início da Batalha"]) --> recomposicao["Fase de Recomposição"]
    recomposicao --> rodada["Rodada<br/>cada personagem da fila de turnos joga um turno"]
    rodada --> pergunta{"Ainda há personagens<br/>na fila de turnos?"}
    pergunta -->|"Sim: nova rodada"| rodada
    pergunta -->|"Não: novo ciclo"| recomposicao
    rodada -.->|"batalha declarada encerrada"| final(["Final da Batalha"])
```

---

## Batalha [!badge text="Battle" variant="ghost"]

A batalha abre com o [<span class="keyword-timing">Início da Batalha</span>](/gameplay/effect.md), antes de qualquer ação dos personagens, e fecha com o [<span class="keyword-timing">Final da Batalha</span>](/gameplay/effect.md), quando é declarada encerrada. São os momentos dos efeitos com essas palavras-chave.

Entre os dois, joga-se um ciclo após o outro.

---

## Fase de Recomposição [!badge text="Reset Phase" variant="ghost"]

Todo ciclo começa por esta fase, em três passos:

1. É o momento dos efeitos [<span class="keyword-timing">Fase de Recomposição</span>](/gameplay/effect.md).
2. Todos os personagens são ordenados por [Iniciativa](/battle/initiative.md), formando a fila de turnos do ciclo.
3. Cada personagem recebe pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) iguais à sua [<span class="house"><b>AGI</b></span>](/gameplay/attributes.md), no mínimo **3** e no máximo **25**, somados aos que já tem.

Os pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) não se perdem de um ciclo para o outro: o que sobra fica guardado. Mas um personagem nunca tem mais pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) do que a sua [<span class="house"><b>AGI</b></span>](/gameplay/attributes.md) somada ao seu nível. O que passar disso se perde. Esse máximo nunca fica abaixo de **3**.

!!!secondary Exemplo
Um personagem de nível **10** e **10** de [<span class="house"><b>AGI</b></span>](/gameplay/attributes.md) pode ter até **20** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação).

* Ele encerra o ciclo com **3** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação). Na [<span class="keyword-timing">Fase de Recomposição</span>](/gameplay/effect.md), um efeito lhe dá **2**, e depois ele recebe **10**: fica com **15**.
* Se tivesse guardado **15**, ficaria com **20**, e os outros **5** se perderiam.
!!!

---

## Rodada [!badge text="Round" variant="ghost"]

Na rodada, cada personagem da fila de turnos joga um turno, na ordem da fila. Quando todos jogaram, começa uma nova rodada com quem continua na fila.

---

## Turno

|||{.briefing} [!badge text="Turn" variant="ghost"]
  O turno é a vez de um personagem agir na batalha.
|||
    
No seu turno, o personagem age: move a sua peça, ataca, ativa efeitos, etc., pagando o custo de cada ação.

O turno termina quando o personagem faz uma ação que encerra o turno ou encerra o seu ciclo. Então joga o próximo personagem da fila. As ações que encerram o turno são:

* ativar por conta própria um efeito ou uma [técnica](/gameplay/technique.md), de qualquer origem, como uma carta ou um [Modelo](/battle/piece/dummy.md);
* fazer um [ataque normal](/battle/#ataque-normal).

Ativar por conta própria é escolher um efeito e ativá-lo manualmente, sem gatilho e sem ser em [resposta](/gameplay/effect.md#responder-a-um-efeito) a outro efeito. Assim, não encerram o turno os efeitos [<span class="keyword-activation">Permanente</span>](/gameplay/effect.md) e [<span class="keyword-activation">Auto</span>](/gameplay/effect.md), nem um efeito [<span class="keyword-activation">Ativar</span>](/gameplay/effect.md) que foi engatilhado ou ativado em resposta.

Nenhuma outra ação encerra o turno. Ficar sem pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) também não: o personagem continua podendo fazer as ações que não custam [<span class="main"><b>AÇÃO</b></span>](/hero/#ação).

Os efeitos de fase inicial, como [<span class="keyword-timing">Sua Fase Inicial</span>](/gameplay/effect.md), acontecem no início do primeiro turno de cada personagem no ciclo, e os de fase final, como [<span class="keyword-timing">Sua Fase Final</span>](/gameplay/effect.md), quando o ciclo dele termina.

---

## Encerrar o Ciclo

O ciclo de um personagem termina quando:

* ele declara que encerra o seu ciclo, o que pode fazer a qualquer momento, mesmo sem ter agido no turno;
* um turno seu termina e ele está sem pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação);
* ele faz uma [<span class="keyword-limit">Ação Total</span>](/gameplay/effect.md), que é a única ação dele no ciclo.

Ao encerrar o ciclo, o personagem sai da fila de turnos e não volta a ela neste ciclo, mesmo que receba pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação). Se for o seu turno, o turno termina.

!!!
Encerrar o ciclo só tira o personagem da fila de turnos. Ele continua podendo ativar efeitos em [resposta](/gameplay/effect.md#responder-a-um-efeito) e efeitos [engatilhados](/gameplay/effect.md#requerimentos-de-ativação), pagando os custos deles, inclusive em [<span class="main"><b>AÇÃO</b></span>](/hero/#ação). Por isso, guardar pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) pode ser estratégico.
!!!

!!!secondary Exemplo
Na [<span class="keyword-timing">Fase de Recomposição</span>](/gameplay/effect.md), a fila de turnos fica A, B e C, com **5**, **3** e **4** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação).

**Rodada 1**

* A move a sua peça, gastando **2** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação), e ativa uma carta que custa **1** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação). A ativação encerra o turno, e A fica com **2** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação).
* B ativa uma carta que custa **3** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação). O turno termina com B sem [<span class="main"><b>AÇÃO</b></span>](/hero/#ação), o que encerra o seu ciclo.
* C encerra o seu ciclo sem agir e guarda os seus **4** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação).

**Rodada 2**

* Só A continua na fila. Ele move a sua peça, gastando os seus **2** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação). Sem [<span class="main"><b>AÇÃO</b></span>](/hero/#ação), o turno continua: A ativa um efeito que não custa [<span class="main"><b>AÇÃO</b></span>](/hero/#ação), e o turno termina, encerrando o seu ciclo.

Fora da fila, B e C ainda podem responder às cartas de A, e C pode pagar essas respostas com os [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) que guardou.

A fila de turnos ficou vazia: o ciclo termina, e o próximo começa pela [<span class="keyword-timing">Fase de Recomposição</span>](/gameplay/effect.md).
!!!

---

## Entrar e Sair da Fila de Turnos

Um personagem que sai do tabuleiro, morre ou é nocauteado sai da fila de turnos. Mover a peça no tabuleiro não altera o seu lugar na fila.

Um personagem que entra na fila durante o ciclo, depois da [<span class="keyword-timing">Fase de Recomposição</span>](/gameplay/effect.md), como quem volta ao tabuleiro, é revivido ou acorda, entra no **final** da fila. Ele não recebe pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) ao entrar, pois só os recebe na [<span class="keyword-timing">Fase de Recomposição</span>](/gameplay/effect.md), mas continua com os que já tinha.

Quem já encerrou o seu ciclo não volta à fila neste ciclo, mesmo que volte ao tabuleiro.

!!!secondary Exemplo
Um efeito tira do tabuleiro uma peça com **5** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) e a traz de volta uma rodada depois. Ela entra no final da fila, ainda com os seus **5** de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação).
!!!

!!!
Se o personagem voltar durante a [<span class="keyword-timing">Fase de Recomposição</span>](/gameplay/effect.md), como acontece com a maioria dos efeitos que retiram personagens do tabuleiro, ele entra na fila de turnos recalculada para o novo ciclo e recebe pontos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) normalmente.
!!!

---

## Simultaneidade de Efeitos
Note que todos os efeitos que devem ser aplicados durante uma determinada fase são aplicados simultaneamente, ou seja, todos acontecem ao mesmo tempo, não tendo uma sucessão ou ordem a ser seguida.

!!!
Por exemplo: Se um efeito diz que “No início do seu turno você deve deitar 2 de [<span class="skill"><b>MANA</b></span>](/hero/#mana)” e outro efeito diz que “No início do seu turno você recupera 2 de [<span class="skill"><b>MANA</b></span>](/hero/#mana)”, ambos os efeitos correm simultaneamente, portanto você não pode usar a [<span class="skill"><b>MANA</b></span>](/hero/#mana) recuperada no segundo efeito para pagar o primeiro.

Neste caso recomenda-se como boa prática, aplicar todos os efeitos dedutivos primeiro e então aplicar os efeitos de recuperação, isso evita que recursos sejam utilizados antes de estarem disponíveis.
!!!
