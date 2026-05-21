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
