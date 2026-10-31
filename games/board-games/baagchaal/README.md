# Baagchaal

Baagchaal (बाघचाल, "tigers' moves") in a single HTML file: play the goats or the tigers against the computer at three levels, or pass one device between two players.

Baagchaal is a traditional board game from Nepal, often played with stones or shells on a board drawn on the ground, and today also sold as brass sets with metal tigers and goats. It is a hunt game: four tigers against twenty goats, strength against numbers.

## Play

Open `index.html` in a browser. No build step needed. Your last side, level, timer and player names are remembered in your browser.

## Rules

- The board is a 5×5 grid of points. Pieces move along the lines; diagonal lines run only through every other point.
- **4 tigers** start on the corners. **20 goats** start off the board. **Goats move first.**
- **Placing**: each goat turn puts one goat on any empty point, until all 20 are in. Only then may goats move. Tigers move and capture from the start.
- **Moving**: a goat steps one point along a line. A tiger steps one point, or **captures** by jumping over a neighbouring goat in a straight line to the empty point behind it. One jump per turn, no chains, and capturing is optional.
- **Tigers win** by capturing **5 goats**. **Goats win** by trapping the tigers so none can move. If the goats ever have no move, the tigers win.
- **Draw** on the same position three times, or after 100 moves in a row without a capture once all goats are placed. You get a warning first.
- Tap an empty point to place a goat. Tap a piece to see its moves (green dots for steps, red rings for captures), then tap a point or drag the piece there.
- **Undo** takes back your move and the computer's reply. **Hint** highlights a good move. Optional move timer: 20 or 40 seconds a turn, after which a quick move is played for you.

Modes: **vs Computer** (play the goats or the tigers; Easy, Medium or Hard) and **2 players** on one device. The computer is a home-made alpha-beta search that runs in a background worker, so the board never freezes while it thinks.
