# Technical Specification

## Platform

**Mobile web first, desktop browser second.** Zero install friction, easy to share. UI decisions prioritize touch:

- Large tap targets — finger-friendly buttons, no tiny upgrade rows
- Single-column or card layout — no wide multi-panel dashboards
- Minimal text input — everything tappable, not typed
- Readable numbers at a glance — abbreviations (1.2M, 4.5B) over long digit strings
- No hover states as primary UI — tap-equivalent fallbacks required
- Offline-friendly by design — mobile players close tabs constantly
- Portrait orientation assumed

---

## Technologies / Engine

Vanilla JS + HTML/CSS, or React. No game engine needed. State is a JS object; `setInterval` drives the tick. LocalStorage for save state. No build pipeline required for week one.

---

## Assets

Mostly text and CSS — lean into it aesthetically (monospace/terminal look, or clean minimal). Icons via emoji or a free icon set (Lucide, Heroicons). No sprites, no audio required for week one.

---

## Testing

Manual playthroughs at 1x and 10x speed (add a dev speed multiplier). Unit test core math functions (production rates, cost curves). No full test suite needed for week one.

---

## Playtesting / Bots

Write a simple headless bot that calls the game tick function in a tight loop — simulates hours of play in seconds, catches balance cliffs early. Two bots:
- **Dumb bot** — buys first available upgrade
- **Greedy bot** — always maximizes rate/cost ratio

---

## Open Questions

- Visual style — terminal/monospace, or warmer organic aesthetic given the theme?
