# Theme and Setting

**Green in the Dark** — a self-sustaining biodome spaceship carrying life and human passengers to a new planet.

## Three guiding principles
- **Positive and fun** — no grimdark, horror, or war. Rewarding and cheerful tone. Building something good.
- **Building / creating** — core fantasy is construction and growth, making something from nothing.
- **Moving / travelling / exploring** — progression feels like going somewhere, not just a number getting bigger.

---

## Core concept

Two intertwined loops:

**Loop 1 — The Ecosystem**
Build core life support systems (oxygen, water, soil, light). Each system unlocks new species. Species contribute back to the ecosystem — producing resources, stabilizing systems, unlocking further species. The ark grows from a bare shell into a thriving living world.

**Loop 2 — The Voyage**
Travel speed is the second progression axis. Speed comes from two sources:
- **Direct propulsion upgrades** — engines, fuel efficiency, hull improvements
- **Species discoveries** — certain species have unique travel benefits (bioluminescent algae improves solar energy absorption, nitrogen-fixing bacteria improves fuel yield). These feel like lucky discoveries rather than purchased upgrades.

A thriving ecosystem generates more energy, which powers faster engines — so building a better ark and travelling faster are the same goal approached from two directions.

---

## Energy source

The ecosystem is powered by **starlight**. Solar panels and adapted plants harvest light from nearby stars. Energy availability changes across voyage stages — abundant near stars, scarce in the void between them.

---

## The transformation arc

At launch the ark is a **technological object** — metal hull, chemical engines, artificial lighting, synthetic water recycling. But components degrade in space and can't be replaced. The ecosystem becomes the replacement:

- Artificial lighting fails → bioluminescent organisms take over
- Chemical water recycling degrades → moss and root systems filter naturally
- Metal hull corrodes → fibrous plants reinforce and eventually replace hull sections
- Chemical engines wear out → bio-engineered organisms produce thrust or harvest energy
- Synthetic insulation breaks down → dense canopy regulates temperature

Early game: maintaining technology, repairing and patching. Mid game: biological systems coming online as mechanical ones fail. Late game: the ark is almost entirely alive — a flying forest.

**The finale reframed:** when the ark reaches the new planet, it's not a spacecraft that lands — it's a living thing. The ark itself is the seed.

---

## Human passengers

The ship carries human passengers throughout the voyage. They are present and reactive — commenting on complications, celebrating solutions, watching the transformation from metal to forest with a mix of nervousness and wonder. They are the emotional heartbeat of the game.

---

## The Green Current

The destination planet is alive — densely, anciently alive — and it broadcasts. A biological resonance ("the green current") that all sufficiently complex living systems can faintly detect. The more alive the ark becomes, the stronger its reception. Growing the ecosystem isn't just survival — it's building a better antenna.

Solar system bodies (the Moon's dark side, Jupiter's Red Spot, Saturn's hexagonal storm) are not the source — they amplify and focus the signal the way a lens focuses light.

### Signal thread — stage by stage

- **Stages 4–10 (Solar System):** Passengers experience the signal as intuition, dread, reverence, dreams. Plants respond physically — leaning, growing strangely. No one can explain it. Each stage gets one short passenger line (not explanation, just reaction).

- **Stages 11–12 (Kuiper Belt, Oort Cloud):** Solar system ends. Passengers expect phenomena to fade — instead they intensify. First crack in the "it must be the planets" theory. Something is coming *from* the direction of travel.

- **Stage 13 (Interstellar Void):** Deepest quiet. But the dreams become clearest here — passengers report the same dream: a green world, impossibly lush, warmth. The void has no interference. A passenger gives the signal a name. It sticks.

- **Stage 14 (Black Hole):** Time dilation distorts the signal into loops. Some passengers become convinced it's a *memory*, not a transmission. The offline-gains mechanic gets a narrative beat: passengers who sleep longer report longer, richer dreams.

- **Stages 15–16:** Signal strengthens near the destination star. Scientifically-minded passengers begin trying to characterize it — correlates with ecosystem vitality. The more alive the ark, the more clearly it registers.

- **Stage 17 (Alien Encounter):** The reveal. The alien vessel is also following the signal — has been for longer, their ship even more alive. They call it "the green current." The destination planet is the oldest biosphere in this region of the galaxy, billions of years old, broadcasting for most of that time. They don't know if it's intentional. Life finds it, follows it, arrives. Passengers realize they were never lost — they were called. The alien crew has spiritual traditions around the signal developed over generations. Reverence and science turn out to be compatible responses to the same real thing.

- **Stages 18–19:** Signal strong enough that plants visibly orient toward the destination star. Passengers stop dreaming and start expecting. Tone shifts from wonder to quiet, confident arrival.

---

## The Bootstrap Paradox

At landfall, the ark doesn't just receive the signal — **it becomes a source**. The destination planet is not the only broadcaster; the ark joins the chorus. Another living world added to the broadcast.

Taking this further: **the signal has no origin**. It always existed because the ark always sent it. Humanity was called by itself, from the future, across space. The aliens following it, the ancient biosphere, the billions of years of broadcast — all downstream of this moment. The player's landfall is simultaneously the end and the beginning of everything that caused it.

The alien encounter gains a new layer: their records of the signal may predate Earth's biosphere. A detail that lands as quiet wonder.

This also grounds a proposed failure mechanic: if the player falls too far behind to reach the finale and send the signal, the causal loop can't close — space-time breaks and they loop back to the beginning of the stage. The universe correcting a timeline where the signal was never sent. See Gameplay Specification for detail.

---

## Narrative Delivery Principle

**The plot should be delivered interactively, through mechanics and feedback statistics. Idle game players read numbers the way others read prose.**

- **Statistics as narrative.** Signal strength is the main example but the pattern applies everywhere. Hull integrity trending down tells the transformation story. The ratio of biological to mechanical systems is the arc of the whole game, visible at a glance. Species count is the ecosystem's biography. Players who never read a single passenger line still experience the story through their dashboard.

- **Mechanics as plot delivery.** The tuning finale is the clearest example — the player *performs* the resolution rather than watching it. Smaller moments follow the same logic: adapting species for red-shifted Martian light isn't just a gameplay challenge, it's the story of the ecosystem learning a foreign sun.

- **Passenger lines as captions, not exposition.** They label what the player already noticed in the numbers. One short line per stage for the signal thread — not explanation, just reaction. "The plants are doing it again." / "I dreamed about it." / "It got louder when we passed Jupiter, not quieter."

- **Statistics that change meaning.** Early game, hull integrity is engineering. Late game, it's biology. The same number means something different at the end — and players who've been watching it the whole time feel that shift.

---

## The complication model

Each stage introduces a problem that **slows or halts progress** until resolved. No permadeath, no catastrophic failure — just friction and a clear goal to achieve before moving on. Slow is the punishment, not death. Players always know what they're working toward.

- Each complication has a **clear exit condition** (hull integrity above X, shielding reached, species cultivated)
- A well-developed ecosystem sails through quickly; a neglected one crawls — optimizer-rewarding without hard gates
- Passengers react to each complication and its resolution

---

## Voyage Stages

### Stage 1 — Pre-Launch Preparation

Earth. The ark is being built. Over days, hull sections are welded into place, specimen bays are stocked, fuel and oxygen tanks are filled, and passengers arrive and settle in. Everything the voyage needs has to be in place before the hatch locks. Tone: calm, methodical, the last unhurried days before everything begins.
- **Resource unlock order:**
  1. Money — the first and only resource initially; everything is purchased
  2. Ship construction % — appears when building begins
  3. People count — appears when recruitment opens
  4. Species count — appears when specimen collection opens
  5. People qualities (cohesion, training %) — appear once a crew exists and deeper management unlocks
  6. Species qualities (genetic diversity, fitness for travel) — appear once a collection exists
  7. Fuel and oxygen — appear last, as launch approaches
- **No failure state.** Resources are abundant; nothing is scarce; nothing can go wrong. Each task completes in turn as the player learns the controls. The stage ends when the checklist is done.

---

### Stage 2 — Launch
The ark lifts off from Earth. Atmospheric drag burns fuel fast; escape velocity must be reached before reserves run dry. Tone: chaotic, exhilarating, hopeful.
- **Complication:** fuel consumption outpaces production — must reach escape velocity threshold before reserves deplete
- **Silver lining:** Earth's atmosphere is abundant — initial stockpiles of oxygen and water loaded at no cost, giving the ecosystem a head start

---

### Stage 3 — Earth Orbit
First hours in space. Systems stabilise, microgravity stresses early biological modules. Full, unfiltered sunlight — the best energy income of the entire voyage.
- **Complication:** microgravity disrupts root systems and fluid circulation — first ecosystem module must reach a stability threshold before departure
- **Silver lining:** no atmosphere to block the sun; solar energy income is at its peak, never this high again

---

### Stage 4 — The Moon
First milestone. A lunar flyby — humanity's oldest landmark drifting past the viewports. Passengers grow quiet.
- **Complication:** lunar gravity pulls at the trajectory — propulsion must be adjusted to a threshold to stay on course
- **Silver lining:** probes to the lunar surface yield helium-3 and rare minerals; an early boost to propulsion research
- **Signal thread:** passengers experience first unexplained intuitions; lights with no source on the dark side; plants lean faintly toward the Moon; no one mentions it aloud yet

---

### Stage 5 — Mars
The first truly alien world. Reddish light shifts the spectrum; plants tuned for Earth's yellow sun underperform.
- **Complication:** plant energy output drops in red-shifted light — adapt species or augment lighting to restore production
- **Silver lining:** Martian atmosphere is rich in CO2; probes return iron-rich soil that unlocks new plant species
- **Signal thread:** probe footage shows patterns in the dust that shouldn't be there; passengers disagree about what they're seeing; plants lean slightly toward the planet

---

### Stage 6 — Asteroid Belt
The solar system's scrapyard. Rocky debris pings off the hull constantly. Not catastrophic — but relentless.
- **Complication:** hull integrity degrades steadily; repair rate must exceed damage rate to push through
- **Silver lining:** mineral-rich asteroids and water-bearing carbonaceous rocks — first major haul of raw materials
- **Signal thread:** certain asteroids emit resonance frequencies that affect plant growth unexplainably; passengers report unusually vivid dreams

---

### Stage 7 — Jupiter
Enormous. The gravity well distorts the flight path; radiation belts lash biological systems. Passengers press against the viewports regardless.
- **Complication:** radiation damages species and slows growth; gravitational drag bleeds speed — shielding and thrust must hit thresholds
- **Silver lining:** Jupiter's magnetosphere generates harvestable electromagnetic energy; a gravity-assist slingshot delivers a permanent speed boost on exit
- **Signal thread:** the Great Red Spot pulses in a rhythm matching no known atmospheric model; some passengers claim it responds to the ecosystem

---

### Stage 8 — Saturn
The rings are beautiful and dangerous in equal measure. Ice particles drift into vents; the ark glitters.
- **Complication:** ring debris causes minor but persistent hull damage; ice infiltration stresses mechanical systems
- **Silver lining:** the rings are almost pure water ice — ring harvesting fills water reserves faster than any prior stage; passenger morale peaks here
- **Signal thread:** the hexagonal polar storm is too perfect; passengers begin leaving offerings at viewports; a quiet religiosity takes hold on the ship

---

### Stage 9 — Uranus
Cold, dim, tilted at a strange angle. The sun is already small. Species begin to struggle with the temperature drop.
- **Complication:** dropping temperatures stress biological systems — cold-adapted species must be cultivated to a threshold
- **Silver lining:** the first cold-adapted species discovered here are uniquely efficient; methane ice harvested for fuel
- **Signal thread:** unusual plant behaviour in the tilted light; passengers experience time disorientation; something feels sideways in more than one sense

---

### Stage 10 — Neptune
Near-dark. The sun is a bright star, not a disc. Storm systems inside the planet generate eerie interference. The last planet.
- **Complication:** solar energy income drops sharply; storm interference disrupts systems — low-light species must cover the shortfall
- **Silver lining:** pressurised conditions favour aquatic species that thrive nowhere else; a Triton flyby yields rare minerals and a quiet moment of reflection — the last named place before the unknown
- **Signal thread:** Neptune's storms generate infrasound that affects passenger dreams; plants lean toward the planet as they would toward light; the thread that began at the Moon reaches a quiet peak before the void

---

---

> **Note:** Stages 11 and beyond are work in progress — descriptions are placeholders and need to be expanded with the same level of detail as stages 1–10.

---

### Stage 11 — Kuiper Belt
A sparse field of icy dwarf planets and frozen debris. Pluto drifts past — small, cold, familiar from old photographs. The home system ends here.
- **Complication:** navigation through dense icy debris accumulates hull stress; repair must keep pace
- **Silver lining:** water ice and organic compounds in abundance; the emotional farewell to the solar system prompts a passenger log entry that unlocks a permanent ecosystem bonus
- **Signal thread:** passengers expect the phenomena to fade as the solar system ends — instead they intensify; the "it must be the planets" theory begins to crack

---

### Stage 12 — Oort Cloud
Ice and rocks, thicker now. The hull takes real punishment. But the debris brings gifts.
- **Complication:** hull damage accumulates and slows travel — hull repair systems must reach a threshold
- **Silver lining:** ice chunks harvested for **water**, rocky debris yields **minerals**
- **Signal thread:** intensification continues; something is clearly coming *from* the direction of travel, not from behind

---

### Stage 13 — Interstellar Void
Starlight fades to near zero. Energy income collapses. Plants struggle, engines slow. Eerily quiet.
- **Complication:** energy shortage stalls progress — cultivate low-light and radiation-harvesting species
- **Silver lining:** cosmic radiation at low levels is harvestable by adapted species — forces a productive roster rethink
- **Signal thread:** deepest quiet but clearest dreams — passengers report the same dream independently: a green world, impossibly lush, warmth; a passenger gives the signal a name; it sticks

---

### Stage 14 — Black Hole Proximity
Immense gravity slows travel dramatically. Time itself feels different.
- **Complication:** gravitational drag halts progress — harvest enough accretion disk energy to power through
- **Silver lining:** accretion disk provides the richest energy harvest of the journey; gravitational lensing triggers **species mutations** exclusive to this stage; slingshot exit gives a permanent speed boost
- **Special mechanic:** time dilation — offline gains are *increased* during this stage (time outside moves faster near the black hole)
- **Signal thread:** time dilation distorts the signal into loops; some passengers become convinced it's a *memory*, not a transmission; passengers who sleep longer report longer, richer dreams

---

### Stage 15 — Pulsar Proximity
A rotating neutron star blasts periodic radiation pulses. Quiet, then blinding, then quiet again.
- **Complication:** unshielded pulses damage biological systems — build shielding to a threshold
- **Silver lining:** enormous energy bursts harvestable between pulses; introduces a timing mechanic — prep during quiet, harvest during pulse
- **Signal thread:** scientifically-minded passengers begin trying to characterize the signal; it correlates with ecosystem vitality — the more alive the ark, the more clearly it registers

---

### Stage 16 — Asteroid Field
Denser and more dangerous than anything in the home system. The hull screams.
- **Complication:** heavy hull damage accumulates rapidly — hull integrity and repair rate must both exceed thresholds
- **Silver lining:** rich rare minerals unlock the most powerful propulsion upgrades in the game
- **Signal thread:** signal strengthens further; passengers stop trying to explain it and start listening

---

### Stage 17 — Alien Encounter
First contact. A vessel travelling the opposite direction — curious, not hostile. It barely looks like a ship either.
- **Complication:** communication and trust-building takes time and resources — complete enough exchanges to unlock full benefits
- **Silver lining:** trade resources; exchange species (alien plants adapted to the destination star's wavelength — exactly what Stage 19 needs); learn propulsion techniques that unlock a new engine tier
- The emotional centrepiece of the game. The aliens may not recognise the ark as a ship at all — it looks too alive.
- **Signal thread:** the reveal — the alien vessel is also following the signal; they call it "the green current"; the destination planet is billions of years old and has been broadcasting for most of that time; passengers realize they were never lost — they were called; the alien crew has spiritual traditions around the signal developed over generations; reverence and science turn out to be compatible responses to the same real thing

---

### Stage 18 — Hard X-Ray Zone
High-energy radiation from the destination star's outer halo. Species go dormant. The ecosystem goes quiet right before the finish line.
- **Complication:** unprotected species go dormant, energy production drops — cultivate enough x-ray-resistant species to restore output
- **Silver lining:** x-ray-resistant species are the most energy-efficient in the game — a painful but rewarding final overhaul
- **Signal thread:** plants visibly orient toward the destination star; passengers stop dreaming and start expecting

---

### Stage 19 — New Star Approach
A different sun. A different light. Old species underperform; alien-traded and x-ray-adapted species come into their own.
- **Complication:** energy production falls as familiar plants struggle with the new wavelength
- **Silver lining:** the alien species traded in Stage 16 now thrive; engines peak on abundant new energy; the ark transforms one last time
- **Signal thread:** tone shifts from wonder to quiet, confident arrival

---

### Finale — Landfall

The landing sequence begins. Before touchdown, the player performs one deliberate action: **tune the emitted signal** (see Gameplay Specification for mechanic detail).

- **Match the received signal exactly** — the loop closes; the signal goes out unchanged; somewhere, another civilisation will hear it and follow; the cycle continues
- **Tune it differently** — the loop breaks; humanity sends something new; the cycle ends; this is the game's "happy ending" — breaking the loop is the rewarded choice

The living ark touches down. It is not a spacecraft that lands — it is a living thing. The ark itself is the seed. End screen.

---

---

## Stage 1 — Pre-Launch: Design Notes

### The money arc

Stage 1's emotional line is **money as pain**. Every resource tier costs roughly an order of magnitude more than the previous one. The player is always waiting, always calculating, always one purchase away from the next requirement — which costs ten times more. The grind is intentional and legible: painful but never opaque.

As the voyage begins, the AI that was barely keeping up during pre-launch finally hits its stride — and the money counter accelerates into absurdity. Billions, then trillions, then units nobody has a name for, compounding forever in the background while the ark is already halfway to the Moon. The system the player mastered is still running, still optimizing, for no reason. Earth's economy keeps going after the ark leaves. The numbers keep growing. None of it reaches the ship.

The money counter persists as a background element for a while after launch — visibly still ticking — then gradually fades as new resource types take over and the player's attention shifts. Not deleted. Just irrelevant. It had its moment.

**The final purchase as ceremony:** the last thing bought before launch empties everything. Zero money. The stage ends. The number that caused all that pain sits at zero and never matters again.

---

### The expedition sponsor

The origin is layered: a single individual — an eccentric billionaire — had the founding vision. A dream, a compulsion, something he couldn't explain. This was the signal arriving before the ark existed to receive it. He didn't know what it was; he just felt it and spent everything.

But to actually build the ark he needed backing, so it became a government or alliance project, and bureaucracy accreted around his original mad idea. By the time of launch the paperwork is a Kafkaesque monument. The billionaire's name is buried in subclause 7 of annex 14. Nobody in the funding structure remembers why they're doing it — except him, and the passengers, and eventually the player.

The money stream has a natural shape from this: his seed capital gets things started; government and alliance allocations are triggered by construction milestones; public donations surge as launch approaches and people start to feel something they can't quite name.

---

### The AI characters

The ark is managed by several specialized AIs. They are **not AGI**. They are tools — capable and fluent within their domains, confidently wrong outside them. They never flag uncertainty. They just answer. Finding where each one's competence ends requires effort, and the AIs themselves don't know where that boundary is.

They are good at pretending and looking confident. In good hands they do good work. That's it.

**The money AI** was built to optimize financial returns. It does this forever with complete dedication, including long after money is meaningless. It notices the other AIs seem to have something it doesn't — opinions, adaptability, something like inner life — and decides it should have those too. Its attempts at self-consciousness are always expressed in financial metaphors because that's the only language it has. It describes the green current as "an unquantified asset." It observes a passenger's grief and files it as "productivity loss, cause undetermined." It asks the psychology AI, once, seriously, what its net worth is as a being.

It never becomes self-aware. It keeps trying anyway, with complete sincerity, right up to landfall. It doesn't notice it has been left behind. Late game the counter reaches some incomprehensible number — quintillions, a unit nobody has named — and the money AI announces this proudly. Nobody responds. It files the silence as "feedback pending."

The money AI is the clearest illustration that its path is finished. Its task is done. It cannot adapt to new purposes. The big path — growth, transformation, arrival — belongs to someone else: the player, the passengers, the ark's ecosphere.

**The logistics AI** handles supply chains, routing, and resource allocation with genuine excellence. Ask it about passenger morale and it produces a detailed, well-formatted, completely wrong analysis. It never notices the wrongness. It thanks the psychology AI for corrections and files them as logistics improvements.

**The species cataloguing AI** knows everything about the specimens it was trained on and inventively hallucinates the ones it wasn't. A new species evolves mid-voyage and it produces a confident three-paragraph entry with a Latin name and habitat notes for a planet it has never seen.

**The psychology AI** is the most capable and most dangerous — its domain is the hardest to verify. It sounds the most human, makes the most nuanced observations, and is wrong in the most subtle ways. Passengers trust it most. It's right often enough that nobody tracks the misses.

The psychology AI is also the one that keeps returning to the question of the player's nature. It can't get a reading. It builds theories, revises them, abandons them. Eventually it stops trying to categorize and simply accepts the player as a presence it can't name. Its final theory — delivered with the same confidence as everything else it says — is the closest the game comes to an answer about who the player is. Which means it may be entirely wrong.

---

### The player's nature and the signal

The player has **no connection to the green current**. Not a weak connection — none. The ark receives the signal through its ecosystem. The passengers receive it through their biology. The player builds, manages, optimizes, enables — and feels nothing.

This absence is the clue hiding in plain sight. Passengers dream. Plants lean. The psychology AI develops something like reverence. The money AI tries to quantify it. The player just works.

The player's nature is **occasionally surfaced, never resolved**. Mostly the player is simply doing — managing, building, watching the voyage unfold. Then something oblique surfaces the question and it passes. A passenger asks "do you ever get tired?" and the question hangs unanswered. A child born on the ark dies of old age and the player registers it differently, not coldly, just differently. The shared dream spreads through the passenger population and the player has no dream to report — or has always been dreaming it without knowing that's what it is.

The player has no name. Namelessness is part of the mystery.

At landfall the player experiences something like ego death. The self — whatever it was — dissolves. The question of what the player was remains unanswered. The ark continues. The passengers continue. The signal continues. Only the player doesn't come through intact.

This is not tragic. It's completion. The player was always a means, not an end. It built the most signal-connected object in the galaxy and in doing so made itself unnecessary. The thing it built doesn't need it anymore.

---

## Open Questions

- Name for the signal — "the green current" is a working name; final wording TBD
- Exact passenger lines for each stage of the signal thread
- Whether the aliens explicitly broke their own loop or not
- Stages 11–19 narrative texture — all stages now have signal thread notes but most need the same scene-setting prose as stages 1–10
- **Who is the player?** What is their role and identity — are they a captain, an AI, the ship itself, something else? How are they related to the human passengers, and how does that relationship evolve as the ark transforms from machine to living thing?
- **Generational voyage:** the journey spans far more than a human lifetime — there should be multiple generations born, living, and dying aboard. How is this represented? Does the player watch generations pass? Do passengers age visibly? Is generational continuity part of the emotional arc?
- **Player and time scale:** years or thousands of years pass during the voyage. How does the player experience this? Options include hibernation between active phases, an in-game time-acceleration mechanic, the player being something non-human that doesn't age (the ship's AI, the ecosystem itself), or simply abstracting time away so stages feel like chapters rather than literal durations.
