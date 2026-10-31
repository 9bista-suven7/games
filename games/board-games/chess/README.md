# Chess

Chess (शतरंज) in a single HTML file: play the computer at three levels, or pass one device between two players.

## Play

Open `index.html` in a browser. No build step needed. Your last mode, side, level, clock and player names are remembered in your browser.

## Rules

- White moves first. Win by **checkmate**: attack the enemy king so it has no way out.
- All the standard rules: **castling** (king and rook unmoved, empty squares between, king not in check and not passing through or landing on an attacked square), **en passant** and **promotion** to a queen, rook, bishop or knight.
- Draws are applied automatically: **stalemate**, **threefold repetition**, the **fifty-move rule** and **insufficient material** (lone kings, or a king with one bishop or knight, or bishops all on one square colour).
- Tap a piece to see its moves (dots for empty squares, rings for captures), then tap a square or drag the piece there.
- **Undo** takes back your move and the computer's reply. **Hint** draws an arrow for a good move. **Resign** ends the game.
- Optional clock: 5 or 10 minutes each for the whole game. It starts after White's first move. Running out loses, unless the other side has no way to checkmate, which is a draw.

Modes: **vs Computer** (play White, Black or a random side; Easy, Medium or Hard) and **2 players** on one device (optionally flip the board each turn). The computer is a home-made alpha-beta engine that runs in a background worker, so the board never freezes while it thinks.
