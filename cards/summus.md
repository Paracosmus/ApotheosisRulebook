---
label: Summus
icon: "../static/img/icons/suit_summus.svg"
order: 0
---

# SUMMUS

Summus são as cartas que possuem os efeitos mais poderosos no jogo. De forma resumida, Summus é uma mecânica extra, que é adicionado a uma carta, conferindo novas capacidades e efeitos a ela, bem como adicionando regras específicas para sua utilização.

Uma carta {{ summus }} pode ser identificada por suas 3 características distintas:

- O ícone do naipe tem sua cor modificada para magenta.
- Raridade {{ rare }} ou superior, e *full-art*.
- Cartas de nível 3 (Exceto quando cartas de {{ house }})
- A presença de uma caixa identificadora do tipo de Summus, abaixo ou acima do texto do efeito da carta, contendo informações adicionais referentes à sua mecânica extra.

---

## Mecânica Básica

Indiferente do tipo de Summus, elas compartilham as seguintes regras de jogo.

**Restrição de Nível**
:   O Herói precisa ter nível 6✚

**Limite de Cartas**
:   Cada Herói pode ter apenas uma carta de cada tipo de Summus e apenas 3 cartas de Summus no total (including MESA, INVENTÁRIO e Anexos)

**Espaço**
:   Não ocupam um espaço na **MESA**
    - Quando cartas de Ficha, elas são adicionadas a *Zona Extra* da **FICHA**
    - Quando cartas de Recurso, elas são adicionadas as suas respectivas zonas da **MESA** conforme naipe, porém não ocupam um espaço de carta naquela zona

---

## Mecânica Adicional

A mecânica adicionada por uma carta Summus é definida pelo seu tipo, e pode ser encontrada na lista a seguir.

<br>


==- <span class="summus"> Ultimatum</span>
> Ultimatum é o termo latino para "último", e refere-se a uma ação final ou definitiva.
> 
> O Ultimatum de um Herói é sua habilidade mais poderosa e definitiva, que quando carregada e pronta, pode mudar o rumo da batalha.

Ultimatums são cartas de **HABILIDADE**, focados em causar uma enorme quantidade de **DANO** em um único ataque, e/ou em causar um efeito devastador na mesa do oponente ou no tabuleiro.

São as Summus mais simples de serem utilizadas e ativadas, o que as torna bastante versáteis e compatíveis com diversas **MESAS**.

<br>

#### Regras Especiais

- No início e no fim da Batalha, remova todos os {{ counter_ultimate }} desta carta.
- No início de cada rodada de batalha, adicione um {{ counter_ultimate }} a esta carta.
- Quando esta carta possuir a quantidade mínima de {{ counter_ultimate }}, você pode ativar esta carta.
- Não possuem custo em {{ ap }}, pois para ativá-la você deve realizar uma *Ação Total*.
- Remova todos os {{ counter_ultimate }} desta carta após ativá-la.
- Nenhuma carta pode ser ativada em resposta a esta ativação.
- Cada Herói pode ativar apenas um Ultimatum por batalha.

<br>

||| Caixa de Mecânica
![Exemplo](/static/img/summus/ultimatum.png)

- <span class="summus"></span>: Número de {{ counter_ultimate }} necessários para ativar a carta.
- *Texto*: Instruções adicionais de uso e ativação da carta.
|||
===



==- <span class="summus"> Collegium</span>
> Collegium é o termo latino para "associação", e refere-se a um grupo de pessoas unidas.
> 
> O Collegium de um Herói é a egrégora da qual ele faz parte (religiosa, profissional, política), conceito que geralmente descreve uma consciência coletiva formada pelo pensamento ou energia de um grupo, e que concede poderes adicionais aos iniciados. Como membro da egrégora, o personagem fornece e recebe energia do coletivo.
> 
> Por este motivo são representados por cartas de CASA, que são o berço, herança e legado do Herói.

Collegiums são cartas de {{ house }} adicionadas na área extra da {{ sheet }}, conferindo efeitos adicionais ao Herói quando pago o *"preço"* cobrado por aquele coletivo de energias.

A ilustração da carta representa o *frater* ou *soror* daquela egrégora.

<br>

#### Regras Especiais

- Para adicionar uma carta Collegium da {{ tavern }} para um espaço extra na sua {{ sheet }}, o Herói deve **banir** uma carta com a propriedade ** INICIAÇÃO**.
- Adicione os bônus de atributos desta carta ao total do Herói, mesmo que ela esteja consumida. (Esta carta não concede espaços na {{ table }})
- No início e no fim da Batalha, ou ao mudar o período do dia, consuma esta carta.
- A qualquer momento do seu turno, você pode pagar os custos referidos na caixa de Mecânica para recuperar esta carta.
- Quando consumida, esta carta não tem efeito. Quando recuperada, o efeito dessa carta deve ser considerado, estando disponível para ser utilizado.
- Você pode descartar esta carta a qualquer momento do seu turno.

<br>

||| Caixa de Mecânica
![Exemplo](/static/img/summus/collegium.png)

- _Texto_: Custo para recuperar esta carta.
|||
===



==- <span class="summus"> Dominium</span>
> Dominium é o termo latino para “domínio”, no sentido de posse, território, propriedade.
> 
> O Dominium é uma dimensão forjada pela vontade do seu criador a sua imagem e semelhança. É uma zona interdimensional que quando ativada, se entrelaça com o espaço-tempo ao redor do seu conjurador criando uma área no local, com regras e características próprias, definidas pela mente e magia do seu criador, e onde ele é deus.
> 
> Por este motivo, são representados por cartas de {{ event }} no {{ scenario }}, aplicando seus efeitos a todos.

Dominiums são cartas de {{ event }} que quando ativadas do {{ inv }} são enviadas para o {{ scenario }} para aplicar efeitos a todos os personagens.

<br>

#### Regras Especiais

- Para ativar um Dominium do seu {{ inv }} o Herói deve consumir **10** de **Energia** e então enviar a carta para o {{ scenario }}.
    - Apenas um Dominium pode estar ativo por vez, portando não é possível ativar um Dominium se já houver outro no {{ scenario }}.
- Enquanto estiver no {{ scenario }} os bônus e efeitos da carta são aplicados a todos os personagens no tabuleiro.
    - Quaisquer bônus negativos proporcionados pela carta **não** são aplicados ao Herói que a ativou.
    - O efeito na caixa identificadora do Summus é valido apenas para o Herói que a ativou.
- A carta deve ser removida do {{ scenario }} após passados a quantidade de *Fases de Restauração* definidas na carta.
- Pode ser ativado apenas no turno do seu dono, e o turno se encerra imediatamente após sua ativação.


<br>

||| Caixa de Mecânica
![Exemplo](/static/img/summus/dominium.png)

- ***Ampulheta***: Quantidade de Fases de Restauração até esta carta ser enviada de volta para o [Inventory](https://www.notion.so/Inventory-27083fd0169e80aba6baefb8c6107f82?pvs=21) do ativador.
- ***Texto***: Efeito que é usado ou aplicado apenas pelo ativar desta carta. São sempre **PERMANENTES**.
|||
===



==- <span class="summus"> Daemon</span>
> Daemon em latim significa “espírito”, “gênio” ou “divindade menor”. Vindo do grego clássico, daímōn.
> 
> Daemon são seres do submundo ou do abismo, feitos de matéria escura, eles existem no mesmo espaço-tempo que nós, porém em uma dimensão “ao lado”. Portando sua matéria está aqui conosco, é possível sentir sua presença assustadora e “pesada”, mas não é possível vê-los, ouvi-los, etc. ou interagir com eles de forma padrão, sendo necessário diferentes tipos de magias para isso.
> 
> Os Daemons por usa vez também podem sentir mas não ver ou interagir conosco, sendo para eles também necessário magias para isso.
> 
> Daemons podem ser evocados para a nossa dimensão através de rituais e magias específicas. Porém evocar uma criatura de matéria no mundo da matéria escura é algo muito mais complexo e quase impossível.
> 
> Eles são como os seres da nossa dimensão, tendo diferentes níveis de inteligência, corpos, personalidades, podem ser bons ou maus, ter ou não consciência, etc. Porém há uma tendência para o comportamento maléfico entre eles.
> 
> São animados por um tipo de espírito chamado Vulto, que existe apenas no submundo.
> 
> Não existe o conceito de espécie entre eles, sendo cada exemplar único, mas é possível agrupá-los em conjuntos com características semelhantes.
> 
> Por este motivo, são representados por cartas de @Companion do tipo Evocação.

Daemons são cartas de {{ companion }} do tipo evocação que ficam de face para baixo no Suporte, quando ativadas elas trazem criaturas de tamanhos variados que por suas dimensões ou condições extra espaciais dimensionais, não possuem uma peça no tabuleiro, mas sim uma área de presença dimensional ou física.

Os daemons são evocados através de um custo em *“sangue”*.

<br>

#### Regras Especiais

- Para evocar um Daemon o Herói deve pagar o custo em VIDA determinado na carta.
- No início do turno do Daemon, o seu dono deve pagar 25 de VIDA, ou desevoca-lo
- Ele deve escolher uma área quadrada no tabuleiro conforme o tamanho especificado do daemon.
    - No início da turno do daemon, esse área pode ser redefinida.
- Toda ação do daemon que tiver um alvo, seleciona todos os personagens dentro da área como alvos.
    - Se o personagem possuir efeitos “ao ser selecionados / ao ser atacado / etc.”, eles são válidos
- Quando mais de um daemon estiver em jogo, eles podem selecionar um ao outro como alvo sem estar na área um do outro.
    - Daemons não podem atacar outras peças que não daemons se houver mais de um daemon em jogo.
    - Considere que o Daemon está adjacente e a 1 de distância, quando atacando
- Quando a VIDA deles chega a 0 ou menos, aplica-se a mesma regra de outras evocações.
- Daemons não podem ser curados
- Seu daemon pode ser evocado apenas uma vez por batalha
- Quando tiverem slots de anexos, para ativar as técnicas que utilizam aqueles slots, as respectivas cartas devem ser descartadas

<br>

||| Caixa de Mecânica
![Exemplo](/static/img/summus/daemon.png)


|||
===

---
