# Callbreak

Nepali Callbreak (कॉल ब्रेक) card game in a single HTML file. Play against three bots, or online with up to three friends.

## Play

Open `index.html` in a browser. No build step needed.

- **Play vs bots**: plays offline against Bikash, Sunita and Rajan.
- **Create table**: opens an online table and shows a QR code, link and 5-letter table code. Friends scan or open the link (or type the code) to join. Empty seats are played by bots.

## How online play works

Players connect directly to each other, browser to browser (WebRTC via [PeerJS](https://peerjs.com)). There is no game server or database. The free PeerJS service only introduces players to each other.

- The host's browser runs the game (shuffle, bots, rules) and sends each move to everyone else. Each friend only receives their own cards.
- The host should keep the page open and in the foreground until the game ends.
- If a friend disconnects, a bot takes over their seat.
- Online play needs the page to be opened from a web address (for example GitHub Pages). Invite links point to `https://9bista-suven7.github.io/games/games/card-games/callbreak/`.

## Rules

- 4 players, 13 cards each. A hand with no spades is redealt.
- Each player calls how many tricks they will win (1–13).
- Follow suit, and beat the current winning card if you can.
- Out of the led suit? You must play a spade (beating any spade already played if you can); otherwise play any card.
- Make your call: +call, plus 0.1 per extra trick. Miss it: −call.
- Highest total after 5 rounds wins.
