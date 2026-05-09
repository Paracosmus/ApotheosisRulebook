---
label: Bônus
icon: diff
order: 45
---

# Bônus

{{ briefing `Bonus` `São valores incluídos em um cálculo e podem ser positivos ou negativos. São aplicados a um valor base, como um teste, Atributo, ` + dmg + `, etc. Eles são indicados por um sinal de mais (+) ou menos (-) seguido de um número ou expressão` }}

Quando um número é apresentado na forma **+X** ou **-X**, isso indica que se trata de um bônus.

!!!secondary Exemplo 1
  > {{ dmg }} = {{ str }} + {{ p'3' }} + {{ d1d6 }}

  * {{ dmg }} é o valor final que se deseja saber. O resultado do cálculo.
  * {{ str }} é a variável base que recebe os bônus.
  * Tanto o valor **3** quanto o valor {{ e1d6 }} são o bônus adicionados ao valor base.
!!!

!!!secondary Exemplo 2
  > {{ dmg }} = {{ str }} + {{ p'3' }} + {{ d1d6 }}

  * {{ dmg }} é o valor final que se deseja saber. O resultado do cálculo.
  * {{ str }} é a variável base que recebe os bônus.
  * Tanto o valor **3** quanto o valor {{ e1d6 }} são o bônus adicionados ao valor base.
!!!

Um bônus não pode ser definido por um efeito de carta, apenas por regras e mecânicas do jogo.

Os adicionais de Atributos (quando +X, -X) e os espaços extras dados por cartas são bônus, pois são adicionados ao Herói pela regra que define como devem ser aplicados. Por não estarem descritos no texto da carta, eles não são efeitos.

Isto porque o bônus é uma consequência de uma regra, e não algo que pode ser gerado pelos jogadores ativando cartas. Assim sendo, um bônus não pode ser impedido, negado ou modificado por efeitos de cartas a não ser que o efeito em sí explicitamente especifique esta capacidade.

!!!
Quando um efeito de carta age sobre um valor isto é chamado de [Modificador](/gameplay/modifiers.md).
!!!

---
