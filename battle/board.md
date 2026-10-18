---
label: Tabuleiro
icon: apps
order: 100
---
{{ review() }}

# Tabuleiro

é a área quadriculada especificamente onde as batalhas entre os personagens ocorrem.

---

## Casa Adjacente

## Casa de Posicionamento

São as casas onde as peças são colocadas no início da batalha.

## Casa de Reforço

São as casas por onde os personagens chamados durante uma batalha em andamento, como um {{ companion }} recrutado, entram no tabuleiro.

As demais casas não permitem que nenhuma peça entre no tabuleiro por elas.

## Direção do Ataque

## Altitude

Toda casa do tabuleiro tem uma {{ alt }}, a sua altura em relação ao nível do solo, onde **1** de {{ alt }} equivale a cerca de **1** metro. O nível do solo é **0**: o que está abaixo dele tem {{ alt }} negativa, como um fosso, e o que está acima tem {{ alt }} positiva, como um telhado.

## Distância

## Mover

## Terreno

Toda casa do tabuleiro tem um tipo de terreno. Por padrão, uma casa é de terreno **Plano**. Além dele, apenas a **Água** está definida; os demais terrenos ainda estão em desenvolvimento:

* ⬜ Plano _(padrão)_
* 🌾 Campo _(grama)_
* ⛰️ Rocha
* 🌿 Pântano
* 🌵 Areia
* ⛄ Gelo
* ❄️ Gelo Prateado
* 💧 Água
* 🟫 Terra
* 🟤 Lama

---





Tiles podem receber estados

Blocked/Ocupado

Void/Denied

Domain area stacked or not

Tiles podem ter efeitos

Apply an effect descrito na carta que adicionou aquele estado. Pode ser ao entrar, ao sair, no início do turno, enfim qualquer coisa que uma carta possa fazer

Seria interessante usar a ilustração da carta que aplicou o efeito, no tiles, tipo uma armadilha ou toxic spikes teria a imagem da carta no cover do tiles, e se for full art teria que ter um token

Tiles tem terrenos

Agua

Field

Etc.

Tiles podem ter peças nele. Mas apenas uma peça por tile. Portanto o Encero precisa ser reescrito e o nuvero eu acho

Os tamanhos mais comuns utilizados de tabuleiro são

- **Battlefield** 11x11 (max size) [quadrado]
- **Chess** 8x8 (Easy to find) [quadrado]
- **Court** 5x7
- **Plaza** 5x5 [quadrado]
- **Skirmish** 3x4 (para PvP simples)
- **Arena** 3x3 [quadrado]
- **Clash** 3x2 (para PvP rápido e descomplicado)
- **Lane** 2x4
- **Pit** 1x2