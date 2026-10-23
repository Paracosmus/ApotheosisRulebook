# Modificador

|||{.briefing} [!badge text="Modifier" variant="ghost"]
  São valores providos por um efeito que são aplicados à um cálculo e podem ser positivos ou negativos
|||
    
Algumas efeitos concedem modificadores para determinadas situações, como testes, ataques e defesas, podendo ser valores constantes, variáveis ou expressões.

!!!secondary Exemplo 1
  > Efeito: [<span class="keyword-activation">Permanente</span>](/gameplay/effect.md) <span class="positive">+2</span> em testes de [<span class="knowledge"><b>FÉ</b></span>](/gameplay/knowledge.md#fé)

  * O valor <span class="positive">+2</span> é um modificador adicionado ao valor que obtiver em um teste cujo conhecimento seja [<span class="knowledge"><b>FÉ</b></span>](/gameplay/knowledge.md#fé).
!!!

!!!secondary Exemplo 2
  > Efeito: [<span class="keyword-activation">Auto</span>](/gameplay/effect.md) [<span class="keyword-timing">Quando Atacado</span>](/gameplay/effect.md) reduza o dano sofrido em ( [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) ✱ **2** )

  * O <b>DANO</b> sofrido é o valor base, que recebe a modificação.
  * O modificador é definido como uma redução pelo texto do efeito, que explicita que o valor será subtraído do valor base.
  * ( [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) ✱ **2** ) é uma expressão entre parênteses, que precisa ser avaliada para determinar o valor do modificador. O resultado desta expressão é o valor do modificador, que é subtraído do valor base.
!!!

---

## Ordem de Aplicação

Quando um valor, como um Atributo ou o nível do Herói, recebe bônus e modificadores, ele é calculado nesta ordem:

1. **[Bônus](/gameplay/bonus.md) fixos**: são somados ao valor base. A ordem entre eles é irrelevante.
1. **[Bônus temporários](/gameplay/bonus.md#bônus-temporários)**: são somados ao resultado. A ordem entre eles é irrelevante.
1. **Modificadores**: são aplicados um a um, cada um sobre o valor deixado pelo anterior, em ordem de prioridade: o de maior prioridade é aplicado primeiro. Um efeito sem prioridade definida tem prioridade **0**. Dois efeitos com mesma prioridade são aplicados na ordem em que foram coletados.
2. **Limites da regra**: por último, o valor é ajustado aos limites que a regra define, como o mínimo de **1** de um Atributo. Este ajuste é realizado após a aplicação de todos os efeitos, portanto ele sempre prevalece.

!!!
Diferente dos bônus, a ordem dos modificadores importa. Um efeito que limita o valor, como "o nível máximo é **8**", precisa ser aplicado depois dos que o aumentam, e por isso tem uma prioridade menor que a deles.
!!!

!!!secondary Exemplo
  > Efeito: [<span class="keyword-activation">Permanente</span>](/gameplay/effect.md) se a sua [<span class="house"><b>FOR</b></span>](/gameplay/attributes.md) for exatamente **1**, ela passa a ser **2**.

  * Os bônus e modificadores da [<span class="house"><b>FOR</b></span>](/gameplay/attributes.md) do Herói resultam em **-2**. O efeito não age, pois o valor não é **1**.
  * O limite da regra transforma **-2** em **1**. A [<span class="house"><b>FOR</b></span>](/gameplay/attributes.md) do Herói é **1**, e não **2**.
!!!

---
