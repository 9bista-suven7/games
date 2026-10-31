# Jhandi Munda

Jhandi Munda (झण्डी मुण्डा), also called Langur Burja, in a single HTML file: shake six symbol dice in a cup on a Dashain mat and bet against three bots, with free play chips only (no real money).

Jhandi Munda is the dice game you see at Dashain and Tihar gatherings, on a cloth spread at a mela or on the floor at home. Rules change from place to place, so this is one clear, common version, not the only correct one.

## Play

Open `index.html` in a browser. No build step needed. Your chip balance is remembered in your browser. If you run out, you get a free refill.

## Rules

- There are **6 dice**, and every die has the same **6 symbols**: Heart (पान), Spade (सुरत), Diamond (ईंट), Club (चिडी), Flag (झण्डा) and Crown (मुण्डा). Each round the dealer (it changes every round) shakes all six in a cup and rolls them. Every face is equally likely.
- Before the roll, pick a chip (10, 50, 100 or 500) and tap symbol boxes on the betting mat. You can bet on several symbols, up to 5,000 per box. **Clear** takes your bets back, **Repeat** places last round's bets again, **Roll** closes betting. After 20 seconds the dice are rolled anyway.
- For each symbol you bet on, count how many of the 6 dice show it. **0 or 1: you lose that bet. 2 to 6: you win N to 1**, where N is that count, and you get your bet back too.
- Example: 100 on Flag and three Flags land. You win 300 and get the 100 back, 400 in all. One Flag or none and the 100 is lost.

| Dice showing your symbol | Chance | Pays | A 100 bet gets back |
| --- | --- | --- | --- |
| 0 | 33.49% | lose | 0 |
| 1 | 40.19% | lose | 0 |
| 2 | 20.09% | 2 to 1 | 300 |
| 3 | 5.36% | 3 to 1 | 400 |
| 4 | 0.80% | 4 to 1 | 500 |
| 5 | 0.064% | 5 to 1 | 600 |
| 6 | 0.0021% | 6 to 1 | 700 |

## House edge

The count for one symbol is binomial with n = 6 and p = 1/6, so P(N = k) = C(6, k) · 5^(6−k) / 6^6, out of 46,656 equally likely rolls: 15,625 / 18,750 / 9,375 / 2,500 / 375 / 30 / 1 for k = 0 to 6.

Expected chips back per 1 chip bet = (9,375·3 + 2,500·4 + 375·5 + 30·6 + 1·7) / 46,656 = 40,187 / 46,656 ≈ **0.8613**.

So the bank keeps **6,469 / 46,656 ≈ 13.87%** of everything staked in the long run. That is the same for every symbol and for any mix of bets, because each symbol is settled on its own. A symbol wins (shows on 2 or more dice) only about 26% of the time. This is a game of pure luck: no pattern, streak or system changes the odds.

The three bots each have a style: **Careful** (small bets on one or two symbols), **Bold** (bigger bets spread over two or three) and **Flag fan** (superstitious, backs the Flag every single round). A bot that runs out of chips leaves and a new one sits down.
