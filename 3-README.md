# Rock Paper Scissors

A polished, playable Rock Paper Scissors game against the computer, with score tracking, round history, and reveal animations.

## What it does

- You pick Rock, Paper, or Scissors; the computer picks at random.
- Both hands shake, then reveal the picks together with the round result.
- Live scoreboard for your wins, computer wins, and draws.
- Round history list (newest on top) showing each round's picks and outcome.
- Reset button to start a fresh game. Fully responsive.

## Tech used

- HTML5, CSS3 (custom properties, Grid, keyframe animations)
- Vanilla JavaScript (ES6+) - single `index.html`, no dependencies, no build tools

## How to run

Open `index.html` in any browser. No server or installation needed.

## Talking points (what the code demonstrates)

- **Classic numeric game logic with switch statements:** choices are numbers (1 = rock, 2 = paper, 3 = scissors) and the winner is decided with `switch` statements - readable, and easy to extend with more moves.
- **Constants instead of magic numbers:** `ROCK`, `PAPER`, `SCISSORS` and `WIN`, `LOSE`, `DRAW` make the logic self-explanatory.
- **Async UI timing:** `setTimeout` coordinates the shake animation with the reveal, and a `busy` flag stops double-clicks from breaking a round in progress.
- **Separation of concerns:** small single-purpose functions (`getResult`, `updateScore`, `showResult`, `addHistoryRow`) each do one thing, so the game flow reads top to bottom.
