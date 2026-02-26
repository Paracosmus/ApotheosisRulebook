---
label: Batalha Campal
icon: project
order: 9
---
{{ review() }}

## Batalha Campal

É um formato de batalha onde os jogadores se enfrentam em um campo de batalha terrestre, com regras específicas para o combate e a movimentação, na intensão de simular uma batalha em grande escala entre exércitos.

## Governo Monárquico

O governo da resistência precisa ser administrado, para isso são usados **Poder**, uma pontuação equivalente ao ( número de províncias controladas - 1 );

|
| --- | --- | --- | --- |
| **Poder** | Representa a quantidade de pessoas ao seu lado e seu poder de convencimento geral | O número de milícias recrutadas a cada rotação. | Representado pelo número de contadores na carta de classe no suporte do Exército |

E **Recursos**, uma moeda de troca usada para comprar tropas, melhorias, entre outros;

| 
| --- | --- |
| 💰 **Dinheiro** | Representado pelo número de contadores na carta de **Muito Papel Moeda** no suporte do Exército |
| 🍊 **Alimentos** | Representado pelo número de contadores na carta de **Banquete** no suporte do Exército |
| 🪨 **Metais** | Representado pelo número de contadores na carta de **Postura Defensiva** no suporte do Exército |

## Diplomacia

Nenhum governo consegue se manter sozinho, por isso é necessário manter uma boa relação com seus vizinhos e criar alianças. A diplomacia é o painel de relação com as outras cidades estados relevantes para o conflito.

O exércitos da resistência pode ter um aliado para cada ponto de **Poder** que possuir. Se perderem **Poder**, a última aliança feita é desfeita.

**Alianças**

|
| --- | --- | --- | --- |
| **Carrefour** | *Comercial* | **+1** de 💰 por rotação | Podem se aliar a ambos os lados |
| **Ultramar** | *Produtiva* | **+1** de 🪨 por rotação |  |
| **~~Akka~~** | *Religiosa* | **+1** de 🍊 por rotação | Não pode ser aliado pois estão sobre controle da Ordem do Caos e já são aliados dos republicanos |
| **Babel** | *Conveniência* | Tropas Mercenárias | Podem ser usados por ambos os lados |

É possível trocar recursos por tropas se você se aliar a Babel;

| Samurais | *Infantaria* | **3** de 🪨 |
| --- | --- | --- |
| Arqueiros Longos | *Artilharia* | **3** de 💰 |
| Horda | *Cavalaria* | **3** de 🍊 |
| Dragoons | *Misto* | **2** de 💰, 🍊 e 🪨  |

## Províncias

| {.compact}
| --- | --- | --- | --- |
| **Vale do Amanhecer** | Base de Operações dos Monarquistas.<br>Se conquistada, acabou<br>Ao final de todas as batalhas de uma rotação. Adicione unidades *Legionários* ao Vale do Amanhecer até que você tenha 2 Legionários totais no exército  | 💰🍊🪨 |
| **Vilarejos** | **+1** Milícia por rotação | 🍊🪨 |
| **Serra** | Se tiver uma única tropa aqui, ela não pode ser reconquistada pelos republicanos | 🪨🪨🪨 |
| **Campos** | Quando conquistada pela primeira vez, compre **3** melhorias de unidade sem pagar os custos associados em 🍊 | 🍊🍊🍊 |
| **Mata** | Se você não tiver nenhuma tropa de arquearia:<br>**1** arqueiro<br>*(não precisa ser aliado de babel)* | 💰🍊 |
| **Periferia** | **+1** aliado | 💰💰 |
| **Centro** | **+1** de **Poder** | 💰💰💰🍊🍊🪨🪨 |
| **Ninho da Fênix** | Base de operações dos Republicanos.<br>Se conquistada, acabou<br>**+1** *Legionário* por rotação | 💰🍊🪨 |

## Exército

O exército é divido em batalhões, cada um fica em uma província.

### Mudança

Na fase de rotação, os jogadores podem mover unidades a suas escolhas, de um província para uma outra adjacente.

- Se a província adjacente for aliada, as tropas apenas se mudam.
- Se a província adjacente for inimiga, tem início uma batalha campal.
    - Quando uma batalha campal é declarada, as tropas daquela província enfrentam as tropas invasoras designadas.

### Batalha

A batalha campal segue as mesmas regras de um combate entre [Companion](https://www.notion.so/Companion-27083fd0169e8001a3c9fbac0d8a3684?pvs=21). Respeitando pontos de ação, regras de movimento, calculo de distância, altura, adjacência, etc.

Porém, apenas [Companion](https://www.notion.so/Companion-27083fd0169e8001a3c9fbac0d8a3684?pvs=21) com a propriedade **Unidade** podem participar.

<aside>

Adicionalmente, unidades possuem orientação, e sofrem bônus de ataque quanto atacadas pelas costas e flancos.

- **Retaguarda** **→** **+4** de Dano
- **Flancos** → **+2** de Dano
</aside>

<aside>

A Vida da unidade representa a sua Moral, ou seja, quando a vida de tropa acaba, isso não significa que ela foi completamente dizimada, mas sim que ela dispersou ou debandou mediante a situação de vida ou morte.

Uma unidade só é exterminada em caso de Perda Total.

</aside>

### **Unidades**

Cada unidade representa uma tropa ou pelotão daquele exército, tendo técnicas e atributos usados conforme regras normais.

Porém, técnicas que requerem anexos, devem ser garantidas anexando as respectivas cartas de recursos ao remover um contador do marcador do exército.

- Item → Dinheiro → Muito Papel Moeda
- Evento → Alimentos → Banquete
- Habilidade → Metal → Postura Defensiva

|
| --- | --- | --- |
| **CON** | MORAL | Define a quantidade de Vida |
| **FOR** | DANO | Dano causando em ataques normais |
| **AGI** | DESLOCAMENTO | Equivalente à AÇÃO nas regras padrão |
| **PER** | ALCANCE | Dano causando em ataques à distância |
| **INT** | EXPERIÊNCIA MÁXIMA | Número máximo de contadores de Experiência que esta carta pode ter |
| **CAR** | CONFIANÇA | Valor de Moral recuperado quando uma unidade inimiga é debandada |
| **ESP** | DANO ESPECIAL | Usado para definir o dano de técnicas domo magias e explosivos |

### Experiência

Unidades ganham experiência de combate. Ao final de uma batalha, todas as unidades vivas recebem **+1** contador na sua respectiva carta (**max igual à INT**). O valor desse contador deve ser somado ao valor de qualquer rolagem de dado feita por esta unidades, seja ele proposto por um ataque, teste, ou técnica.

### Melhorias

Cada unidade pode ter até **3** melhorias que podem ser compradas para ela. Adicione o ícone de marcador para representar.

| **Nome** | **Marcador** | **Preço** | **Efeito** |
| --- | --- | --- | --- |
| **Marchar** | *Triângulo* | 🍊🍊 | +1 de Deslocamento |
| **Formação**  | *Quadrado* | 🪨🪨 | Esta unidade e unidades aliadas adjacentes sofrem -2 de DANO (não cumulativo) |
| **Entrincheirar**  | *Escudo* | 🪨 | Sofre -3 de DANO se não se mover nesse ciclo |
| **Inspirar**  | *Encantamento* | 💰💰 | +10 de CONFIANÇA |
| **Disciplina** | *Coração* | 💰💰🍊 | +2 de MORAL (20 de HP) |
| **Flanquear** | *Seta* | 💰🪨 | +2 de DANO quando atacando pelos flancos ou retaguarda |
| **Treinamento**  | *Impacto* | 🪨 | +2 de EXPERIÊNCIA MÁXIMA |
| **Escaramuça**  | *Mira* | 💰💰🍊 | +1 de ALCANCE |
| **Reagrupar**  | *Circulo* | 🪨🪨 🍊🍊 | Uma vez por batalha, se debandada por falta de Moral, eles voltam na próxima fase de restauração com 10 de VIDA |

!!!
Mercenários não podem receber melhorias.
!!!

### Oficial Comandante

Cada Herói pode se juntar a uma unidade como seu oficial comandante, fornecendo um bônus extra.

Se a unidade de um comandante morrer, ele pode assumir outra unidade na próxima fase de restauração.

|
| --- | --- | --- |
| **Marechal** | Comandante       | +1 de Moral (10 de HP) |
| **Caleb**    | *Estrategista*   | Sua unidade recebe +1 contadores de EXP ao final da batalha |
| **Drako**    | *Artilheiro*     | +1d3 de DANO |
| **Hércules** | *Batedor*        | +1 de DESLOCAMENTO |
| **Carlos**   | *Defensor*       | -2 sofrido de Ataques |
| **Ryan**     | *Ponta de Lança* | +3 de DANO quando sem aliados adjacentes |
| **von**      | *Inspiração*     | Unidades recuperam o dobro de moral ao eliminar unidades inimigas |

### Promoção

Para recrutar uma unidade nova, o jogador deve promover uma milícia, lhe fornecendo treinamento adequado.

||| Preço de promoção

| {.compact}
| --- | --- |
| **Homens-de-Armas** | 🍊🪨 |
| **Lanceiros** | 💰🍊 |
| **Arqueiros** | 💰🪨 |
| **Rifleiros** | 💰🍊🪨 |
| **Canhões** | 💰💰🪨 |
| **Cavalaria Leve** | 💰🍊🪨 |
| **Cavalaria Arqueira** | 💰🍊🍊 |
| **Cavalaria Pesada** | 🍊🪨🪨 |

||| Quantidade de soldados aproximada por unidade

| {.compact}
| --- | --- |
| **Infantaria** | 100 homens |
| **Cavalaria** | 50 homens |
| **Artilharia** | 25 homens |

||| 

---

Acampamento de campanha

+25 de vida

+6 de energia

---
