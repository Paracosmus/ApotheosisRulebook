# 1. The Cards

As cartas são o elemento central de qualquer jogo de cartas. Elas são a base da maioria das interações e jogabilidade. Então nada mais justo e fundamental do que começarmos por elas.

Na nossa engine, existem 3 tipos de cartas, cada uma com suas próprias características e funções. São elas:

[Card](#card), [Set Card](#set-card), e [Play Card](#play-card).

---

## Card

Este é o objeto carta de fato, é onde as informações da mesma estão contidas, como nome, descrição, atributos, etc.

+++ Card Object

  ```typescript
  abstract class Card {
      name: Text;
      illustration: Texture;
      effects: [Text];
      keywords: [EKeyword];
  };
  ```

  ```typescript
  class MonsterCard extends Card {
      attack: integer;
      defense: integer;
  };
  ```

  ```typescript
  class SpellCard extends Card {
      type: ESpellType;
      manaCost: integer;
  };
  ```

  !!! Classe **Abstrata**
  A classe `Card` é abstrata, o que significa que ela não pode ser instanciada diretamente. Ela serve como uma base para outras classes de cartas específicas, como `MonsterCard` e `SpellCard`, que podem herdar suas propriedades e métodos, comuns a todas as cartas.
  !!!

  !!! Tipo **Text**
  O tipo `Text` é utilizado para armazenar uma string localizável, ou seja, que pode ser traduzida para diferentes idiomas. A maioria das engines possuem um tipo nativo para isso, como o `FText` do Unreal Engine, que é recomendado para textos que serão exibidos para o jogador, como nomes, descrições e flavor text. Ele permite que o jogo suporte múltiplos idiomas de forma eficiente. Se seu sistema de localização for diferente, adapte o tipo conforme necessário, ou use uma string simples caso não tenha esta funcionalidade.
  !!!

  !!! Tipo **Texture**
  O tipo `Texture` é utilizado para armazenar uma imagem ou textura, que pode ser exibida no jogo. A maioria das engines possuem um tipo nativo para isso, como o `UTexture2D` do Unreal Engine, que é recomendado para ilustrações de cartas, ícones e outros elementos visuais. Ele permite que o jogo utilize recursos gráficos de forma eficiente. Se seu sistema de renderização for diferente, adapte o tipo conforme necessário, ou use um caminho para a imagem caso não tenha esta funcionalidade.
  !!!

  !!! Tipagem
  O efeito ocasionalmente pode ser uma estrutura mais complexa, podendo conter campos como `requirements`, "keywords", entre outros. Na implementação do Apotheosis especificamente, é usado um array de `Effect (struct)`, já que evita redundância e melhora a organização, pois uma carta pode ter vários efeitos.
  !!!

+++ Card Properties

  ```typescript
  enum EKeyword {
      // Activation
      Activate,
      Permanent,

      // Triggered
      OnPlay,
      OnDiscard,

      // Mechanical
      Flying,
      Trample,
  };
  ```

  ```typescript
  enum ESpellType {
      Normal,
      Quick,
      Continuous,
  };
  ```

  !!! Implementação
  Esta é apenas uma forma de implementar a os efeitos. Para o seu jogo, pode ser melhor dividir as keywords em diferentes enums por categorias por exemplo. Aqui, como em todo este guia, manteremos a implementação o mais simples possível.
  !!!

  !!! Implementação
  No seu jogo você pode notar que algumas propriedades da carta são tipos primitivos, outros são enumerators, outros são data structures, e outras são objetos completos. Como desenvolvedor você deve avaliar cada propriedade e seus tipo adequado.
  !!!

+++

---

## Set Card

!!!secondary
No Apotheosis não existem Set Cards, isso porque por ser um jogo puramente digital, não existe reprint, portanto toda carta aparece apenas uma vez, na coleção em que foi lançada. A raridade é usada como um "marcador de qualidade" da carta, portanto uma carta precisa ter sempre a mesma raridade. E as coleções são usada para controle de quais cartas são permitidas em cada partida.
!!!

---

## Play Card

---
