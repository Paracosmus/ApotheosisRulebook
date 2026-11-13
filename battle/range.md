---
label: Alcance
icon: 
order: 75
---
{{ review() }}

# Alcance

{{ briefing `Range` `É a distância, contada usando as casas do tabuleiro e suas características, entre quem realiza uma ação e o seu alvo, e a forma como a ação chega até ele.` }}

O alcance é utilizado mais comumente no tabuleiro, para calcular a distância de uma casa do tabuleiro para outra.

Ele determina se uma ação pode atingir um alvo, se um movimento de determinada distância pode ser percorrido e influencia a forma como a ação se propaga pelo tabuleiro.

Existem quatro formas distintas de calcular o alcance de uma ação, cada uma representa uma ideia narrativa de como aquela ação se propaga até o seu alvo.

- Indiferente ao tipo de ação, o alcance sempre é contado usando as casas do tabuleiro e alguns deles podem ser afetados por obstáculos ou características de cada casa.
- A casa de onde a ação se origina, geralmente aquela onde o personagem que executa a ação está localizado, é considerado como distância zero, e portanto, está sempre dentro do alcance, podendo o personagem sempre selecionar a si mesmo como alvo.
- Casas na diagonal não são contadas como adjacentes, sendo necessário percorrer as casas ortogonais para alcançar uma casa diagonal.

---

## <span class="icon"></span> Contato [!badge text="Melee" variant="ghost"]

> São ações físicas de interação de toque contra o alvo, como toca, empurrar golpear com uma arma branca, entre outros.

**Diferença de Altura:** Verifique a diferença de altura entre a casa de origem e a casa de destino.
- Se estiver em uma casa mais alta, você ganha 1 de alcance.
- Se estiver em uma casa mais baixa, você perde 1 de alcance.

**Distância Horizontal:** Conte a distância horizontal entre a casa de origem e a casa de destino.

**Obstáculos:** Verifique se há obstáculos entre a casa de origem e a casa de destino. Se houver o alvo não pode ser atingido.

Se o alvo estiver em uma casa adjacente, ele está sempre dentro do alcance desde que não esteja a uma altura maior que o valor natural do alcance da arma.

---

## <span class="icon"></span> Direto [!badge text="Direct" variant="ghost"]

> São ações de disparo que atingem o alvo de forma direta, sem se desviar ou contornar obstáculos, como disparos de armas de fogo ou magias de projétil.

**Diferença de Altura:** Verifique a diferença de altura entre a casa de origem e a casa de destino e adicione este valor à contagem de alcance.
- Se você estiver em uma casa mais alta, você ganha alcance.
- Se você estiver em uma casa mais baixa, você perde alcance.

**Distância Horizontal:** Conte a distância horizontal entre a casa de origem e a casa de destino.

**Obstáculos:** Verifique se há obstáculos entre a casa de origem e a casa de destino. Se houver o alvo não pode ser atingido.

---

## <span class="icon"></span> Arqueado [!badge text="Arcing" variant="ghost"]

> São ações de disparo que atingem o alvo contornando obstáculos ou seguindo uma trajetória curva, como arcos, magias perseguidoras, entre outros.

**Diferença de Altura:** Verifique a diferença de altura entre a casa de origem e a casa de destino e adicione este valor à contagem de alcance.
- Se você estiver em uma casa mais alta, você ganha alcance.
- Se você estiver em uma casa mais baixa, você perde alcance.

**Distância Horizontal:** Conte a distância horizontal entre a casa de origem e a casa de destino.

**Obstáculos:** Obstáculos com diferença de altura maior que 3 bloqueiam o alcance. Paredes que sobem até o teto também bloqueiam o alcance. Teto sobre a linha de disparo também bloqueia o alcance.

---

## <span class="icon"></span> Área [!badge text="Area" variant="ghost"]

> São ações que afetam uma área ao redor do usuário, podendo atingir múltiplos alvos simultaneamente, como explosões, magias de área, sons, ou ataques em cone.

**Diferença de Altura:** Ignorada.

**Distância por Horizontal:** Conte por adjacência, para todos os lados, as casas que compõem a área de efeito, considerando a casa de origem como distância zero.

**Obstáculos:** devem ser contornadas.

---
