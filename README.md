# Idle Game Design — Iteration One

**Codename:** green-in-dark

## Overview
Planning for a series of idle/incremental games. First game should be simple and implementable in one week. Ideas may be earmarked for later games rather than forced into game #1.

---

## 1. Reference Games

- **Universal Paperclips** — minimalist, text-only, narrative arc with a clear ending. Gold standard for week-one scope.
- **Adventure Capitalist** — clean idle loop, very approachable, good example of simple multiplier progression.
- **Kittens Game** — deep resource chains, civilization-building feel, very long-form. Good reference for complex economy design.
- **Idle Breakout** — classic arcade mechanic (Breakout) as the idle engine. Shows how a familiar physical loop can drive an incremental game.
- **Trimps** — lots of interlocking systems but readable UI, good balance of automation and decision-making.
- **Antimatter Dimensions** — deep prestige layering, multiple reset mechanics stacked. Good reference for later games.
- **Prestige Tree** — modular, meta game about prestige mechanics. Useful for reset layer design thinking.
- **Leaf Blower Revolution** — great pacing of unlocks, distinct systems layered over time without feeling overwhelming.
- **Soda Dungeon 1 & 2** — idle RPG with team composition, equipment, dungeon crawling. Light strategy in the idle space.
- **Increlution** — idle RPG with roguelike flavor, character progression with resets.
- **Unnamed Space Idle** — space-themed, clean UI, dramatic but meaningful scale. Good reference for theming without heavy art.
- **BitBurner** — programmable idle, players write scripts to automate. Excellent later-game inspiration for a "meta automation" angle.
- **Pachinkremental** — physical simulation meets incremental, very visual and tactile.
- **Pincremental** — pinball as the idle engine, shows real-time physics driving a numbers game.

---

## 2. Idle / Clicker Balance

Mostly idle with a handful of meaningful manual actions early on, then full automation takes over. Avoid click-spam — one deliberate click per minute feels better than 60 mindless ones.

---

## 3. Mechanics

Core loop: resource generation → spend on multipliers → unlock new resource types → repeat.

Optional layers to consider: prestige reset, tech trees, conversion ratios that reward optimization.

**Week one:** 2–3 resource tiers and one upgrade tree. Save prestige for later games.

---

## 4. Player Involvement

Patient-friendly but optimizer-rewarding — you always progress, but smart players go 20–30% faster. Avoid gates that require wiki-diving. One or two "aha" moments where a non-obvious combo pays off is plenty.

---

## 5. Randomness

Minimal for game #1. Maybe one small random event (a windfall, a setback) every 10–15 minutes for texture. Avoid RNG that blocks progress.

---

## 6. Endless vs. Clear Finale

**Clear finale** recommended for game #1. Ends with a satisfying surprise, leaves players wanting more. Endless games are harder to pace and easier to abandon.

---

## 7. Multiplayer

Skip entirely for game #1. Even a leaderboard adds auth/backend complexity. Save for a later game where async competition is a core mechanic worth building around.

---

## 8. Platform

**Mobile web first, desktop browser second.** Zero install friction, easy to share. UI decisions prioritize touch:

- Large tap targets — finger-friendly buttons, no tiny upgrade rows
- Single-column or card layout — no wide multi-panel dashboards
- Minimal text input — everything tappable, not typed
- Readable numbers at a glance — abbreviations (1.2M, 4.5B) over long digit strings
- No hover states as primary UI — tap-equivalent fallbacks required
- Offline-friendly by design — mobile players close tabs constantly
- Portrait orientation assumed

---

## 9. Technologies / Engine

Vanilla JS + HTML/CSS, or React. No game engine needed. State is a JS object; `setInterval` drives the tick. LocalStorage for save state. No build pipeline required for week one.

---

## 10. Assets

Mostly text and CSS — lean into it aesthetically (monospace/terminal look, or clean minimal). Icons via emoji or a free icon set (Lucide, Heroicons). No sprites, no audio required for week one.

---

## 11. Testing

Manual playthroughs at 1x and 10x speed (add a dev speed multiplier). Unit test core math functions (production rates, cost curves). No full test suite needed for week one.

---

## 12. Playtesting / Bots

Write a simple headless bot that calls the game tick function in a tight loop — simulates hours of play in seconds, catches balance cliffs early. Two bots:
- **Dumb bot** — buys first available upgrade
- **Greedy bot** — always maximizes rate/cost ratio

---

## 13. Theme / Setting

**Green in the Dark** — a self-sustaining biodome spaceship carrying life and human passengers to a new planet.

### Three guiding principles
- **Positive and fun** — no grimdark, horror, or war. Rewarding and cheerful tone. Building something good.
- **Building / creating** — core fantasy is construction and growth, making something from nothing.
- **Moving / travelling / exploring** — progression feels like going somewhere, not just a number getting bigger.

### Core concept
Two intertwined loops:

**Loop 1 — The Ecosystem**
Build core life support systems (oxygen, water, soil, light). Each system unlocks new species. Species contribute back to the ecosystem — producing resources, stabilizing systems, unlocking further species. The ark grows from a bare shell into a thriving living world.

**Loop 2 — The Voyage**
Travel speed is the second progression axis. Speed comes from two sources:
- **Direct propulsion upgrades** — engines, fuel efficiency, hull improvements
- **Species discoveries** — certain species have unique travel benefits (bioluminescent algae improves solar energy absorption, nitrogen-fixing bacteria improves fuel yield). These feel like lucky discoveries rather than purchased upgrades.

A thriving ecosystem generates more energy, which powers faster engines — so building a better ark and travelling faster are the same goal approached from two directions.

### Energy source
The ecosystem is powered by **starlight**. Solar panels and adapted plants harvest light from nearby stars. Energy availability changes across voyage stages — abundant near stars, scarce in the void between them.

### The transformation arc
At launch the ark is a **technological object** — metal hull, chemical engines, artificial lighting, synthetic water recycling. But components degrade in space and can't be replaced. The ecosystem becomes the replacement:

- Artificial lighting fails → bioluminescent organisms take over
- Chemical water recycling degrades → moss and root systems filter naturally
- Metal hull corrodes → fibrous plants reinforce and eventually replace hull sections
- Chemical engines wear out → bio-engineered organisms produce thrust or harvest energy
- Synthetic insulation breaks down → dense canopy regulates temperature

Early game: maintaining technology, repairing and patching. Mid game: biological systems coming online as mechanical ones fail. Late game: the ark is almost entirely alive — a flying forest.

**The finale reframed:** when the ark reaches the new planet, it's not a spacecraft that lands — it's a living thing. The ark itself is the seed.

### Human passengers
The ship carries human passengers throughout the voyage. They are present and reactive — commenting on complications, celebrating solutions, watching the transformation from metal to forest with a mix of nervousness and wonder. They are the emotional heartbeat of the game.

### The complication model
Each stage introduces a problem that **slows or halts progress** until resolved. No permadeath, no catastrophic failure — just friction and a clear goal to achieve before moving on. Slow is the punishment, not death. Players always know what they're working toward.

- Each complication has a **clear exit condition** (hull integrity above X, shielding reached, species cultivated)
- A well-developed ecosystem sails through quickly; a neglected one crawls — optimizer-rewarding without hard gates
- Passengers react to each complication and its resolution

---

## 14. Voyage Stages

### Stage 1 — Home System

**Sub-stage 1a — Inner Planets**
Calm, familiar yellow starlight. Tutorial phase. Build the ecosystem, get engines running. Other planets visible — explorable for resources via probes. Ends when the outer planets are passed.

**Sub-stage 1b — The Oort Cloud**
Ice and rocks pelting the hull. Hull integrity introduced as a resource. Complication: hull damage accumulates and slows travel. Goal: build hull repair systems to a threshold. Silver lining: ice chunks harvested for **water**, rocky debris yields **minerals**.

---

### Stage 2 — Interstellar Void
Starlight fades to near zero. Energy income collapses. Plants struggle, engines slow. Complication: energy shortage stalls progress. Goal: cultivate low-light and radiation-harvesting species. Silver lining: cosmic radiation at low levels is harvestable by adapted species — forces a roster rethink. Eerily quiet tone.

---

### Stage 3 — Black Hole Proximity
Immense gravity slows travel dramatically. Time dilation: production ticks slow — or alternatively, offline gains increase (time outside moves faster). Complication: gravitational drag halts progress. Goal: harvest enough accretion disk energy to power through. Silver lining: accretion disk provides the richest energy harvest of the early game; gravitational lensing triggers **species mutations** exclusive to this stage; slingshot exit gives a permanent speed boost.

---

### Stage 4 — Pulsar Proximity
A rotating neutron star blasts periodic radiation pulses. Complication: unshielded pulses damage biological systems. Goal: build shielding to a threshold. Silver lining: enormous energy bursts harvestable between pulses — introduces a light timing mechanic (prep during quiet, harvest during pulse).

---

### Stage 5 — Asteroid Field
Denser and more dangerous than the Oort Cloud. Complication: heavy hull damage accumulates rapidly. Goal: hull integrity and repair rate above threshold to push through. Silver lining: rich rare minerals unlock the most powerful propulsion upgrades in the game.

---

### Stage 6 — Alien Encounter
First contact with an alien intelligence — curious, not hostile, travelling in the opposite direction. Complication: communication and trust-building takes time and resources. Goal: complete enough exchanges to unlock the full benefits. Silver lining: trade resources; exchange species (aliens have plants adapted to the destination star's wavelength — exactly what's needed for Stage 8); learn propulsion techniques that unlock a new engine tier. The emotional centrepiece of the game. Aliens may not recognise the ark as a ship at all — it looks too alive.

---

### Stage 7 — Hard X-Ray Zone
High-energy radiation from the destination star's outer halo. Complication: unprotected species go dormant, energy production drops. Goal: cultivate enough x-ray-resistant species to restore output. Silver lining: x-ray-resistant species are the most energy-efficient in the game — a painful but rewarding final ecosystem overhaul.

---

### Stage 8 — New Star Approach
The destination star emits a different wavelength of light. Old species underperform. Complication: energy production falls as familiar plants struggle. Goal: alien-traded and x-ray-adapted species now thrive — complete the transition. Engines peak on abundant new energy. The ark transforms one last time.

---

### Finale — Landfall
Landing sequence triggers. The living ark touches down. First seedling in alien soil — or perhaps the ark itself takes root. End screen.

---

## 15. Offline Mode

Capped offline progress (e.g. max 8–12 hours of gains). Easier to balance than true offline — avoids players returning to broken economies. Calculate time elapsed on load, apply capped production, show the player what they earned. That reveal moment is itself satisfying. Especially important as a mobile-first game — players close tabs constantly.

**Special case:** during the Black Hole stage, time dilation could invert this — offline gains are *increased* during this stage as a narrative flourish (time outside moves faster near the black hole).

---

## Open Questions

- Specific resource chain — needs detailing (energy, water, minerals, oxygen, biomass?)
- Species list — which species, what do they do mechanically?
- Upgrade structure — tech tree shape, cost curves
- Prestige mechanic — defer to game #2 or include in game #1?
- Visual style — terminal/monospace, or warmer organic aesthetic given the theme?
