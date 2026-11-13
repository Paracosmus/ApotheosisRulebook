!!!danger
Esta seção ainda não foi completamente revisada. Algumas informações podem estar desatualizadas ou incompletas, e a formatação pode não estar finalizada.
!!!
    
# Batalha

A batalha acontece em um tabuleiro quadriculado. O tabuleiro pode conter paredes ou casas com diferentes níveis de altura. Cada casa possui um tipo de [terreno](/battle/board.md#terreno).

---

## AÇÕES

No seu turno, o personagem pode executar uma variedade de ações. As ações geralmente possuem algum custo de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação). Quando o personagem realizar ações até esgotar a sua [<span class="main"><b>AÇÃO</b></span>](/hero/#ação), o seu turno se encerra. Alguns tipos de ações podem ter custos associados como [<span class="skill"><b>MANA</b></span>](/hero/#mana) e [<span class="skill"><b>ESTAMINA</b></span>](/hero/#estamina).

### MOVER

Em seu turno, o personagem pode se mover no tabuleiro. Por padrão, o custo para mover é de 1 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) por casa. Alguns terrenos podem ter regras específicas para mover, por exemplo em um terreno de lama pode custar 2 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) por casa.

Pode-se mover para casas adjacentes com <b>ALTITUDE</b> diferente, pagando-se 1 [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) a mais para cada nível a mais de altura.

Quando terminar de mover, o personagem fica na direção em que se moveu até a casa de destino.

---

## DIREÇÃO (TODO)

---

## ÁREA DE INFLUÊNCIA
Todo personagem possui uma área de influência sobre o tabuleiro, que são as casas adjacentes à sua peça no tabuleiro, com exceção da casa atrás da peça em relação à sua orientação.

A área de influência aumenta em 1 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) o custo para que um personagem inimigo possa se mover para ela. Caso uma casa do tabuleiro esteja na área de influência de 2 ou mais personagens, o custo para se mover para esta casa aumenta em 1 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) para cada personagem inimigo.

---

## DESCANSAR
O personagem pode realizar uma [<span class="keyword-limit">Ação Total</span>](/gameplay/effect.md) para:

* Curar <span class="positive">10</span> de [<span class="hp"><b>VIDA</b></span>](/hero/#vida); e

* Recuperar <span class="positive">2</span> de **Energia** ([<span class="skill"><b>ESTAMINA</b></span>](/hero/#estamina) e/ou [<span class="skill"><b>MANA</b></span>](/hero/#mana)).

---

## Ataque Normal

> O personagem, sem nenhuma arma ou ferramenta, realiza um ataque corpo a corpo usando a força do seu corpo, mãos, pés, etc., para tentar causar o maior dano possível.

<style>
    .normal-attack {
        width: 50%;
        margin: 40px 0px;
        font-weight: bold;
    } .normal-attack td {
        font-size: 16px;
    } .normal-attack span {
        padding: 0 10px;
    }
</style>

:::normal-attack

| {.compact}
| ---                                                              | ---                            | ---                            |
| <span class="hse"></span> [<span class="house"><b>FOR</b></span>](/gameplay/attributes.md) + <span><span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">2</span></span></span></span> | <span class="hse"></span> 1 | <span class="hse"></span> 3 |

:::

É o ataque padrão que todo personagem pode realizar, sem a necessidade de cartas ou recursos.

Ao custo de 3 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) o personagem pode realizar um ataque <b>CONTATO</b> de 1 de <b>ALCANCE</b>, com <b>DANO</b> igual a ( [<span class="house"><b>FOR</b></span>](/gameplay/attributes.md) + <span class="tk tk-dice"><span class="tk-icon"></span><span class="tk-literal"><span class="tk-dice-number">1</span><span class="tk-dice-separator">d</span><span class="tk-dice-sides">2</span></span></span> ).

Este ataque não possui propriedades ou efeitos, é o mais simples e direto que um ataque pode ser.

---

## USAR UMA CARTA

Você pode utilizar uma carta conforme as regras durante a batalha. Você pode utilizar uma [<span class="skill"><b>HABILIDADE</b></span>](/cards/skills.md) pagando os seus custos. Você pode utilizar um [<span class="item"><b>ITEM</b></span>](/cards/item.md) para atacar. Você pode enviar uma carta do [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) para a [<span class="main"><b>MESA</b></span>](/hero/table/) ou enviar uma carta da [<span class="main"><b>MESA</b></span>](/hero/table/) para o [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md), pagando os custos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação).

---

## Dano

Todo ataque causa uma quantidade de <b>DANO</b> ao alvo. Desse <b>DANO</b> sofrido, subtrai-se a defesa do alvo — isto é, todos os descontos e reduções que o alvo aplica ao <b>DANO</b> recebido. O resultado final é a <b>LESÃO</b>, que corresponde à quantidade de [<span class="hp"><b>VIDA</b></span>](/hero/#vida) que o personagem perde, calculada observando os seguintes passos:

* +1 de <b>LESÃO</b> se o <b>DANO</b> for maior ou igual à metade da [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) do alvo
* +1 de <b>LESÃO</b> se o <b>DANO</b> for maior ou igual à [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) do alvo
* +1 de <b>LESÃO</b> para cada 5 pontos que o <b>DANO</b> for maior que a [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) do alvo

!!!info
Por exemplo, se um alvo tem <u>_6 de [<span class="house"><b>CON</b></span>](/gameplay/attributes.md)_</u> e recebe um ataque de <u>_18 de <b>DANO</b>_</u>, o alvo sofre <u>_4 de <b>LESÃO</b>_</u>. O cálculo é feito da seguinte forma:

* +1 de <b>LESÃO</b> por ter sofrido um ataque maior ou igual a ( [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) / 2 ) → (18 ≥ 6 / 2)
* +1 de <b>LESÃO</b> por ter sofrido um ataque maior ou igual à [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) → (18 ≥ 6)
* +1 de <b>LESÃO</b> por ter sofrido um ataque 5 pontos maior que a [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) → (18 ≥ 11)
* +1 de <b>LESÃO</b> por ter sofrido um ataque 10 pontos maior que a [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) → (18 ≥ 16)

==- Expresso em fórmula:
$$
\small
\text{Injury} =
\text{Dmg} \geq \left\lfloor \dfrac{\text{END}}{2} \right\rfloor
\; ? \; \left( \text{Dmg} \geq \text{END}
    \; ? \; 2 + \left\lfloor \dfrac{\text{Dmg} - \text{END}}{5} \right\rfloor
    : 1 \right)
: 0
$$

<br>

> $ \text{O critério inicial é verificar se } \text{Dmg} \geq \left\lfloor \dfrac{\text{END}}{2} \right\rfloor $
> $ \text{Substituindo os valores:} $
> $ \left\lfloor \dfrac{6}{2} \right\rfloor = \left\lfloor 3 \right\rfloor = 3 $
> $ \text{Agora verificamos a desigualdade:} \quad 18 \geq 3 $
> $ \text{Como a condição é verdadeira, seguimos para o próximo passo.} $

> $ \text{Agora verificamos se } \text{Dmg} \geq \text{END} $
> $ \text{Substituindo os valores:} \quad 18 \geq 6 $
> $ \text{A condição é verdadeira, então usamos a fórmula:} $
> $ \text{Injury} = 2 + \left\lfloor \dfrac{\text{Dmg} - \text{END}}{5} \right\rfloor $
> $ \text{Agora seguimos para resolver essa equação.} $

> $ \text{Calculamos primeiro:} \quad \text{Dmg} - \text{END} $
> $ 18 - 6 = 12 $
> $ \text{Agora dividimos por 5:} \quad \dfrac{12}{5} = 2.4 $
> $ \text{Aplicamos a função piso:} \quad \left\lfloor 2.4 \right\rfloor = 2 $

> $ \text{Injury} = 2 + 2 $
> $ \text{Injury} = 4 $

===
!!!

### Falha

Observando a equação acima, note que quando o <b>DANO</b> for menor que a metade da [<span class="house"><b>CON</b></span>](/gameplay/attributes.md) do alvo, o ataque falha e não causa <b>LESÃO</b>. Neste caso é considerado que o atacante errou o ataque, que pode ser por diversos motivos, como o alvo se esquivou, se defendeu ou o ataque não atingiu o alvo.

### Rolagem Perfeita

Quando o <b>DANO</b> de um ataque incluir a rolagem de dados, aplica-se a regra de [rolagem perfeita](/gameplay/die.md#dados-extras-rolagem-perfeita) ao dado principal da rolagem, somando o resultado dos dados extras ao <b>DANO</b> do ataque.

---

## TERRENO (TODO)

---

- [ ]  Explicar o que é um ataque. É a ação de ataque normal ou a ativação de uma carta que possui um dano na sua barra de ação. Um dano causado por um efeito não é um ataque, assim como quando você recebe dano de explosivo, apenas o tile alvo que foi atacado
- [ ]  Explicar a diferença de sofrer dano, lesão e perder vida
