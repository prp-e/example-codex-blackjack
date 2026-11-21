# The Velvet Room Blackjack

A free, Vegas-inspired blackjack game built with plain HTML, CSS, and JavaScript. Play against a computer dealer without betting or creating an account.

## Run locally

Clone this repository or download `index.html`, then open the file in a modern browser. The game needs no build step, server, or package installation.

## How to play

1. Select **Deal cards**. You and the dealer each receive two cards, with one dealer card face down.
2. Select **Hit** to draw another card or **Stand** to end your turn. Going over 21 busts your hand.
3. The dealer reveals the hidden card and draws until reaching 17 or more. The dealer stands on soft 17. If neither hand busts, the higher total wins. Equal totals are a push.

Aces count as 1 or 11, whichever gives the best total without busting. Face cards count as 10. An ace and a ten-value card on the opening deal make blackjack. If both players have blackjack, the hand is a push.

## At the table

- A six-deck shoe carries over between hands and reshuffles before the next deal when fewer than 60 cards remain.
- The opening deal is staggered, and the dealer reveals and draws cards at a measured pace. The game respects your browser’s reduced-motion preference.
- **Sound** toggles locally generated audio cues. Sound starts off.
- The table tracks wins, losses, and pushes for the current session. Reloading resets the tally and shoe.

## Source and artwork

`index.html` contains the layout, styles, dealing animations, shuffle, scoring, and dealer logic. Card faces load from [Deck of Cards API](https://deckofcardsapi.com/). If an image is unavailable, the card displays its rank and suit.
