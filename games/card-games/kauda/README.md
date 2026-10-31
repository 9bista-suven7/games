# Kauda

Kauda (कौडा) in a single HTML file: toss 16 cowrie shells on a Tihar mat and bet against three bots, with free play chips only (no real money).

Kauda is the shell game Nepali families and friends play during Tihar, by diyo light on a straw mat or a cloth spread on the floor. Rules change from village to village and house to house, so this is one clear, common-style version, not the only correct one.

## Play

Open `index.html` in a browser. No build step needed. Your chip balance is remembered in your browser. If you run out, you get a free refill.

## Rules

- Each round the tosser (it changes every round) shakes **16 cowries** and throws them on the mat. The result is how many land **open**, mouth up: 0 to 16. Every shell is a fair 50/50.
- Before the toss, pick a chip (10, 50, 100 or 500) and tap boxes on the betting mat. You can bet on several boxes, up to 5,000 per box. **Clear** takes your bets back, **Repeat** places last round's bets again, **Toss** closes betting. After 20 seconds the shells are thrown anyway.
- **Exact number** 1 to 16, **Low** (0 to 6), **Middle** (7 to 9), **High** (10 to 16), **Odd** or **Even** (0 counts as even). There is no exact 0 bet; an all-closed toss counts only as Low and Even.
- A win pays **×N** of your bet, bet included. Each multiplier comes from the real binomial chance of that result with a house edge of about 5%, rounded to a friendly number:

| Bet | Pays |
| --- | --- |
| Exactly 8 | ×4.8 |
| Exactly 7 or 9 | ×5.4 |
| Exactly 6 or 10 | ×7.8 |
| Exactly 5 or 11 | ×14 |
| Exactly 4 or 12 | ×34 |
| Exactly 3 or 13 | ×110 |
| Exactly 2 or 14 | ×520 |
| Exactly 1 or 15 | ×3,900 |
| Exactly 16 | ×62,000 |
| Low or High | ×4.2 |
| Middle | ×1.75 |
| Odd or Even | ×1.9 |

The three bots each have a style: **Careful** (small outside bets), **Bold** (bigger, mixed bets) and **Numbers** (spreads chips over favourite exact numbers). A bot that runs out of chips leaves and a new one sits down.
