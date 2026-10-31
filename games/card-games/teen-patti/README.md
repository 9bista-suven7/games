# Teen Patti

Teen Patti (तीन पत्ती) in a single HTML file: you against four bots, with free play chips only (no real money).

## Play

Open `index.html` in a browser. No build step needed. Your chip balance is remembered in your browser.

## Rules

- Everyone puts the boot (100) in the pot and gets 3 cards face down.
- Stay **Blind** or tap **See**. Blind players bet the stake; seen players bet double. **Raise** doubles the stake.
- **Pack** to fold. The last player left, or the best hand at a show, wins the pot.
- **Show**: with two players left, pay your bet and compare hands.
- **Sideshow**: a seen player can ask the previous seen player to compare privately; the weaker hand packs.
- Ties go against the player who asked for the show or sideshow.
- Limits: chaal limit 6.4K, pot limit 1L (everyone left shows automatically).

Hand ranking, best first: Trail, Pure Sequence, Sequence, Color, Pair, High Card. A-K-Q is the top sequence, then A-2-3.
