# Modificador

|||{.briefing} [!badge text="Modifier" variant="ghost"]
  São valores providos por um efeito que são aplicados à um cálculo e podem ser positivos ou negativos
|||
    
Algumas efeitos concedem modificadores para determinadas situações, como testes, ataques e defesas, podendo ser valores constantes, variáveis ou expressões.

!!!secondary Exemplo 1
  > Efeito: [<span class="keyword-activation">Permanente</span>](/cards/effect.md) <span class="positive">+2</span> em testes de [<span class="knowledge"><b>FÉ</b></span>](/hero/knowledge.md#fé)

  * O valor <span class="positive">+2</span> é um modificador adicionado ao valor que obtiver em um teste cujo conhecimento seja [<span class="knowledge"><b>FÉ</b></span>](/hero/knowledge.md#fé).
!!!

!!!secondary Exemplo 2
  > Efeito: [<span class="keyword-activation">Auto</span>](/cards/effect.md) [<span class="keyword-timing">Quando Atacado</span>](/cards/effect.md) reduza o dano sofrido em ( [<span class="house"><b>CON</b></span>](/hero/attributes.md) ✱ **2** )

  * O <b>DANO</b> sofrido é o valor base, que recebe a modificação.
  * O modificador é definido como uma redução pelo texto do efeito, que explicita que o valor será subtraído do valor base.
  * ( [<span class="house"><b>CON</b></span>](/hero/attributes.md) ✱ **2** ) é uma expressão entre parênteses, que precisa ser avaliada para determinar o valor do modificador. O resultado desta expressão é o valor do modificador, que é subtraído do valor base.
!!!

---

## Modificadores Temporários

Também conhecidos como Vantagem (_Buff_) e Penalidade (_Debuff_).

São modificadores não permanentes, que um personagem pode receber. Por serem temporários, eles tem um "prazo de validade" e se dissipam automaticamente após um determinado evento ou condição, explicitado pelo efeito que os concedeu.

Todo efeito de modificador temporário utilizam a mecânica de [<span class="keyword-limit">Residual</span>](/cards/effect.md) e portanto, explicitam sua duração no corpo do efeito.

!!!secondary Exemplo
  > _Estimulante_: [<span class="keyword-activation">Ativar</span>](/cards/effect.md) [<span class="keyword-limit">Residual</span>](/cards/effect.md) <span class="positive">+1</span> de [<span class="house"><b>AGI</b></span>](/hero/attributes.md) até o [<span class="keyword-timing">Final da Batalha</span>](/cards/effect.md).

  Sendo do tipo [<span class="keyword-limit">Residual</span>](/cards/effect.md), o modificador é aplicado imediatamente e mesmo que a carta seja removida de jogo, ele se mantém ativo até o [<span class="keyword-timing">Final da Batalha</span>](/cards/effect.md), quando se dissipa automaticamente.
!!!

---
