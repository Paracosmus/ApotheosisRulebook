---
label: Bônus
icon: diff
order: 90
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

Um bônus fixo não pode ser definido por um efeito de carta, apenas por regras e mecânicas do jogo. Efeitos {{ lingering }} podem conceder [bônus temporários](#bônus-temporários).

Os adicionais de Atributos (quando +X, -X) e os espaços extras dados por cartas são bônus, pois são adicionados ao Herói pela regra que define como devem ser aplicados. Por não estarem descritos no texto da carta, eles não são efeitos.

Isto porque o bônus é uma consequência de uma regra, e não algo que pode ser gerado pelos jogadores ativando cartas. Assim sendo, um bônus não pode ser impedido, negado ou modificado por efeitos de cartas a não ser que o efeito em sí explicitamente especifique esta capacidade.

!!!
Quando um efeito de carta age sobre um valor isto é chamado de [Modificador](/gameplay/modifier.md).
!!!

---

## Bônus Temporários

Também conhecidos como Vantagem (_Buff_) e Penalidade (_Debuff_).

São bônus não permanentes que um personagem pode receber de um efeito {{ lingering }}. Um bônus temporário é sempre um valor constante somado por um tempo, como "{{ p'+1' }} até o final da rodada", e nunca possui condições. Por ser temporário, ele tem um "prazo de validade", explicitado pelo efeito que o concedeu, e se dissipa automaticamente ao final dele.

No cálculo de um valor, os bônus temporários são somados depois dos bônus fixos e antes dos [modificadores](/gameplay/modifier.md#ordem-de-aplicação), em qualquer ordem entre si.

!!!secondary Exemplo
  > _Estimulante_: {{ activate }} {{ lingering }} {{ p'+1' }} de {{ agi }} até o {{ endOfBattle }}.

  Sendo do tipo {{ lingering }}, o bônus é aplicado imediatamente e, mesmo que a carta seja removida de jogo, ele se mantém até o {{ endOfBattle }}, quando se dissipa automaticamente.
!!!

---
