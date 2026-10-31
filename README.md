# Score Tracker

A single-page thumbs up / thumbs down score tracker with a "saves" system.
Open `index.html` in any browser — no build step or server needed.

## Rules

- **👍 (right answer):** score goes up by 1.
- **👎 while score is above zero and you have saves:** you lose one save and the score stays where it is.
- **👎 while score is above zero and you have no saves:** score resets to 0, the global saves counter goes up by 1, and the new round starts with that many saves.
- **👎 at score 0:** nothing happens. Saves and the global counter stay the same.

## Extras

- ↑ / ↓ arrow keys work as 👍 / 👎.
- State is remembered across page reloads (browser `localStorage`).
- "Reset everything" link at the bottom starts over.
