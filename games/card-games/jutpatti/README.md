# Jutpatti

Jutpatti (जुटपत्ती) in a single HTML file: you against three bots. Pair off your cards and don't get stuck with the odd one.

## Play

Open `index.html` in a browser. No build step needed.

## Rules

- 4 players, one deck. One card is taken out face down and set aside unseen, so its colour partner becomes the odd card that can never be paired. The other 51 cards are dealt out (12 or 13 each).
- A pair (jut) is two cards of the same rank and the same colour: K♥ + K♦, or 7♠ + 7♣. 7♠ + 7♥ is not a pair.
- Everyone first throws all their pairs face up on the table.
- Then, clockwise from the player after the dealer, each player draws one card blind from the next player's hand. If it makes a pair, the pair is thrown down. The player who was drawn from goes next.
- Run out of cards and you're safe. Safe players are skipped; you draw from the next player who still has cards.
- The last player left holding the odd card loses the round, and the set-aside card is revealed.
- Each loss is counted on the scoreboard. Fewest losses is best.
- You have 20 seconds to draw; if time runs out, a random card is drawn for you. Bots shuffle their hands now and then; you can Shuffle or Sort yours.

Local rules vary (a Joker as the odd card, pairing any two of a rank, drawing from the previous player). This version uses a set-aside card, same-colour pairs and drawing from the next player clockwise.
