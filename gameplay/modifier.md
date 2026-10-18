---
label: Modificador
icon: boolean-on
order: 80
---

# Modificador

{{ briefing `Modifier` `São valores providos por um efeito que são aplicados à um cálculo e podem ser positivos ou negativos` }}

Algumas efeitos concedem modificadores para determinadas situações, como testes, ataques e defesas, podendo ser valores constantes, variáveis ou expressões.

!!!secondary Exemplo 1
  > Efeito: {{ permanent }} {{ p'+2' }} em testes de {{ faith }}

  * O valor {{ p'+2' }} é um modificador adicionado ao valor que obtiver em um teste cujo conhecimento seja {{ faith }}.
!!!

!!!secondary Exemplo 2
  > Efeito: {{ auto }} {{ attacked }} reduza o dano sofrido em ( {{ enr }} ✱ **2** )

  * O {{ dmg }} sofrido é o valor base, que recebe a modificação.
  * O modificador é definido como uma redução pelo texto do efeito, que explicita que o valor será subtraído do valor base.
  * ( {{ enr }} ✱ **2** ) é uma expressão entre parênteses, que precisa ser avaliada para determinar o valor do modificador. O resultado desta expressão é o valor do modificador, que é subtraído do valor base.
!!!

---

## Ordem de Aplicação

Quando um valor, como um Atributo ou o nível do Herói, recebe bônus e modificadores, ele é calculado nesta ordem:

1. **[Bônus](/gameplay/bonus.md) fixos**: são somados ao valor base. A ordem entre eles é irrelevante.
1. **[Bônus temporários](/gameplay/bonus.md#bônus-temporários)**: são somados ao resultado. A ordem entre eles é irrelevante.
1. **Modificadores**: são aplicados um a um, cada um sobre o valor deixado pelo anterior, em ordem de prioridade: o de maior prioridade é aplicado primeiro. Um efeito sem prioridade definida tem prioridade **0**. Dois efeitos com mesma prioridade são aplicados na ordem em que foram coletados.

!!!
Diferente dos bônus, a ordem dos modificadores importa. Um efeito que limita o valor, como "o nível máximo é **8**", precisa ser aplicado depois dos que o aumentam, e por isso tem uma prioridade menor que a deles.
!!!

---
