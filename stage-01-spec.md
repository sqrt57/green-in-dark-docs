# Stage 1 — Pre-Launch: Specification

Working spec for implementing Stage 1. Open questions are marked **open**; resolved items state the decision. Cross-reference: [Design Notes](stage-01-prelaunch.md), [Theme](theme.md), [Gameplay](gameplay.md), [Technical](technical.md).

**Open questions by priority:**

| Category | Blockers (can't start without) | Important (needed soon) | Deferrable |
|---|---|---|---|
| Story | Upgrade tree / named purchases, passenger lines | Billionaire in-game presence, final purchase identity | Pre-signal foreshadowing |
| Gameplay | Money sources mechanic vs. flavor, cost curve | People/species count mechanics, people qualities effect | Resource unlock triggers |
| UI | Visual style decision | Mobile layout | Money counter presentation |
| Tech | Vanilla JS vs. React | Tick rate | — |

---

## Story / Narrative

### AI characters

**Introduction:** AIs are not present from the start. Each AI becomes available for purchase after the resource it governs is unlocked and the player has clicked manually through that resource a number of times. Once purchased, the AI gradually automates its domain.

**Communication UI:** Each AI has a panel showing: current status, current task, and a progress indicator on the current task. No chat feed — it's a dashboard, not a dialogue.

- Exact unlock thresholds (how many manual clicks before the AI appears) **open**
- Which resource/domain maps to which AI **open**

### The billionaire

- **In-game presence** — named character or anonymous? Founding message, news ticker, log entry? **open**
- **Pre-signal foreshadowing** — how does Stage 1 plant the seed of his unexplained compulsion without naming the signal? **open**

### Passenger lines

- No specific lines written yet. Need at least a handful: arrival, reaction to the scale of the build, something that establishes voice before launch. **open**

### The final purchase

- Is it a fixed named action ("Seal the hatch") that the player explicitly triggers, or whichever upgrade happens to be last in the tree? **open**

---

## Gameplay / Mechanics

### Money sources

- Income shape implied by the backstory: seed capital (baseline per-tick) → milestone-triggered government grants (lump sums) → public donation surge as launch approaches.
- Whether this is the actual mechanic or purely flavor **open**
- Exact income rates and milestone triggers **open**

### Upgrade tree

The upgrade tree includes upgrades for each AI (purchasing and upgrading each AI is part of Stage 1 progression). Full named purchase list **open**.

### Cost curve

- "Order of magnitude per tier" is the stated principle. Exact tier 1 cost and number of tiers **open**

### Resource: Ship construction %

A percentage that grows while building is in progress — not a direct purchase. Named checkpoints are displayed at key thresholds ("Hull finished", "Navigation system installed", etc.).

### Resource: People count

- Recruitment mechanic (per-click, per-tick, event-based), cost, unlock condition, and cap **open**

### Resource: Species count

- Acquisition mechanic, cost, pool, and cap **open**

### Resource: People qualities (cohesion, training %)

- Mechanical effect (multiplier, unlock gate, or narrative stat) **open**

### Resource: Species qualities (genetic diversity, fitness for travel)

Purely narrative stats. They are requirements for progressing — the player must reach target values to advance.

### Resource unlock sequencing

Order: Money → Ship construction % → People count → Species count → People qualities → Species qualities → Fuel and oxygen.

- What triggers each reveal (elapsed time, purchase threshold, percentage reached) **open**

### Stage win condition

All key resources must reach their targets. The final resource is **Launch Preparation**, which can only be filled after all other resources are at target. When Launch Preparation fills, Stage 2 begins.

---

## UI / Visual Design

### Visual style

- Terminal/monospace vs. warmer organic aesthetic. **open** — must be resolved before layout work begins.

### Signal indicator

Introduced later in the game, not in Stage 1.

### Money counter

- Presentation at absurd scale (billions → trillions → unnamed units): special formatting, colour shift, or named magnitudes? **open**

### Mobile layout

- 7+ resource panels unlock sequentially. Layout design (single-column card stack, expandable sections, etc.) **open**

---

## Technical

### Framework

- Vanilla JS + HTML/CSS or React **open**

### Tick rate

- Not specified **open**

