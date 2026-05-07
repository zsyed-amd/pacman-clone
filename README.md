# Ceiling Raccoon

A Pac-Man inspired browser game built with plain HTML, CSS, and JavaScript — no frameworks, no dependencies.

---

## Context / Inspiration

> **Based on true events.**
>
> Long ago, in the AMD office located in Markham, Canada, a family of raccoons lived in the ceiling.
> One day, a baby raccoon fell through — and an employee chased it around the office.
>
> *Ceiling Raccoon* recreates that fateful day. You are the raccoon. The office is the maze. The AMD processor chips scattered on the floor are yours for the taking. The employee is not amused.

---

## How to run

1. Clone or download this repository.
2. Open `index.html` in any modern web browser (Chrome, Firefox, Safari, Edge).

No build step, no server required. Or serve it locally:

```
python3 -m http.server 8000
```

Then open **http://localhost:8000**.

---

## Controls

| Key | Action |
|-----|--------|
| Arrow Up / Down / Left / Right | Move the raccoon |
| R | Restart |

---

## Objective

- Eat every **AMD chip** (white arrow shapes) scattered through the office to **escape**.
- Avoid the **employee** (the angry guy chasing you) — if he catches you, it's over.
- Your best score is saved for the current session.

---

## Scoring

- **+10 points** per chip collected.
- Eat all 164 chips to win.

---

## Characters

| Sprite | Who |
|--------|-----|
| Gray raccoon with black eye mask | You — the baby raccoon |
| Angry employee with blue shirt | The enemy |
| White arrow shapes | AMD processor chips |

The employee chases you 65% of the time and wanders randomly the rest — challenging but beatable.

---

## File structure

```
pacman-clone/
├── index.html   ← entire game (HTML + CSS + JS in one file)
└── README.md    ← this file
```

---

## Notes

- All artwork is original — simple shapes drawn with the Canvas 2D API. No copyrighted assets used.
- Movement is queued: press a direction just before a turn and the raccoon takes it as soon as the corridor opens.
- Runs at the browser's native refresh rate (~60 fps) via `requestAnimationFrame`.
- Beginner-friendly code: no classes, no bundler, no transpiler — one readable script block.
