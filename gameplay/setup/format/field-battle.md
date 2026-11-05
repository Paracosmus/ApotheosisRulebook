---
label: Batalha Campal
icon: square-fill
---
{{ review() }}

## Batalha Campal

É um formato de batalha onde os jogadores se enfrentam em um campo de batalha terrestre, com regras específicas para o combate e a movimentação, na intenção de simular uma batalha em grande escala entre exércitos.

## Governo Monárquico

O governo da resistência precisa ser administrado, para isso são usados **Poder**, uma pontuação equivalente ao ( número de províncias controladas - 1 );

|
| --- | --- | --- | --- |
| **Poder** | Representa a quantidade de pessoas ao seu lado e seu poder de convencimento geral | O número de milícias recrutadas a cada rotação. | Representado pelo número de {{ counter }} na carta de {{ class }} no {{ support }} do Exército |

E **Recursos**, uma moeda de troca usada para comprar tropas, melhorias, entre outros;

|
| --- | --- |
| 💰 **Dinheiro** | Representado pelo número de {{ counter }} na carta de **Muito Papel Moeda** no {{ support }} do Exército |
| 🍊 **Alimentos** | Representado pelo número de {{ counter }} na carta de **Banquete** no {{ support }} do Exército |
| 🪨 **Metais** | Representado pelo número de {{ counter }} na carta de **Postura Defensiva** no {{ support }} do Exército |

## Diplomacia

Nenhum governo consegue se manter sozinho, por isso é necessário manter uma boa relação com seus vizinhos e criar alianças. A diplomacia é o painel de relação com as outras cidades estados relevantes para o conflito.

O exército da resistência pode ter um aliado para cada ponto de **Poder** que possuir. Se perderem **Poder**, a última aliança feita é desfeita.

**Alianças**

|
| --- | --- | --- | --- |
| **Carrefour** | *Comercial* | **+1** de 💰 por rotação | Podem se aliar a ambos os lados |
| **Ultramar** | *Produtiva* | **+1** de 🪨 por rotação |  |
| **~~Akka~~** | *Religiosa* | **+1** de 🍊 por rotação | Não pode ser aliado pois estão sob controle da Ordem do Caos e já são aliados dos republicanos |
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

O exército é dividido em batalhões, cada um fica em uma província.

### Mudança

Na fase de rotação, os jogadores podem mover unidades à sua escolha, de uma província para uma outra adjacente.

- Se a província adjacente for aliada, as tropas apenas se mudam.
- Se a província adjacente for inimiga, tem início uma batalha campal.
    - Quando uma batalha campal é declarada, as tropas daquela província enfrentam as tropas invasoras designadas.

### Batalha

A batalha campal segue as mesmas regras de um combate entre {{ companion }}. Respeitando pontos de {{ ap }}, regras de movimento, cálculo de distância, {{ alt }}, adjacência, etc.

Porém, apenas {{ companion }} com a propriedade **Unidade** podem participar.

<aside>

Adicionalmente, unidades possuem orientação, e sofrem bônus de ataque quando atacadas pelas costas e flancos.

- **Retaguarda** **→** **+4** de {{ dmg }}
- **Flancos** → **+2** de {{ dmg }}
</aside>

<aside>

A {{ hp }} da unidade representa a sua Moral, ou seja, quando a {{ hp }} de tropa acaba, isso não significa que ela foi completamente dizimada, mas sim que ela dispersou ou debandou mediante a situação de vida ou morte.

Uma unidade só é exterminada em caso de Perda Total.

</aside>

### **Unidades**

Cada unidade representa uma tropa ou pelotão daquele exército, tendo técnicas e atributos usados conforme regras normais.

Porém, técnicas que requerem anexos, devem ser garantidas anexando as respectivas cartas de recursos ao remover um {{ counter }} do marcador do exército.

- {{ item }} → Dinheiro → Muito Papel Moeda
- {{ event }} → Alimentos → Banquete
- {{ skill }} → Metal → Postura Defensiva

|
| --- | --- | --- |
| {{ enr }} | MORAL | Define a quantidade de {{ hp }} |
| {{ str }} | {{ dmg }} | {{ dmg }} causado em ataques normais |
| {{ agi }} | DESLOCAMENTO | Equivalente à {{ ap }} nas regras padrão |
| {{ per }} | {{ range }} | {{ dmg }} causado em ataques à distância |
| {{ int }} | EXPERIÊNCIA MÁXIMA | Número máximo de contadores de Experiência que esta carta pode ter |
| {{ cha }} | CONFIANÇA | Valor de Moral recuperado quando uma unidade inimiga é debandada |
| {{ spt }} | DANO ESPECIAL | Usado para definir o {{ dmg }} de técnicas como magias e explosivos |

### Experiência

Unidades ganham experiência de combate. Ao final de uma batalha, todas as unidades vivas recebem **+1** {{ counter }} na sua respectiva carta (**max igual à {{ int }}**). O valor desse {{ counter }} deve ser somado ao valor de qualquer rolagem de dado feita por esta unidade, seja ele proposto por um ataque, teste, ou técnica.

### Melhorias

Cada unidade pode ter até **3** melhorias que podem ser compradas para ela. Adicione o ícone de {{ marker }} para representar.

| **Nome** | **Marcador** | **Preço** | **Efeito** |
| --- | --- | --- | --- |
| **Marchar** | *Triângulo* | 🍊🍊 | +1 de Deslocamento |
| **Formação**  | *Quadrado* | 🪨🪨 | Esta unidade e unidades aliadas adjacentes sofrem -2 de {{ dmg }} (não cumulativo) |
| **Entrincheirar**  | *Escudo* | 🪨 | Sofre -3 de {{ dmg }} se não se mover nesse ciclo |
| **Inspirar**  | *Encantamento* | 💰💰 | +10 de CONFIANÇA |
| **Disciplina** | *Coração* | 💰💰🍊 | +2 de MORAL (20 de {{ hp }}) |
| **Flanquear** | *Seta* | 💰🪨 | +2 de {{ dmg }} quando atacando pelos flancos ou retaguarda |
| **Treinamento**  | *Impacto* | 🪨 | +2 de EXPERIÊNCIA MÁXIMA |
| **Escaramuça**  | *Mira* | 💰💰🍊 | +1 de {{ range }} |
| **Reagrupar**  | *Circulo* | 🪨🪨 🍊🍊 | Uma vez por batalha, se debandada por falta de Moral, eles voltam na próxima {{ resetPhase }} com 10 de {{ hp }} |

!!!
Mercenários não podem receber melhorias.
!!!

### Oficial Comandante

Cada Herói pode se juntar a uma unidade como seu oficial comandante, fornecendo um bônus extra.

Se a unidade de um comandante morrer, ele pode assumir outra unidade na próxima {{ resetPhase }}.

|
| --- | --- | --- |
| **Marechal** | Comandante       | +1 de Moral (10 de {{ hp }}) |
| **Caleb**    | *Estrategista*   | Sua unidade recebe +1 {{ counter }} de EXP ao final da batalha |
| **Drako**    | *Artilheiro*     | +{{ d1d3 }} de {{ dmg }} |
| **Hércules** | *Batedor*        | +1 de DESLOCAMENTO |
| **Carlos**   | *Defensor*       | -2 sofrido de Ataques |
| **Ryan**     | *Ponta de Lança* | +3 de {{ dmg }} quando sem aliados adjacentes |
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
