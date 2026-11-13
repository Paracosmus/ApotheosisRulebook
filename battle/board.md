!!!danger
Esta seção ainda não foi completamente revisada. Algumas informações podem estar desatualizadas ou incompletas, e a formatação pode não estar finalizada.
!!!
    
# Tabuleiro

É a área quadriculada especificamente onde as batalhas entre os personagens ocorrem.

---

## Tamanho

Cada tabuleiro tem o seu próprio tamanho: um número de colunas por um número de linhas de casas.

## Casa Adjacente

## Casa Ocupada

Uma casa comporta apenas uma peça. Duas peças nunca podem estar na mesma casa, e nenhum efeito pode mudar isso.

## Casa de Posicionamento

São as casas onde as peças são colocadas no início da batalha.

## Casa de Reforço

São as casas por onde os personagens chamados durante uma batalha em andamento, como um [<span class="companion"><b>COMPANHEIRO</b></span>](/cards/companion.md) recrutado, entram no tabuleiro.

As demais casas não permitem que nenhuma peça entre no tabuleiro por elas.

## Direção do Ataque

## Camadas

Toda casa tem pelo menos uma <b>CAMADA</b>, e pode ter outras empilhadas sobre ela, como o chão e uma ponte acima dele. Cada <b>CAMADA</b> tem a sua própria <b>ALTITUDE</b> e o seu próprio [terreno](#terreno), e pode ter uma <b>PAREDE</b> em cada um dos seus lados.

Uma peça fica sempre na <b>CAMADA</b> mais alta da casa. Toda <b>CAMADA</b> abaixo dela serve apenas de passagem: uma peça pode passar por ela ou atirar através dela, mas não pode parar nela, como no chão sob uma ponte.

Por padrão, uma casa tem uma única <b>CAMADA</b>, no nível do solo, de terreno **Plano** e sem <b>PAREDE</b>.

## Altitude

Toda <b>CAMADA</b> de uma casa tem uma <b>ALTITUDE</b>, a sua altura em relação ao nível do solo, onde **1** de <b>ALTITUDE</b> equivale a cerca de **1** metro. O nível do solo é **0**: o que está abaixo dele tem <b>ALTITUDE</b> negativa, como um fosso, e o que está acima tem <b>ALTITUDE</b> positiva, como um telhado.

## Teto

Uma casa pode ter um <b>TETO</b>. A altura do <b>TETO</b> é medida em <b>ALTITUDE</b> a partir do chão da casa, a sua <b>CAMADA</b> mais alta, e não a partir do nível do solo. Uma casa sem <b>TETO</b> fica a céu aberto.

!!!
Por exemplo, em uma casa de <b>ALTITUDE</b> **4** com <b>TETO</b> **2**, o <b>TETO</b> fica na <b>ALTITUDE</b> **6**.
!!!

## Paredes

Uma <b>PAREDE</b> fica em um dos quatro lados de uma <b>CAMADA</b>, e impede que uma peça naquela <b>CAMADA</b> saia da casa ou interaja por aquele lado.

A <b>PAREDE</b> só impede a saída da casa onde ela está. Para fechar a passagem nos dois sentidos, as duas casas vizinhas têm uma <b>PAREDE</b> no lado que dividem. Uma <b>PAREDE</b> em apenas uma delas é uma passagem de mão única.

!!!
Por exemplo, se uma casa tem uma <b>PAREDE</b> no lado oeste e a casa a oeste dela não tem <b>PAREDE</b> no lado leste, uma peça pode entrar na casa vindo do oeste, mas não pode sair dela pelo oeste.
!!!

Uma <b>PAREDE</b> bloqueia toda ação por aquele lado, não apenas o movimento e o ataque: uma peça também não pode, por exemplo, interagir com um baú ou um contêiner do outro lado dela. A única exceção é o ataque <b>ARQUEADO</b>, que passa por cima da <b>PAREDE</b>, a não ser que um <b>TETO</b> o impeça.

## Trajetória

Quando a trajetória de uma ação passa exatamente pela quina entre duas casas, as duas casas fazem parte dela. Se qualquer uma das duas bloquear a trajetória, ela fica bloqueada.

## Gimmicks

### Escada

### Rampa

### Portal

### Névoa de Guerra

## Mover

Ao se mover, uma peça pode passar por uma [casa ocupada](#casa-ocupada), mas não pode terminar o movimento nela. É a mesma regra das [camadas](#camadas) inferiores de uma casa: a peça passa por elas, mas não para nelas.

!!!
Por exemplo, uma peça pode atravessar a casa onde está outra peça para chegar à casa seguinte, mas não pode parar na casa da outra peça.
!!!

## Terreno

Toda <b>CAMADA</b> de uma casa tem um tipo de terreno. Por padrão, uma <b>CAMADA</b> é de terreno **Plano**.

* ⬜ Plano _(padrão)_
* 🌾 Campo
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
