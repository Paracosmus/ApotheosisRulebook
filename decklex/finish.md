---
label: Acabamento
icon: paintbrush
order: 90
---
{{ review() }}

# Acabamento

{{ briefing `Finish` `O acabamento é o tratamento visual que uma cópia de uma carta recebe sobre a sua arte, como um brilho ou um efeito na ilustração. Ele não muda nada no jogo: só a aparência da carta.` }}

---

## Composição

- Um acabamento combina até três partes: um brilho sobre a carta (*foil*), um tratamento da ilustração e floreios.
- Só existem os acabamentos que têm nome. Cada nome é uma combinação fixa dessas partes.
- Acabamentos com nome hoje: **Simples** (*Plain*) e **Brilhante** (*Gloss*).

## Peso e chance

- Cada acabamento que uma carta pode receber tem um peso.
- A chance de um acabamento é o seu peso dividido pela soma dos pesos de todos os acabamentos da lista.
- A chance de cada acabamento é pública: o álbum mostra, em porcentagem, a chance de cada um.

## De onde vem a lista

- Uma carta pode ter a sua própria lista de acabamentos, cada um com o seu peso.
- Uma carta sem lista própria usa a lista da sua raridade:

{.clean}
| Raridade        | Acabamentos                    |
| --------------- | ------------------------------ |
| {{ common }}    | Simples **100%**               |
| {{ uncommon }}  | Simples **100%**               |
| {{ rare }}      | Simples **60%**, Brilhante **40%** |
| {{ epic }}      | Brilhante **100%**             |
| {{ legendary }} | Brilhante **100%**             |

## Cópias

- O acabamento é sorteado quando uma cópia da carta é criada, e fica com ela.
- Duas cópias da mesma carta podem ter acabamentos diferentes.
- Uma carta animada nunca recebe um acabamento que atrapalhe a sua animação.
