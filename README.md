# Neon Snake

Glow-in-the-dark arcade Snake. Zero build, single `index.html`.

## Play

Open `index.html` in a browser, or serve locally:

```bash
python3 -m http.server 8000
# http://localhost:8000/index.html
```

## Controls

- Arrows / WASD — move
- Space / P — pause, Enter/Space — start / restart
- M — mute, buttons + swipe + d-pad on mobile

## Modes

- Classic (120ms), Speed (90ms, ramps fast), No Walls (wrap).

Bonus food every 5 eats (+30, 5s timer). Win by filling the board.

## Files

- `index.html` — game (CSS + JS inline for zero-build Pages hosting)
- `CHANGELOG.md` — history
- `LICENSE` — MIT
