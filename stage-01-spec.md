# Stage 1 — Pre-Launch: Specification

Working spec for implementing Stage 1. Open questions are marked **open**; answered ones get the answer inline. Cross-reference: [Design Notes](stage-01-prelaunch.md), [Theme](theme.md), [Gameplay](gameplay.md), [Technical](technical.md).

---

## Story / Narrative

### AI characters

- **When and how are the AIs introduced?** The four AIs (money, logistics, species cataloguing, psychology) are described in depth but Stage 1 has no plan for their introduction. Do they all appear from day one, or unlock as resources unlock? **open** **user note** after resource becomes available player clicks buttons several times then AI becomes available for purchase. Then it gtadually automates everything.
- **AI communication UI** — no design exists for how AIs communicate. Chat feed? Notifications? Ambient log? Mixed? **open** **user note** AI has a status, current task and progress indicator on current task.

### The billionaire

- **In-game presence** — his unexplained compulsion is the earliest echo of the signal, but there is no mechanism to surface it. Is he a named character? Does he appear (a founding message, a news ticker, a log entry)? **open**
- **Pre-signal foreshadowing** — the signal thread formally starts at Stage 4, but the billionaire's compulsion *is* the signal arriving before the ark existed to receive it. How (if at all) does Stage 1 plant that seed without naming it? **open**

### Passenger lines

- No specific lines are written for Stage 1. Need at least a handful — arrival, a comment on the scale of the build, something that establishes voice before launch. **open**

### The final purchase

- "The last thing bought before launch empties everything" is vivid. Is this a fixed named purchase (e.g. "Seal the hatch") that the player explicitly triggers, or whichever upgrade happens to be last? **open**

---

## Gameplay / Mechanics

### Money sources

- The sponsor backstory implies a natural income shape: seed capital to start → milestone-triggered government grants → public donation surge as launch approaches. Are these the actual mechanics, or just flavor?
- Is income passive (per-tick) or event-based (milestones unlock lump sums)? A hybrid — baseline per-tick income plus milestone bonuses — would match both the narrative and the "always calculating, always one purchase away" arc. **open**

### Upgrade tree

- The upgrade tree for Stage 1 is completely unspecified. What are the named purchases? Hull sections? Specimen bays? Fuel tanks? Crew quarters? This is the hardest unresolved item — nothing else can be balanced without it. **open** **user note** There are upgrades fo AIs.

### Cost curve

- "Order of magnitude per tier" is the stated principle. What does tier 1 cost? How many tiers are there in Stage 1? **open**

### Resource: Ship construction %

- Is construction % a direct purchase, or does it accumulate from buying sub-components (hull sections, systems, etc.)? **open** **user note** It's a percentage which grows when building is in progress. "Hull finished", "navigation system installed", etc are displayed at some checkpoints.

### Resource: People count

- How is recruitment triggered — per-click, per-tick, or event-based? Is there a cost? An unlock condition? What is the cap? **open**

### Resource: Species count

- Same questions as people count. Purchased? Donated? Found? What is the pool and the cap? **open**

### Resource: People qualities (cohesion, training %)

- Mechanical effect is undefined. Are these multipliers on some output, unlock gates for later content, or purely narrative flavour stats? **open**

### Resource: Species qualities (genetic diversity, fitness for travel)

- Same question. Mechanical effect undefined. **open** **user note** Those are purely for narrative and they are requirements for progressing.

### Resource unlock sequencing

- Resources unlock in order: Money → Ship construction % → People count → Species count → People qualities → Species qualities → Fuel and oxygen. What triggers each reveal — elapsed time, a purchase threshold, a percentage reached? **open**

### Stage win condition

- How does the player know Stage 1 is ending? Explicit checklist UI? Resources filling to a target? A final named action? **open** **user note** All important resources must be filled to a target. Last important resource in stage 1 is "launch preparation", it can be filled only after all other resources.
- Stage transition to Stage 2 trigger: what exact condition fires it? **open** **user note** When "launch preparation" is filled, we transition to stage 2.

---

## UI / Visual Design

### Visual style

- Terminal/monospace vs. warmer organic aesthetic. Listed as open in the technical spec. This decision affects everything else — should be resolved before layout work begins. **open**

### Signal indicator

- Described as "barely registers" in early game. Should it be visible from Stage 1 (priming curiosity) or introduced at a later stage? **open**  **user note** introduce later in the game

### Money counter

- The absurd scale (billions → trillions → unnamed units) is a core design intention. Does the counter change its presentation as numbers become surreal? Special formatting, colour shift, or unit labels for unnamed magnitudes? **open**

### Mobile layout

- The resource unlock sequence adds 7+ resource panels. Single-column card stack? Expandable sections? No layout design exists yet. **open**

---

## Technical

### Framework

- Vanilla JS + HTML/CSS or React. Listed as TBD in the technical spec. **open**

### Tick rate

- Not specified. **open**
