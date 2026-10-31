# Tic-tac-toe

Tic-tac-toe (noughts and crosses) in a single HTML file, drawn in chalk on a slate: the classic 3×3 game or five in a row on a 15×15 board, against the computer at three levels or with two players sharing one device.

## Play

Open `index.html` in a browser. No build step needed. Your last board, mode, level and player names are remembered in your browser. The score lasts for the session, until you change the game settings.

## Rules

- Players take turns putting their mark in an empty square. **X always moves first.**
- **3×3 classic**: get **three in a row** across, down or diagonally. A full board with no line is a draw.
- **Five in a row**: get **five in an unbroken line** in any direction on the 15×15 board. Six or more in a line also counts.
- Tap a square to place your mark. On the 3×3 board, keys **1–9** pick a square (1 top left, 9 bottom right). On either board, the **arrow keys** move a highlight and **Enter** or **Space** places your mark.
- **Undo** takes back your move (and the computer's reply). **Rematch** starts the next game; a game you restart halfway doesn't count. **Reset** sets the score back to zero.

Modes: **vs Computer** (play X, play O, or alternate who starts; Easy, Medium or Hard) and **2 players** on one device (X can alternate between you). On Hard the computer plays 3×3 perfectly and never loses. At five in a row it blocks your threats and looks for chains of fours that force a win.
