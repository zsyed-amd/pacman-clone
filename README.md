# Dot Muncher

A simple Pac-Man inspired browser game built with plain HTML, CSS, and JavaScript — no frameworks, no dependencies.

## How to run

1. Clone or download this repository.
2. Open `index.html` in any modern web browser (Chrome, Firefox, Safari, Edge).

That's it. No build step, no server required.

## Controls

| Key | Action |
|-----|--------|
| Arrow Up / Down / Left / Right | Move your character |
| R | Restart the game |

## Objective

- Eat every yellow dot on the board to **win**.
- Avoid the red ghost — if it touches you, it's **game over**.
- Your best score is saved for the current session.

## Game rules

- **+10 points** for each dot collected.
- The ghost chases you using a mix of direction-toward-player logic and random turns, so it's challenging but beatable.
- Movement is queued: press a direction key just before a turn and the character will take it as soon as the corridor opens.

## File structure

```
pacman-clone/
└── index.html   ← entire game (HTML + CSS + JS in one file)
└── README.md    ← this file
```

## Notes

- All artwork and audio is original — no copyrighted Pac-Man assets are used.
- The game runs at the browser's native refresh rate (~60 fps) via `requestAnimationFrame`.
- Beginner-friendly code: no classes, no bundler, no transpiler — just one readable script block.
