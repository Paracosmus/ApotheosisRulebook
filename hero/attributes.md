---
label: Atributos
icon: sliders
order: 4
---

<style>

    .attr {
        font-size: 1.5rem;
        color: #00BFA5;
    }
    .bar { color: #212121; }
    .short { color: #607D8B; }

    .combat  { color: #D50000; }
    .ability { color: #64DD17; }
    .magic   { color: #304FFE; }

</style>

{{
    func attr(name, short, class)
        ret '<span class="attr ' + class + '">' + name + '<span class="bar"> | </span> <span class="short">' + short + '</span></span>'
    end
}}



# ATRIBUTOS

Os ATRIBUTOS são uma forma de transpor e quantificar numericamente conceitos complexos da capacidade física, mental e espiritual de um ser vivo, para o mundo do jogo. São as características primárias de todo indivíduo e variam de um para o outro.

O valor mínimo que um ATRIBUTO pode ter é 1. Se o valor se tornar inferior a 1, ele deve ser considerado igual a 1.

---



||| {{ attr " CONSTITUIÇÃO" "CON" "" }}  <span style="width: 20px; display: inline-block;"></span> [!badge variant="secondary" text="completude"]
É o vigor físico e saúde do personagem, baixa constituição resulta em aparência de doente e alta constituição, em aparência saudável.

* Testes relacionados à resistência física.
* Resistência a {{ dmg }}.

|||

---

[!badge variant="danger" text="Corpo"]

||| {{ attr " FORÇA" "FOR" "combat" }}
Determina a força física do personagem, mais ligada à sua capacidade muscular. pode deixar os músculos mais bem definidos, mas não obrigatoriamente.

* Testes relacionados à esforço muscular.
* {{ dmg }} do Ataque Normal.
* {{ dmg }} de ataques corpo-a-corpo como espadas, machados, martelos, entre outros.

|||

||| {{ attr " AGILIDADE" "AGI" "combat" }}
Está relacionada às ações feitas com o corpo, velocidade, reflexos, equilíbrio, destreza, sutileza e graça dos movimentos.

* Testes relacionados à movimentação.
* Número de pontos de {{ ap }} por turno.

|||

---

[!badge variant="success" text="Mente"]

||| {{ attr " PERCEPÇÃO" "PER" "ability" }}
Referente ao uso dos cinco sentidos e acuidade. Um personagem com alta percepção consegue ver e ouvir minúcias imperceptíveis para os demais, em contraparte, um personagem com baixa percepção, é distraído.

* Testes relacionados aos sentidos físicos.
* {{ dmg }} de ataques a distância, como arco e flecha, armas de fogo, entre outros.
* Ordem de turno dos personagens.

|||

||| {{ attr " INTELIGÊNCIA" "INT" "ability" }}
É a capacidade de pensar e raciocinar. Um personagem inteligente tem mais possibilidades de cumprir objetivos sem que para isso seja necessário esforço físico, sendo mais hábil em lidar intelectualmente com pessoas e situações.

* Testes relacionados à capacidade cerebral.

|||

---

[!badge variant="primary" text="alma"]

||| {{ attr " CARISMA" "CAR" "magic" }}
Determina a capacidade do personagem de fazer com que outros gostem dele, seria o seu charme ou característica nata em agradar as pessoas.

* Testes relacionados às habilidades sociais, simpatia, agradabilidade e emoções.
* Sorte, dádivas e outras bençãos.

|||

||| {{ attr " ESPIRITUAL" "ESP" "magic" }}
Está relacionado à capacidade do personagem de sentir e manipular tudo que envolve o éter e é chamado popularmente de magia.

* Testes relacionados ao éter.
* {{ dmg }} de ataques etéreos, como magias e encantamentos.

|||

---
