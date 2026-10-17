---
label: Decklex
icon: /static/img/icons/decklex.svg
order: 0
visibility: protected
---

<style>
    h1:first-of-type {
        display: none !important;
    }

    .logo {
        border: 3px solid rgba(0, 28, 112, 0.2);
    }
</style>

![](/static/img/banners/decklex.svg){.rounded-lg .logo}

## What is Decklex?

> *Deck* + *Lex* (Law) | *Lexer* (Lexical Analyzer)

Decklex is a card game rules engine, first created for the electronic version of [Apotheosis Card Game](https://apotheosiscardgame.com/). A card game rules engine is a system responsible for processing player actions and calculating outcomes. The Decklex engine is mainly responsible for the correct application of game rules and card effects in a digital environment.

Above that, **Decklex is a concept**, a system architecture, not a specific application. It is a set of principles and techniques that can be improved, modified, adapted, and implemented in different ways according to the needs of each project. Here you will find how to code your own version of Decklex, suitable for your project's needs.

This system is designed to be flexible and extensible, allowing new cards, rules, and mechanics to be added easily with little to no changes to existing code. These features make Decklex a powerful tool for managing the complexity of card interactions and game rules in a digital card game.

---

## Who is this for?

This guide is dedicated to explaining what Decklex is, how it works, and especially how it is implemented, step by step, in a simple, clear, and accessible way so it can be replicated and improved by other developers.

**If you are a developer, a card game enthusiast, or simply someone interested in how digital card games work under the hood, this section is for you.**

However, this is not a beginner's guide, and I will not go into detail about basic programming or game development concepts. This guide is for those who already have some development experience and are interested in learning more about how to create a rules engine for card games.

Additionally, **this guide does not cover UI and visual aspects of the game**, as Decklex is focused on the rules engine and card system. UI and visual implementation are handled using completely different methods in each engine or platform and are not relevant to the core concepts of implementing a rules engine. A rules engine is a backend system, and its implementation is independent of the frontend or visual aspects of the game.

Note that Decklex is an indie project; therefore, this is not an AAA-level system, and the methods and solutions presented here are not always the same as those used by major studios in games like [Yu-Gi-Oh! Master Duel](https://www.konami.com/yugioh/masterduel/), [Magic: The Gathering Arena](https://magic.wizards.com/mtgarena), [Pokemon TCG Online](https://tcg.pokemon.com/tcgl/), etc.

Decklex is a robust and powerful system capable of handling a wide variety of situations and scenarios in-game. If you are developing a simple game like *Hearthstone* or a complex one like *Yu-Gi-Oh!*, this guide and system may be useful to you, and I hope it is.

[!badge text="Best regards, Bruno Caxito" size="l" variant="question"]

---
