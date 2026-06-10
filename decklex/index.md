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

Decklex is the brain of the electronic version of **Apotheosis Card Game**. It is the rules engine, the card system, and the foundation for all interactions in the game. It is responsible for interpreting the rules, processing player actions, storing the game state, and calculating outcomes. The Decklex engine is mainly responsible for the correct application of card effects in a digital environment, ensuring cards are applied at the right time and in the right way.

This system is designed to be flexible and extensible, allowing new cards, rules, and mechanics to be added easily with little to no changes to existing code.

---

## What is this Section?

This section is dedicated to explaining what Decklex is, how it works, and especially how it is implemented, step by step, in a simple, clear, and accessible way so it can be replicated and improved by other developers, following a tutorial format.

Here, we will explore the concepts behind the rules engine, its architecture and engineering, the data structures it uses, and how these elements interact to process player actions and card interactions.

We will also discuss the design decisions made during Decklex's implementation, the challenges faced, and the solutions used to ensure the engine is efficient, flexible, and easy to maintain.

---

## Who is this Section for?

This section is a space to share the knowledge and experience gained during Decklex's development, and to inspire and help others create their own rules engines for card games or other types of games, serving as a guide, reference, or tutorial.

**If you are a developer, a card game enthusiast, or simply someone interested in how card games work behind the scenes, this section is for you.**

However, this will not be a beginner's guide, and I will not go into detail about basic programming or game development concepts. This guide is for those who already have some game development experience and are interested in learning more about how to create a rules engine for card games.

Decklex was built with [Unreal Framework C++](https://dev.epicgames.com/documentation/unreal-engine/programming-with-cplusplus-in-unreal-engine), specifically to run natively on [Unreal Engine](https://www.unrealengine.com/). Do not worry, because prior experience with Unreal Engine or C++ will not be necessary to understand this guide, since these topics will not be covered and are not relevant to the objective.

**The concepts and techniques presented here are generally applicable** and can be used in other contexts and game engines, or even in a platform-agnostic way. It is expected that you, as a developer, will know how to transfer them to your project's specific context, such as development environment, programming language, platform, etc.

---

## Why does this Section exist?

I decided to write about Decklex's implementation because when I decided to build the digital version of my card game, I noticed a huge lack of resources and information about how to program a card game, how it is done, how cards are resolved, what the best practices are, and how to create a system that can receive a constant flow of new cards and rules without breaking the existing game or requiring huge code additions, and so on.

The topic of coding for card games is almost like a closed club, where few people share their experience and knowledge. The idea of this section is to spread this knowledge so it becomes known and commonplace.

First of all, I need to make it clear that **I am not an expert on this subject**, nor do I have extensive experience in card game development or professional game development in general. What I do have is the experience of creating Decklex and facing the challenges and difficulties that arose during the development process. It was a process of research, constant learning, and considerable difficulty in finding the right information and suitable examples.

Note that Decklex is an indie project under continuous development, built by an enthusiast. Therefore, this is not an AAA-level system, and the techniques and solutions presented here may not be the best or most efficient, or the same ones used by major studios in games like [Yu-Gi-Oh! Master Duel](https://www.konami.com/yugioh/masterduel/), [Magic: The Gathering Arena](https://magic.wizards.com/mtgarena), [Pokemon TCG Online](https://tcg.pokemon.com/tcgl/), etc.

But given the complexity of the rules, mechanics, card effects, and interactions in Apotheosis Card Game, close to the complexity of *Yu-Gi-Oh!*, Decklex is a robust and powerful system capable of handling a wide variety of situations and scenarios in-game. If you are developing a simple or complex card game, this tutorial may be useful to you, and I hope it is, so you do not have the same difficulty I had in finding adequate information and solutions.

---
