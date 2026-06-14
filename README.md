# Pac-Hunt

Pac-Man, but you're the ghost.

You chase an AI-controlled Pac-Man around the maze. Catch him to win. If he
eats a power pellet he turns the tables and hunts *you* for a few seconds — run.

**Play:** open `index.html`, or visit the Pages URL once deployed.

## Controls

| Action | Keyboard | Gamepad |
|---|---|---|
| Move | Arrow keys / `WASD` | Left stick / D-pad |
| Pause | `Space` | Start (button 9) |
| Restart | `R` | B (button 1) |
| Start / Play again | any move key | A (button 0) |

Touch: swipe to move.

## How it works

Single self-contained HTML file, canvas-rendered, no build step and no
dependencies (the only external thing is a Google Fonts link for the arcade
typeface). Pac-Man runs a BFS that seeks the nearest dot, flees when you close
within ~6 tiles, and beelines for power pellets when cornered — flip to chasing
you while powered.

Tuning knobs live at the top of the `<script>`: `SPEED_GHOST`, `SPEED_PAC`,
`SPEED_PAC_POWER`, and `FLEE_R`.

## License

[MIT](LICENSE)
