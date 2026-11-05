---
label: Dominium
icon: "/static/img/icons/summus_dominium.svg"
order: 0
---
{{ review() }}

# <span class="summus"> Dominium</span>

> Dominium é o termo latino para “domínio”, no sentido de posse, território, propriedade.
>
> O Dominium é uma dimensão forjada pela vontade do seu criador à sua imagem e semelhança. É uma zona interdimensional que, quando ativada, se entrelaça com o espaço-tempo ao redor do seu conjurador criando uma área no local, com regras e características próprias, definidas pela mente e magia do seu criador, e onde ele é deus.
>
> Por este motivo, são representados por cartas de {{ event }} no {{ scenario }}, aplicando seus efeitos a todos.

{{ dominium }} são cartas de {{ event }} que quando ativadas do {{ inv }} são enviadas para o {{ scenario }} para aplicar efeitos a todos os personagens.

<br>

#### Regras Especiais

- Para ativar um {{ dominium }} do seu {{ inv }} o Herói deve consumir **10** de **Energia** e então enviar a carta para o {{ scenario }}.
    - Apenas um {{ dominium }} pode estar ativo por vez, portanto não é possível ativar um {{ dominium }} se já houver outro no {{ scenario }}.
- Enquanto estiver no {{ scenario }} os bônus e efeitos da carta são aplicados a todos os personagens no tabuleiro.
    - Quaisquer bônus negativos proporcionados pela carta **não** são aplicados ao Herói que a ativou.
    - O efeito na caixa identificadora do {{ summus }} é válido apenas para o Herói que a ativou.
- A carta deve ser removida do {{ scenario }} após passada a quantidade de {{ resetPhase }} definida na carta.
  - O jogador que ativou o {{ dominium }} pode optar por remover o {{ dominium }} do {{ scenario }} antes do tempo.
- Quando no {{ scenario }}, o {{ dominium }} não pode ser removido por efeito.
- Pode ser ativado apenas no turno do seu dono, e o turno se encerra imediatamente após sua ativação.


<br>

||| Caixa de Mecânica
![Exemplo](/static/img/summus/dominium.png)

- ***Ampulheta***: Quantidade de {{ resetPhase }} até esta carta ser enviada de volta para o {{ inv }} do ativador.
- ***Texto***: Efeito que é usado ou aplicado apenas pelo ativador desta carta. São sempre {{ permanent }}.
|||

---
