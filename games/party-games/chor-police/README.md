# Chor Police

Chor Police (चोर पुलिस) in a single HTML file: the classic Nepali children's game played with folded slips torn from a school notebook. Everyone picks a slip, the Police show themselves, and they have to find the Chor. Play against bots, pass one phone around, or play online with friends on their own phones.

## Play

Open `index.html` in a browser. No build step needed. Your name and last setup are remembered in your browser.

- **Play vs bots**: you and 2 to 9 bots.
- **Pass & play**: one phone, 3 to 10 people. Each player picks a slip, looks, and taps **Fold & pass**. A cover screen hides it before the next player takes the phone. The talking happens out loud.
- **Create table**: everyone plays on their own phone. Friends scan the QR code, open the link or type the 5-letter table code. Empty seats are played by bots.

## Rules

- One folded slip per player: at least one **चोर Chor**, at least one **पुलिस Police**, and the rest **नागरिक Citizens**. The slips are shuffled and spread on the mat, and everyone picks one.
- The Police show themselves. Then everyone else says one line (the **talk round**): calm, defensive or cheeky. The Chor tries to bluff, and nervous bots tend to give themselves away (but not always).
- Each Police secretly names one suspect. A Chor is **caught** if any Police names them. Then all slips are opened.
- **Roles**: pick how many of each on setup. 2 Chor, 2 Police (and 2 Mantri) are allowed from 6 players; Citizens fill the rest. **Auto** brings back the default split.

### Modes

- **Points** (our default): each Citizen +500 every round. A Police who names a Chor +1000, a wrong guess 0. A Chor who isn't caught +1000, a caught Chor 0. Play 5 or 10 rounds; the highest total wins. The point values are our own, modelled on Raja Mantri Chor Sipahi style scoring.
- **Elimination** (the classic chit version): a caught Chor is out, and a Police who names someone who isn't a Chor is out. Each round has one slip per player still in, so the pile shrinks. When only 2 are left, both win.
- **Raja Mantri Chor Sipahi** (राजा मन्त्री चोर सिपाही): 4 to 10 players with **Raja** (always 1), **Mantri** (1, or 2 by default with 8 or more), **Chor**, **सिपाही Police** and **प्रजा Citizens**. The Raja shows himself first and calls "मेरो सिपाही को हो?", then the Police show themselves and name the Chor (the Raja can't be named). Raja 1000, each Mantri 800, each Citizen 300. A Police who catches a Chor gets 500; a Chor who isn't caught gets 500 instead. Point values vary by region and family; this is one common version (in some places the Mantri does the guessing).

## How online play works

Players connect directly to each other, browser to browser (WebRTC via [PeerJS](https://peerjs.com)). There is no game server or database. The free PeerJS service only introduces players to each other.

- The host's browser runs the game (shuffle, bots, rules) and sends each player only their own slip. Everyone's slips are sent out only when they are opened at the end of the round.
- The host should keep the page open and in the foreground until the game ends.
- If a friend disconnects, or their phone goes quiet for 30 seconds (closed tab, lost signal, locked screen), a bot takes over their seat.
- Online play needs the page to be opened from a web address (for example GitHub Pages). Invite links point to `https://9bista-suven7.github.io/games/games/party-games/chor-police/`.
