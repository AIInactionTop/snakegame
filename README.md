# Super Snake Bros.

A Nintendo-style snake game with these features:

## Game Boy Aesthetic

- Classic green checkerboard background (Game Boy color palette #9bbc0f)
- Press Start 2P pixel font
- Rounded "console" frame with shadow/border effects
- Retro 8-bit sound effects via Web Audio API (eat, power-up, level up, death)

## Gameplay

- Smooth movement — interpolated position between grid steps for fluid animation
- Wrap-around edges — no wall death, snake teleports to opposite side (Nintendo style)
- Eyes on the snake head that track movement direction
- Body segments with gradient coloring and connectors

## Power-ups

Spawn after Level 2, 30% chance on food eat:

- **Speed Boost** (lightning bolt) — 50% faster movement for 8 seconds, blue snake head
- **Score Multiplier** (purple star) — x2 points for 8 seconds, purple body glow
- Power-ups disappear after 12 seconds if not collected, with blinking warning

## Difficulty Progression

- Level increases every 5 apples
- Speed increases each level (150ms → 60ms minimum interval)
- Level-up flash animation + fanfare sound

## Local Leaderboard

- Top 10 scores stored in localStorage
- Shows date, score, and level reached
- New record badge on game over screen

## Controls

- **Arrow keys / WASD** — move
- **P / ESC** — pause
- **Enter / Space** — menu select
- **Mobile** — D-pad + swipe support on canvas
