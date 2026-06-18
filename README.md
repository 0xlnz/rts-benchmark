# RTS Benchmark

A small, ongoing benchmark: every time a new model comes out, it gets handed the
**exact same prompt** and has to build a real-time strategy game as a single,
self-contained HTML file — one shot, no editing, no follow-up turns.

**▶ Play the entries: https://0xlnz.github.io/rts-benchmark/**

## The prompt

> Create a simple but functional real time strategy (RTS) game similar to old
> WarCraft, StarCraft or Command & Conquer games. The player should be able to
> build buildings, create units, gather resources and should uncover the whole
> map. No AI or multiplayer needed. Use simple but nice-looking graphics. No
> sound. Implement everything in HTML/CSS/JS, everything in a single file (you
> can use 3rd-party js or css libraries/frameworks via CDN).

The prompt lives in [`rts-fable/PROMPT.md`](rts-fable/PROMPT.md).

## Rules

- The prompt is given **verbatim** — no edits, no extra instructions.
- The model gets **one attempt**.
- Output must be a **single HTML file** (CDN libraries allowed).
- Whatever the model produces is saved **untouched** — no hand-fixing.

## Entries

| Model | Game | Notes | File |
|-------|------|-------|------|
| Claude Fable 5 | **IRONHOLD** | English · retro CRT / pixel look | [`rts-fable/fable.html`](rts-fable/fable.html) |
| Claude Opus 4.8 | **Regno di Eldoria** | Italian · polished fantasy UI | [`rts-fable/opus48.html`](rts-fable/opus48.html) |

Each game runs entirely in the browser — just open the file (or play via the
link above). Typical controls: drag to box-select, right-click to move, `WASD`
to pan the camera.

## Adding a new model

1. Give the model the prompt from `rts-fable/PROMPT.md`, unchanged.
2. Save its single-file output next to the others (e.g. `rts-fable/<model>.html`).
3. Add a card to `index.html` and a row to the table above.
