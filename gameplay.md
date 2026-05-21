# Gameplay Specification

## Idle / Clicker Balance

Mostly idle with a handful of meaningful manual actions early on, then full automation takes over. Avoid click-spam — one deliberate click per minute feels better than 60 mindless ones.

---

## Mechanics

Core loop: resource generation → spend on multipliers → unlock new resource types → repeat.

Optional layers to consider: prestige reset, tech trees, conversion ratios that reward optimization.

**Week one:** 2–3 resource tiers and one upgrade tree. Save prestige for later games.

---

## Player Involvement

Patient-friendly but optimizer-rewarding — you always progress, but smart players go 20–30% faster. Avoid gates that require wiki-diving. One or two "aha" moments where a non-obvious combo pays off is plenty.

---

## Randomness

Minimal for game #1. Maybe one small random event (a windfall, a setback) every 10–15 minutes for texture. Avoid RNG that blocks progress.

---

## Endless vs. Clear Finale

**Clear finale** recommended for game #1. Ends with a satisfying surprise, leaves players wanting more. Endless games are harder to pace and easier to abandon.

### Time Loop Failure State (proposed idea)

A way to fail without dying. If the player falls so far behind — ecosystem collapsed, unable to generate the resources needed to reach the finale and send the signal — space-time starts to break. The causal loop requires the signal to be sent; if it can't be, the timeline unravels. The player loops back to the beginning of the current stage.

- **Not permadeath.** Progress within the stage is lost, but knowledge isn't — the player knows what went wrong.
- **Slow before the loop.** The break should be visible in advance: a "timeline stability" metric degrading, passenger unease, the signal indicator flickering. The loop is a last resort, not a surprise.
- **Fits the black hole stage naturally.** Time dilation already makes that stage feel unstable; a loop there has the most narrative logic.
- **Ties to the bootstrap paradox.** The signal *must* be sent — it always was. A timeline where it isn't can't exist. The loop is the universe correcting itself.

Open question: should the loop be stage-scoped (restart the current stage) or section-scoped (restart a group of stages)?

---

### The Tuning Finale

The finale is not passive. The player must tune the emitted signal — the one meaningful manual action at the very end of an otherwise idle game.

- The received signal has a "shape" visible in the signal indicator throughout the game, so matching or diverging from it is legible without instruction.
- **Match exactly** → the loop closes; the signal goes out unchanged; somewhere, another civilisation will hear it and follow; the cycle continues.
- **Tune it differently** → the loop breaks; humanity sends something new; the cycle ends. This is the "happy ending" — breaking the loop is the rewarded choice.

The resolution is earned by choosing it, not just arriving at it. The alien encounter can hint at this choice — whether their own civilisation broke their loop is left as a quiet open question.

---

## Signal Indicator

A persistent signal indicator — small, always visible, not explained when it first appears.

- **Early game:** barely registers.
- **As ecosystem grows:** strengthens visibly; players notice the correlation before anyone names it.
- **Alien encounter (Stage 16):** the indicator visually syncs with the alien ship's; no text needed.
- **Finale:** indicator flips direction (receiving → emitting); during tuning, it shows the shape being adjusted; on completion it transforms or resolves.

By the time the alien encounter confirms the explanation, players have already figured it out themselves from watching the indicator. The dialogue confirms rather than informs.

---

## Multiplayer

Skip entirely for game #1. Even a leaderboard adds auth/backend complexity. Save for a later game where async competition is a core mechanic worth building around.

---

## Offline Mode

Capped offline progress (e.g. max 8–12 hours of gains). Easier to balance than true offline — avoids players returning to broken economies. Calculate time elapsed on load, apply capped production, show the player what they earned. That reveal moment is itself satisfying. Especially important as a mobile-first game — players close tabs constantly.

**Special case:** during the Black Hole stage, time dilation could invert this — offline gains are *increased* during this stage as a narrative flourish (time outside moves faster near the black hole).

---

## Open Questions

- Specific resource chain — needs detailing (energy, water, minerals, oxygen, biomass?)
- Species list — which species, what do they do mechanically?
- Upgrade structure — tech tree shape, cost curves
- Prestige mechanic — defer to game #2 or include in game #1?
- Signal indicator visual design — what does "shape" look like concretely?
- Tuning interface design — how does the player adjust the shape at the finale?
