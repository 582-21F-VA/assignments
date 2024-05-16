# Project 1: Twenty-one

> Weight: 20% \
> Due date: June 3rd

Twenty-one is the name given to a family of popular card games, the
progenitor of which is recorded in Spain in the early 17th century.
Whilst there are numerous variants of twenty-one, the following general
rules apply:

-   A *banker* deals two cards from the top of shuffled deck of 52 to a
    player known as the *punter*.
-   The punter, having examined both cards, announce whether they will
    stay with the cards they have ("stand") or receive another card from
    the banker ("hit").
-   The aim is to score exactly twenty-one points or, failing that, to
    come as close to twenty-one as possible, based on the card values
    dealt. If a player exceeds twenty-one, they lose.
-   Number cards count as their number, the jack, queen, and king ("face
    cards" or "pictures") count as 10, and aces count as 11.
-   Once the punter has either announced they will stay with their cards
    or exceeded twenty-one, the banker takes their turn.
-   The banker is dealt cards until their hand achieves a total of 17 or
    higher.
-   Whoever's hand is closer to twenty-one (but not higher) wins.

A standard 52-card deck comprises 13 ranks in each of the four suits:
clubs (♣), diamonds (♦), hearts (♥) and spades (♠). Each suit includes
three court cards (face cards): king, queen and jack. Each suit also
includes ten numeral cards, from one (ace) to ten.

## Requirements

Create a program that allows one to play twenty-one from the
command-line. When executed, the program should print the punter's hand,
and wait for them to input "hit" to receive another card, or "stand" to
stay with the cards they have. Any other input should be responded to
with an error message explaining how to play. Once the punter has
announced they will stay with their cards or exceeded twenty-one, the
program should print the banker's hand, and declare a winner. At the end
of a round, the player is prompted to enter "continue" to play another
round, or "exit" to close the program. Of course, the deck must be
shuffled before each round. To do so, swap each card once with another
random card in the deck.

## Tips

-   The `prompt` built-in fonction can be used to take input from the
    command-line.
-   The `random` method of the `Math` built-in object returns a
    floating-point, pseudo-random number that's greater than or equal to
    0 and less than 1.
-   Use functions to break down the program: `dealCard`, `shuffleDeck`,
    etc. Each function should contain one idea only.
-   The punter only needs to know the total value of their hand.

## Submission

The project must be submitted in a repository using GitHub Classroom. To create the repository, click [here][], and accept the assignment.

[here]: https://classroom.github.com/a/-ixXrxdI

## Assessment criteria

-   Requirements are met.
-   Code is readable and consistently formatted.
-   Naming is descriptive and consistant.
-   Program flow is decomposed into manageable, logical pieces.
-   Common code is unified, and not duplicated.

