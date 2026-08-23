# TypeRacer

> A timed typing speed test that shows you which keys you actually keep getting wrong.

**[Live demo](https://typeracer-mlx.vercel.app)**

Typing tests give you a WPM number and nothing actionable. TypeRacer runs the same 30-second, 60-second, or 2-minute drill over a rotating set of programming quotes, coloring each character green or red as you type it, but it also records every mistyped character and renders the tally as a heat-mapped QWERTY keyboard on the results screen — so the fix is a specific finger, not "practice more." Every completed run is written to `localStorage`, giving you a running log to compare against without an account.

## Features

- Three timed modes: 30 seconds, 60 seconds, or 2 minutes
- Live WPM, accuracy, error count, countdown, and a progress bar, updated as you type
- Per-character feedback with a blinking cursor, backspace support, and auto-scroll to keep the cursor in view
- Error heatmap on the results screen shading each key by how often you mistyped it
- Attempt history saved in `localStorage` (last 50 runs stored, 10 shown), with a clear button
- Keyboard shortcuts: <kbd>Tab</kbd> to restart, <kbd>Esc</kbd> for a new passage
- 24 built-in passages drawn from programming quotes

## Stack

- Vanilla JavaScript, HTML, and CSS in a single `index.html` — no framework, no runtime dependencies
- Vite for the local dev server and production build
- `localStorage` for attempt history; no backend and no external APIs

## Running locally

```bash
npm install
npm run dev
```

---

Part of a series of 90 small web apps. [Browse them all](https://lorenzoylosada.vercel.app).
