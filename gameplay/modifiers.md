# Modificadores

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

São de curta duração, geralmente duram até o início do próximo turno de quem os aplicou, até o final da batalha ou até que a carta ativada fique sem contadores de tempo.

---
