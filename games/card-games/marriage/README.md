# Marriage

Nepali Marriage (म्यारिज), the 21-card rummy game played with 3 decks, in a single HTML file: you against three bots.

## Play

Open `index.html` in a browser. No build step needed.

## Rules

- 4 players, 3 decks (156 cards, no printed jokers), 21 cards each. One card starts the discard pile; one more is set aside face down as the hidden **Maal** card. The rest is the stock.
- On your turn, draw from the stock or take the top discard (only if it makes a meld right away with two of your cards), then discard one card.
- Melds: **pure sequence** (3+ in a row, same suit; A-2-3 and Q-K-A are fine, K-A-2 is not), **trial** (3 of a rank in different suits), **tunnela** (3 identical cards, counts as pure).
- **Show**: lay down 3 pure melds of 3 cards (sequences or tunnelas). You then see the Maal card, and its jokers become wild for you: Tiplu (same card), Poplu (one up), Jhiplu (one down), Alter (same rank and colour) and the other cards of that rank. Players who haven't shown get no jokers.
- **Finish**: after showing, finish when every card in your hand but one fits into melds (jokers allowed). Your last card goes face down and the round ends. If the stock runs out, nobody finishes.
- **Maal points** (only for players who have seen): Tiplu 3, Poplu 2, Jhiplu 2, Alter 5, Marriage (Jhiplu + Tiplu + Poplu together) 10. Each player gets Maal × 4 − total Maal of everyone.
- **Game points** to the winner: 10 from each player who hasn't seen, 3 from each who has.
- 5 rounds; highest total wins. You have 40 seconds per turn.
- Helpers: sort by suit or rank, **Group** puts your melds together, **Find melds** picks 3 pure melds to show, and after showing **Hint** suggests a discard.

Not included: the dublee (7 pairs) finish, Man cards, and kidnap/murder variants.
