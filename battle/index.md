!!!danger
Esta seção ainda não foi completamente revisada. Algumas informações podem estar desatualizadas ou incompletas, e a formatação pode não estar finalizada.
!!!
    
# Batalha

A batalha acontece em um tabuleiro quadriculado de 11x11 casas. No tabuleiro, podem conter casas bloqueadas ou com diferentes níveis de altura. Cada casa possui um tipo de terreno (grama, terra, água, lama, areia etc.).

---

## AÇÕES

No seu turno, o personagem pode executar uma variedade de ações. As ações geralmente possuem algum custo de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação). Quando o personagem realizar ações até esgotar a sua [<span class="main"><b>AÇÃO</b></span>](/hero/#ação), o seu turno se encerra. Alguns tipos de ações podem ter custos associados como [<span class="skill"><b>MANA</b></span>](/hero/#mana) e [<span class="skill"><b>ESTAMINA</b></span>](/hero/#estamina).

### MOVER

Em seu turno, o personagem pode se mover no tabuleiro. Por padrão, o custo para mover é de 1 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) por casa. Alguns terrenos podem ter regras específicas para mover, por exemplo em um terreno de lama pode custar 2 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) por casa.

Pode-se mover para casas adjacentes com <b>ALTITUDE</b> diferentes, pagando-se 1 [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) a mais para cada nível a mais de altura.

Existem casas no tabuleiro que podem estar bloqueadas (ex.: uma parede) ou obstruídas (ex.: um corpo no chão, uma porta). Não se pode passar por ou ocupar casas bloqueadas. É possível passar por casas ocupadas, mas não é possível ocupá-las (encerrar a movimentação sobre esta casa).

Quando terminar de mover, o personagem fica na direção que se moveu até a casa de destino.

Adjacente
Distância
Casas

---

## DIREÇÃO (TODO)

---

## ÁREA DE DOMÍNIO
Todo personagem possui uma área de domínio sobre o tabuleiro, que são as casas adjacentes a sua peça no tabuleiro com exceção da casa atrás da peça em relação a sua orientação.

A área de domínio aumenta em 1 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) o custo para que um personagem inimigo possa se mover para ela. Caso uma casa do tabuleiro esteja na área de domínio de 2 ou mais personagens, o custo para se mover para esta casa aumenta em 1 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) para cada personagem inimigo.

---

## DESCANSAR
O personagem pode sacrificar o seu turno para recuperar:

* 1 de [<span class="hp"><b>VIDA</b></span>](/hero/#vida).
ou
* 2 de [<span class="skill"><b>ESTAMINA</b></span>](/hero/#estamina) e/ou [<span class="skill"><b>MANA</b></span>](/hero/#mana).

---

## Ataque Normal

> O personagem sem nenhuma arma ou ferramenta, realiza um ataque corpo a corpo usando a força do seu corpo, mãos, pés, etc., para tentar causar o maior dano possível.

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
| <span class="house"></span> [<span class="house"><b>FOR</b></span>](/hero/attributes.md) + <span></span> | <span class="house"></span> 1 | <span class="house"></span> 3 |

:::

É o ataque padrão que todo personagem pode realizar, sem a necessidade de cartas ou recursos.

Ao custo de 3 de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação) o personagem pode realizar um ataque <b>DIRETO</b> de 1 de <b>ALCANCE</b>, com <b>DANO</b> igual a ( [<span class="house"><b>FOR</b></span>](/hero/attributes.md) +  ).

Este ataque não possui propriedades ou efeitos, é o mais simples e direto que um ataque pode ser.

---

## USAR UMA CARTA

Você pode utilizar uma carta conforme as regras durante a batalha. Você pode utilizar uma HABILIDADE pagando os seus custos. Você pode utilizar uma FERRAMENTA para atacar. Você pode enviar uma carta do [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md) para a [<span class="main"><b>MESA</b></span>](/hero/table/) ou enviar uma carta da [<span class="main"><b>MESA</b></span>](/hero/table/) para o [<span class="main"><b>INVENTÁRIO</b></span>](/hero/inventory.md), pagando os custos de [<span class="main"><b>AÇÃO</b></span>](/hero/#ação).

---

## Dano

Todo ataque causa uma quantidade de <b>DANO</b>. O personagem que recebeu o ataque perde uma quantidade de [<span class="hp"><b>VIDA</b></span>](/hero/#vida) equivalente ao <b>DANO</b> sofrido. A quantidade de [<span class="hp"><b>VIDA</b></span>](/hero/#vida) perdida é chamada de <b>LESÃO</b> e calculada observando os seguintes passos.

* +1 de <b>LESÃO</b> se o <b>DANO</b> for maior ou igual à metade da [<span class="house"><b>CON</b></span>](/hero/attributes.md) do alvo
* +1 de <b>LESÃO</b> se o <b>DANO</b> for maior ou igual à [<span class="house"><b>CON</b></span>](/hero/attributes.md) do alvo
* +1 de <b>LESÃO</b> para cada 5 pontos que o <b>DANO</b> for maior que a [<span class="house"><b>CON</b></span>](/hero/attributes.md) do alvo

!!!info
Por exemplo, se um alvo tem <u>_6 de [<span class="house"><b>CON</b></span>](/hero/attributes.md)_</u> e recebe um ataque de <u>_18 de <b>DANO</b>_</u>, o alvo sofre <u>_4 de <b>LESÃO</b>_</u>. O cálculo é feito da seguinte forma:

* +1 de <b>LESÃO</b> por ter sofrido um ataque maior ou igual à ( [<span class="house"><b>CON</b></span>](/hero/attributes.md) / 2 ) → (18 ≥ 6 / 2)
* +1 de <b>LESÃO</b> por ter sofrido um ataque maior ou igual à [<span class="house"><b>CON</b></span>](/hero/attributes.md) → (18 ≥ 6)
* +1 de <b>LESÃO</b> por ter sofrido um ataque 5 pontos maior que a [<span class="house"><b>CON</b></span>](/hero/attributes.md) → (18 ≥ 11)
* +1 de <b>LESÃO</b> por ter sofrido um ataque 10 pontos maior que a [<span class="house"><b>CON</b></span>](/hero/attributes.md) → (18 ≥ 16)

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

Observando a equação acima, note que quando o <b>DANO</b> for menor que a metade da [<span class="house"><b>CON</b></span>](/hero/attributes.md) do alvo, o ataque falha e não causa <b>LESÃO</b>. Neste caso é considerado que o atacante errou o ataque, que pode ser por diversos motivos, como o alvo se esquivou, se defendeu ou o ataque não atingiu o alvo.

### Crítico

Quando o <b>DANO</b> de um ataque incluir a rolagem de dados, um desses dados deve ser considerado um dado crítico. Caso o dado crítico tenha o valor máximo, o atacante deve rolar  (+1D3) e continuar assim até que o dado crítico não tenha o valor máximo. O resultado da soma dos dados críticos é adicionado ao <b>DANO</b> do ataque.

---

## ALCANCE (TODO)

Distância
Casas
Adjacentes

### <span class="icon"></span> Direto

TODO

Deve ser feito o cálculo de alcance para verificar se o alvo está dentro do alcance do ataque.

### <span class="icon"></span> Arqueado

TODO

No calculo de alcance deve se adicionar/subtrair a altura do alvo e do atacante.

### <span class="icon"></span> Área

TODO

Uma área ao redor do usuário. Não confundir com explosivos.

---

## TERRENO (TODO)

---
