# Score Tracker

A single-page thumbs up / thumbs down score tracker with a "saves" system.
Open `index.html` in any browser — no build step or server needed.

## Rules

- **👍 (right answer):** score goes up by 1.
- **👎 while score is above zero and you have saves:** you lose one save and the score stays where it is.
- **👎 while score is above zero and you have no saves:** score resets to 0, the global saves counter goes up by 1, and the new round starts with that many saves.
- **👎 at score 0:** nothing happens. Saves and the global counter stay the same.
- **Bonus stars:** if the score was 10 or more when it resets to 0, you earn one ⭐ bonus star. It's one star per reset, however far above 10 you got.
- **Highest score:** the highest score you've ever reached is tracked.

## Extras

- ↑ / ↓ arrow keys work as 👍 / 👎.
- State is remembered across page reloads (browser `localStorage`).
- The ↺ button (top right) resets everything.
- The layout scales to fill the window, so it fits a short split-screen pane on a phone.
