---
label: Batalha
icon: flame
order: 96
---
{{ review() }}

# Batalha

A batalha acontece em um tabuleiro quadriculado. O tabuleiro pode conter paredes ou casas com diferentes níveis de altura. Cada casa possui um tipo de [terreno](/battle/board.md#terreno).

---

## AÇÕES

No seu turno, o personagem pode executar uma variedade de ações. As ações geralmente possuem algum custo de {{ ap }}. Quando o personagem realizar ações até esgotar a sua {{ ap }}, o seu turno se encerra. Alguns tipos de ações podem ter custos associados como {{ mp }} e {{ sp }}.

### MOVER

Em seu turno, o personagem pode se mover no tabuleiro. Por padrão, o custo para mover é de 1 de {{ ap }} por casa. Alguns terrenos podem ter regras específicas para mover, por exemplo em um terreno de lama pode custar 2 de {{ ap }} por casa.

Pode-se mover para casas adjacentes com {{ alt }} diferente, pagando-se 1 {{ ap }} a mais para cada nível a mais de altura.

Quando terminar de mover, o personagem fica na direção em que se moveu até a casa de destino.

Adjacente
Distância
Casas

---

## DIREÇÃO (TODO)

---

## ÁREA DE INFLUÊNCIA
Todo personagem possui uma área de influência sobre o tabuleiro, que são as casas adjacentes à sua peça no tabuleiro, com exceção da casa atrás da peça em relação à sua orientação.

A área de influência aumenta em 1 de {{ ap }} o custo para que um personagem inimigo possa se mover para ela. Caso uma casa do tabuleiro esteja na área de influência de 2 ou mais personagens, o custo para se mover para esta casa aumenta em 1 de {{ ap }} para cada personagem inimigo.

---

## DESCANSAR
O personagem pode realizar uma Ação Total para:

* Curar {{ p'10' }} de {{ hp }}; e

* Recuperar {{ p'2' }} de **Energia** ({{ sp }} e/ou {{ mp }}).

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
| <span class="hse"></span> {{ str }} + <span>{{ d1d2 }}</span> | <span class="hse"></span> 1 | <span class="hse"></span> 3 |

:::

É o ataque padrão que todo personagem pode realizar, sem a necessidade de cartas ou recursos.

Ao custo de 3 de {{ ap }} o personagem pode realizar um ataque {{ direct }} de 1 de {{ range }}, com {{ dmg }} igual a ( {{ str }} + {{ d1d2 }} ).

Este ataque não possui propriedades ou efeitos, é o mais simples e direto que um ataque pode ser.

---

## USAR UMA CARTA

Você pode utilizar uma carta conforme as regras durante a batalha. Você pode utilizar uma HABILIDADE pagando os seus custos. Você pode utilizar uma FERRAMENTA para atacar. Você pode enviar uma carta do {{ inv }} para a {{ table }} ou enviar uma carta da {{ table }} para o {{ inv }}, pagando os custos de {{ ap }}.

---

## Dano

Todo ataque causa uma quantidade de {{ dmg }} ao alvo. Desse {{ dmg }} sofrido, subtrai-se a defesa do alvo — isto é, todos os descontos e reduções que o alvo aplica ao {{ dmg }} recebido. O resultado final é a {{ injury }}, que corresponde à quantidade de {{ hp }} que o personagem perde, calculada observando os seguintes passos:

* +1 de {{ injury }} se o {{ dmg }} for maior ou igual à metade da {{ enr }} do alvo
* +1 de {{ injury }} se o {{ dmg }} for maior ou igual à {{ enr }} do alvo
* +1 de {{ injury }} para cada 5 pontos que o {{ dmg }} for maior que a {{ enr }} do alvo

!!!info
Por exemplo, se um alvo tem <u>_6 de {{ enr }}_</u> e recebe um ataque de <u>_18 de {{ dmg }}_</u>, o alvo sofre <u>_4 de {{ injury }}_</u>. O cálculo é feito da seguinte forma:

* +1 de {{ injury }} por ter sofrido um ataque maior ou igual a ( {{ enr }} / 2 ) → (18 ≥ 6 / 2)
* +1 de {{ injury }} por ter sofrido um ataque maior ou igual à {{ enr }} → (18 ≥ 6)
* +1 de {{ injury }} por ter sofrido um ataque 5 pontos maior que a {{ enr }} → (18 ≥ 11)
* +1 de {{ injury }} por ter sofrido um ataque 10 pontos maior que a {{ enr }} → (18 ≥ 16)


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

Observando a equação acima, note que quando o {{ dmg }} for menor que a metade da {{ enr }} do alvo, o ataque falha e não causa {{ injury }}. Neste caso é considerado que o atacante errou o ataque, que pode ser por diversos motivos, como o alvo se esquivou, se defendeu ou o ataque não atingiu o alvo.

### Rolagem Perfeita

Quando o {{ dmg }} de um ataque incluir a rolagem de dados, aplica-se a regra de [rolagem perfeita](/gameplay/die.md#dados-extras-rolagem-perfeita) ao dado principal da rolagem, somando o resultado dos dados extras ao {{ dmg }} do ataque.

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

No cálculo de alcance deve-se adicionar/subtrair a altura do alvo e do atacante.

### <span class="icon"></span> Área

TODO

Uma área ao redor do usuário. Não confundir com explosivos.

---

## TERRENO (TODO)

---



- [ ]  Explicar o que é um ataque. É a ação de ataque normal ou a ativação de uma carta que possui um dano na sua barra de ação. Um dano causado pelo efeito de uma carta não é um ataque, assim como quando você recebe dano de explosivo, apenas o tile alvo que foi atacado
- [ ]  Explicar a diferença de sofrer dano, lesão e perder vida