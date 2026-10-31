# Carrom

Carrom (क्यारम) in a single HTML file: flick the striker against the computer at three levels, or pass one device between 2 or 4 players.

## Play

Open `index.html` in a browser. No build step needed. Your last mode, level, match length, player names and control style are remembered in your browser.

## Rules

- Each side has **9 coins** (White or Black). The red **queen** starts in the centre with the coins packed round it.
- Slide the striker along your **baseline**, between the two red circles (it can't sit on a coin), then **pull back** from it like a slingshot and let go. The dotted line shows the path and the first piece it will hit. Shots must go forward. You have 30 seconds; after that a shot is played for you.
- Pocket one of **your own** coins or the queen and you shoot again. Opponent coins you pocket count for them.
- The **queen** can go in once you have pocketed at least one coin (a coin in the same shot counts). You must **cover** it by pocketing one of your coins in the same shot or your next one, or it goes back to the centre.
- **Striker pocketed**: your turn ends and one of your pocketed coins goes back to the centre. A queen pocketed on that shot goes back too.
- You can't pocket the opponent's **last** coin, or your own last coin before the queen is covered: the coin goes back and your turn ends.
- First side to pocket all 9 (with the queen covered by someone) wins the board and scores **1 point per opponent coin left**, plus **3** if they covered the queen.
- Matches: **1 board**, **3 boards** (most points; if level, most boards won) or first to **25 points**. White breaks first, then the break alternates.
- **Aim + Strike** (in the menu) swaps the slingshot for tap-to-aim, a power bar and a Strike button. Keyboard: ←/→ aim, ↑/↓ power, A/D move the striker, Space strikes.

Modes: **vs Computer** (you play White from the bottom; Easy, Medium or Hard) and **Pass & play** for 2 players, or 4 players where partners sit across the board and share a colour. In pass & play the board turns so whoever is shooting is always at the bottom.

The physics is home-made: fixed 240 Hz steps split into substeps so nothing tunnels at full power, elastic collisions (the striker is heavier than the coins), springy cushions and powder-like sliding friction. The computer lines up cut shots with the ghost-ball method, checks that the path is clear, then plays each candidate out in the same physics engine and picks the best result. Sounds are synthesised on the fly.
