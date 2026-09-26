# Changelog

All notable changes to Neon Snake.

## [Unreleased]

### Fixed
- Start screen Space no longer opens PAUSED overlay with no game running; Space/Enter now starts the game
- Pause and game-over overlays only cover the canvas (controls stay clickable)
- Stale game-over timer cleared on restart so overlay can't pop over a new game
- `setMode()` takes effect immediately with per-mode base speed (Classic 120ms, Speed 90ms, No Walls 120ms)
- Window resize clamps snake/food back into bounds instead of stranding them off-board
- Bonus timer is wall-clock based with smooth bar; pauses correctly
- Normal food no longer spawns on top of bonus food
- NEW BEST banner only on strict improvement (`score > prevBest`), removed dead `isNewBest`
- Win state when board fills: golden explosion + YOU WIN screen
- Double-reverse race fixed by guarding queued direction (`nextDx/nextDy`)
- rAF accumulator loop replaces `setInterval`/rAF mismatch; full-body interpolation, no head snap
- HiDPI canvas scaling via `devicePixelRatio`
- `ctx.roundRect` fallback for older browsers
- `localStorage` guarded for private mode
- Auto-pause on `visibilitychange`/`blur`
- Swipe scoped to canvas only; viewport allows pinch-zoom; `touch-action` scoped to canvas
- `prefers-reduced-motion` disables background/title/pulse animations

### Added
- Favicon, Open Graph tags, `noscript` message
- Dialog roles, `aria-pressed`, `aria-live` score, `:focus-visible` styles, canvas label

## [1.0.0] — Initial Release

- Glow-in-the-dark snake game
- Three game modes: Classic, Speed, No Walls
- Bonus food and death animations
- Touch and keyboard support
- Animated neon grid background
