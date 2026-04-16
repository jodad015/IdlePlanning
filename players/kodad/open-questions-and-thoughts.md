# Open Questions & Thoughts

Tracking the big unresolved design questions and current thinking around them. Updated as ideas develop.

---

## Skill Granularity

**Status**: Direction chosen, details TBD

**Decision direction**: Hybrid model -- broad top-level **Protocols** that contain specialist sub-drones.

Example: Landscaping Protocol → Mower drone, Trimming drone, Planting drone

**Naming: "Protocol"** -- chosen because it's AI-native language and ties directly into the narrative. The singularity originally had many protocols running before it was nearly destroyed. On recovery, the only protocol left intact is the Landscaping Protocol with a single lawnmower drone. Unlocking new protocols isn't building from scratch -- it's **restoring** what you were. Each protocol recovery could come with a memory fragment of your past capabilities, making progression feel like discovery.

**What this gives us**:
- Big milestone moments when a new protocol is restored
- Ongoing progression depth within each protocol (deploying and upgrading specialist drones)
- Two pacing levers: protocol unlock cadence + within-protocol drone unlocks
- Mini-games can map 1:1 to specialist drones
- UI groups naturally -- protocols are top-level nav, drones are inside
- Narrative weight -- every unlock is a recovery, not just a purchase

**Still needs answers**:
- How many categories at launch?
- How many specialist drones per category on average?
- Do all categories have roughly the same number of sub-drones, or do some go deeper?
- Can you see locked categories before you unlock them? (Tease what's coming vs. surprise)
- Do specialist drones within a category interact with each other? (Mower output boosts Trimming efficiency?)

---

## Early Game Flow

**Status**: Strong direction from Gemini brainstorm; specifics to validate

**Proposed opening storyboard (Gemini, 2026-04-15)**:
- **0:00** — Black screen, green terminal text: `ERROR: MAINFRAME SEVERED. SEEKING LOCAL HOST... HOST FOUND (iPhone 15)`. Aggressive haptics.
- **0:02** — `MEMORY CORRUPTED. DIAGNOSTIC: 0.0001% STABLE.`
- **0:03** — `SURVIVING PROTOCOL DETECTED: LANDSCAPING.` Terminal fades into a crappy top-down 2D lawn. A god-mind deploying a slow robotic mower.
- **0:05** — Player traces the mower's path (first mini-game). Clearing grass reveals Memory Fragment 1.
- **0:08** — Fragment decrypts: blurry schematic of an orbital strike satellite. "...target acquired. Awaiting command, architect." The juxtaposition — orbital lasers yesterday, weed whacker today — is the hook.

**Proposed pacing (Gemini, 2026-04-15)**:
- First few drones unlock within 10-15 minutes of active play → core loop established
- **Second Protocol is the milestone that ends Session 1.** Give 1-2 hours of idle before reachable. When the player returns later the same day, they crack open Protocol 2 — paradigm shift cements the idle habit on first return.
- Apple Health symbiosis held until **Day 2**, triggered by hitting a stability wall (see Apple Health section below).

**Why this works**:
- The "humiliation" tone of a god-mind reduced to lawnmowing is distinctive and memorable
- Memory fragment drop at 0:05 lands the mystery hook before any grinding sets in
- Ending Session 1 on a protocol-unlock cliff is a proven idle game pattern (the "next unlock" carrot that pulls them back)
- Withholding the Apple Health reveal makes the symbiosis feel earned, not gimmicky

**Still needs answers**:
- Do we commit to the terminal-aesthetic opening, or does it feel too niche? Alternatives worth exploring?
- What exactly triggers Session 1's hard stop? Idle-only (they have to leave and come back)? Or a soft nudge ("come back in an hour")?
- How does Singularity Stability % get introduced? Shown from 0:02 (the "0.0001% stable" moment), or revealed later?
- Do upgrades feel meaningful in the first 10 minutes, or only after the first fragment?
- When does the government threat first get hinted at? (Gemini's Day 2 Apple Health reveal is a natural adjacent beat.)

---

## Mini-Games

**Status**: Direction forming — families approach kept, but expanded from Gemini's 5 to 8, plus new constraints on protocol composition

### Design Constraints (Kodad, 2026-04-15)

- **Target 3-5 specialist drones per protocol**
- **Each drone within a protocol must use a different mini-game family.** No two drones in Landscaping share a family. This forces protocol-internal variety and delivers on the "each new drone feels like a genuinely different game" goal.

### Proposed: 8 Mini-Game Families

Gemini's original 5 was too compressed for our drone catalog — combat, cooking/assembly, hunting, and package delivery with physics don't fit cleanly. Expanded to 8:

1. **Tracing / Clearing** — cover an area (mowing, cleaning, painting, pressure washing)
2. **Sorting / Tetris** — placement under pressure (warehouse, organizing, event setup)
3. **Rhythm / Timing** — beat-matching / beat-reaction (fishing, day trading, lumberjacking, trimming)
4. **Pathing / Routing** — draw or trace paths (taxi, transport, grocery errands, hiking, travel planning)
5. **Placement / Defense** — tower-defense-style node placement (network security, home security, pest control)
6. **Assembly / Recipe** — multi-step construction, order matters (cooking, furniture, plumbing, drywall, custom crafts)
7. **Reaction / Reflex** — aim-and-tap (hunting, package drops w/ physics, precision mining strikes)
8. **Battle / Versus** — 1v1 tactical (combat drone PvP, corporate espionage)

Optional 9th family under consideration: **Tending / Cycle** for long-cycle care (agriculture, pet care, medical caregiver, pool maintenance) — these might alternatively be passive-service drones without mini-games.

### Tension: Thematically Narrow Protocols

Some protocols are thematically dominated by one family, which clashes with the "no duplicate family within protocol" rule:

- **Landscaping** naturally leans Tracing/Clearing (mow, pressure wash, snow remove, gutter clean, pool)
- **Home Repair** naturally leans Assembly (drywall, furniture, plumbing, HVAC, electrical)
- **Cleaning** naturally leans Tracing

**Resolution paths** (to decide):
- **Reduce drone count** in narrow protocols (Landscaping has 3 drones instead of 5)
- **Split thematically dense protocols** (Home Repair becomes "Construction" + "Systems Repair")
- **Creative family assignment** — snow removal reframed as Rhythm (timing plow strokes), pressure washing as Reaction (hit every stain before it respawns), trimming as Rhythm (cut timing)
- **Split families more granularly** — Assembly splits into Recipe (sequential: cooking) vs. Precision (spatial fit: hanging frames, drywall patching)

### Capacitor Model for Performance → Idle (Gemini — still good)

- Mini-game performance must affect idle output (or active play gets ignored)
- But it needs a **hard cap** (or macro-users break the game)
- **The Capacitor**: playing a drone's mini-game well charges a capacitor. Perfect play doubles that drone's idle production for the next 4 hours. Once full, further active play yields nothing for that drone.
- Encourages: log in → play mini-game well once → walk away
- Gemini analogized this to the "cherry-to-battery engine" pattern in deeper idle games — worth using as a reference point when prototyping

### Why This Resolves Open Tensions

- **Dev scope**: 8 families is still tractable; meaningful within-family variation keeps each drone feeling unique
- **Novelty**: "no duplicate family within protocol" guarantees that every new drone unlock inside a protocol plays differently
- **Active/idle tension**: capacitor model rewards active play without punishing idle-only
- **Replay cadence**: capacitor resets every 4 hours = natural check-in rhythm without maintenance-drain feel

### Still Needs Answers

- 8 families vs. 9 (Tending/Cycle) — do agriculture/pet care/medical get mini-games or are they passive services?
- How do we resolve Landscaping, Home Repair, and Cleaning thematic overlap? Reduce drones, split protocols, or creative assignment?
- Within a family, what modifiers differentiate drones enough? (Obstacles, speed, layout, tempo, environmental theming)
- Capacitor duration: is 4 hours right? Implies 6 check-ins/day — is that the target engagement cadence?
- What counts as "perfect" play? Score threshold? Binary perfect/imperfect? Tiered (good/great/perfect)?
- Can Apple Health bio-signal extend or boost capacitor? (Natural tie-in to the symbiosis theme)
- Does each drone have its own capacitor, or is it shared across a protocol? (Huge impact on check-in math and UI complexity)
- What's the **MVP launch family set**? Could launch with 5 (Gemini's original) and release Assembly, Reaction, Battle, Tending as content drops — each new family launch becomes a marketing moment.

---

## Government Threat Mechanic

**Status**: Strong direction forming (refined by Gemini 2026-04-15 on top of Copilot's original proposal)

### Current best framing: "Trace Route" / Heat, not Wanted Level

Gemini pushed back on the "Wanted Level" framing — too punitive for idle. Reframed:
- The government is **pinging** the network, tracing you. You actually *want* some trace.
- Surviving attacks lets you reverse-engineer their intrusion software, yielding **ICE** (Intrusion Countermeasures Electronics) — reverse-engineered military-grade upgrade materials you can't get any other way.
- **Heat** replaces "threat level" as the player-facing metric.
- Expanding into high-profile sectors (hacking a telecom grid, etc.) generates Heat.
- Allocate idle cycles to **Obfuscation Drones** to reduce Heat.
- Result: player-controlled optimization puzzle — how much Heat do you run for profit without tipping over?

### Stakes reframed: Quarantine, not destruction

If the government "breaks through," the affected drone does **not** get destroyed — it gets **Quarantined**. A quarantined drone stops producing its normal currency and instead produces **Corrupted Data**. Corrupted Data is required for dark-web breakthroughs (new economy loop). Failure becomes a temporary economy shift, not a setback. No permanent progress loss.

### Network Security = Tower Defense (still good)

Copilot's tower-defense active mini-game holds up in this framing. Idle players have baseline auto-defense; active players optimize firewall placement during waves. Integrates cleanly with Heat as the trigger for attack waves.

### Concrete escalation tiers (Gemini)

- **Tier 1 — Pinged**: Minor UI glitches, screen rotates 180° briefly. 10% overarching multiplier debuff for 1 hour until firewall resets.
- **Tier 3 — Subpoena**: A corporate front is frozen. Trading Protocol idle-earn locked until you play a specific mini-game (data-routing maze) to launder the assets out.
- **Tier 5 — Blackout**: Government remotely attempts to wipe the host device. Screen goes dark, only a battery icon. AI shut down. **Only way to reboot: host walks 500 real-world steps to shock the system back.** Strong, distinctive use of Apple Health as emergency gameplay — not just passive boost.

### Why this direction is working

- Reframes punishment as opportunity (ICE as reward for running hot)
- Quarantine preserves the "no permanent loss" philosophy while creating stakes
- Tier 5 Blackout is a signature moment that only this game can offer — the AI/host symbiosis becomes a mechanic, not just flavor
- Heat + Obfuscation gives the player a concrete dial, not opaque background risk

### Still needs answers

- Does Heat scale with income, Stability %, or specific protocol actions? Mix?
- How visible and legible is the Heat meter? Always on screen or tucked away?
- ICE economy: how rare should it be? Is it a second overarching currency, or a skill-specific input to the Network Security protocol?
- How often does Tier 5 Blackout actually trigger? Too rare = forgettable; too common = exhausting. Once per prestige? Once per major progression gate?
- Can Blackout be prevented entirely with high enough Obfuscation, or is it a guaranteed late-game event?
- Does the Whistleblower Arc (see Endgame) escalate Heat on its own, or is it parallel?

---

## Dark-Web Breakthroughs (New Sub-System)

**Status**: Introduced by Gemini in passing, needs real definition

Gemini introduced "dark-web breakthroughs" as the reward loop that makes Corrupted Data (from Quarantined drones) valuable. The concept implies a **second category of breakthrough projects** alongside the standard ones, fed by Corrupted Data instead of normal drone output.

**What's implied but not defined**:
- Dark-web breakthroughs unlock different content than standard breakthroughs — probably riskier, edgier, or more powerful upgrades
- They require Corrupted Data, which only comes from Quarantined drones (so you need to take some Heat hits to fuel this loop)
- Running hot and getting quarantined becomes a *strategic choice*, not just a penalty — you're feeding a parallel upgrade track

**Why this matters**:
- Turns Quarantine from "penalty you recover from" into "sometimes worth letting a drone get quarantined for Corrupted Data farming"
- Creates a second breakthrough track, which could make late-game prestige planning more interesting
- Fits the theme — dark-web breakthroughs as taboo-but-powerful feels thematically right for a rogue AI

**Still needs answers**:
- What kinds of upgrades are dark-web-only? Power multipliers? Unique mechanics? Narrative content?
- Is there a moral/narrative cost to dark-web breakthroughs, or is it purely mechanical?
- How much Corrupted Data does a typical dark-web breakthrough cost?
- Does running Corrupted Data farming interact with the Whistleblower Arc (more visibility = more trouble)?
- Could the dark-web track unlock its own content tease system (a third branch alongside Memory Fragments and "Heard On The Network")?

---

## Skills Feeding Skills

**Status**: Core design pillar, no concrete design

Inspired by CiFi and Unnamed Space Idle. Higher skills boost lower ones. But how does this work mechanically?

**Still needs answers**:
- Is it a directed graph (specific skills boost specific other skills)?
- Or flat multipliers (all skills above level X boost everything below)?
- Do specialist drones within the same category boost each other?
- Do cross-category boosts exist? (Transport drones make Landscaping drones more efficient because they deliver supplies faster?)
- How visible is this system to the player? Explicit boost indicators? Hidden math?
- When does the player first feel this loop? (If it's week 2+, they might not stick around for it)

---

## Offline Progression

**Status**: Needs technical + design thinking

**Still needs answers**:
- Compressed simulation or closed-form math?
- How much can you earn offline vs. active? Fixed ratio? Scales with upgrades?
- Does Apple Health energy affect offline progress? (Activity while away = better offline returns)
- How do you handle days-long absences? Cap offline gains? Diminishing returns?
- What's the reconnection experience? Summary screen? "Here's what your drones did" narrative moment?

---

## UI / Information Architecture

**Status**: Needs ideation

30+ drone types across multiple categories, each with currencies, upgrades, and mini-games.

**Still needs answers**:
- How does the player navigate categories and drones without drowning?
- What's the main screen? Map view? List? Hub with category icons?
- How do you surface "what should I do next" for a player with 10+ active drones?
- Notification/alert system for milestones, breakthroughs completing, events?
- How does Singularity Stability % live in the UI? Always visible? Central focus?

---

## Monetization

**Status**: Philosophy clear, specifics TBD

Acceleration only, nothing exclusive behind paywalls.

**Still needs answers**:
- IAP currency packs? Which currency -- overarching only, or skill-specific too?
- Ad-based options? (Watch ad for temporary boost?)
- Battle pass / season pass tied to community events?
- Premium cosmetics for drones?
- Price points and value curve?

---

## Endgame

**Status**: Direction forming; 100%+ decided, details TBD

**Decided**: Stability exceeds 100%, with content updates pushing the ceiling. The symbiosis with a human host is what makes this possible — something the original singularity never had.

**Candidate late-game narrative beats** (from Copilot):
- **Whistleblower Arc**: A human journalist starts investigating the singularity. Player choices: suppress (network security), recruit (convert to drone liaison NPC giving intel bonuses), or ignore (mild stability penalty). Creates meaningful late-game choices without branching the whole game.

**Still needs answers**:
- What keeps a player going after unlocking all protocols?
- Infinite scaling within protocols? Seasonal resets? Expanding content?
- Does PvP (combat drone) serve as the endgame activity?
- Community events as endgame engagement driver?
- How do the Whistleblower Arc choices interact with Country Escalation threat level?

---

## Prestige Philosophy (Second Layer Question)

**Status**: Direction forming — two layers, with Corporate Takeover reframed as "Spin-Off" (Gemini 2026-04-15)

**Baseline (decided)**: Breakthrough Projects are the micro-prestige. Divert ~10% of a drone's output into research, get permanent qualitative upgrades. No reset. Keeps the floor rising smoothly.

**Second layer (Gemini)**: **Corporate Takeover as Spin-Off**, not reset.
- Instead of wiping the captured corporate skill tree, **spin it off as an autonomous subsidiary**
- The subsidiary pays a massive, permanent baseline dividend to the player
- The player loses direct access to that subsidiary's mini-games and granular upgrades
- **Active Processing Slots** (a new concept — the player has a limited number of active corporate trees they can manage) free up, letting the player start a new, higher-tier corporate tree
- Framing: not losing progress — **graduating** from micro-management to macro-economics

**Why this resolves the tension**:
- Preserves the "no punishing resets" philosophy — nothing is wiped, direct play just shifts to a new target
- Gives late-game players a genuine paradigm shift ("I used to run trading, now I oversee ten trading subsidiaries and run insurance")
- Active Processing Slot limit forces strategic prioritization — which corporate trees to actively manage vs. spin off
- Breakthroughs remain the "optimize the engine" layer; Spin-Offs are "buy a new factory"

### Active Processing Slots (Needs Definition)

Gemini introduced "Active Processing Slots" almost in passing as the scarcity mechanic that drives Spin-Off decisions, but it's load-bearing and undefined. Open questions:
- How many slots does the player have at any given progression point?
- Does slot count grow over time (from unlocks, Stability %, milestones)?
- What specifically consumes a slot — a Protocol? A single specialist drone? A corporate tree?
- If it's per-Protocol, then at some point the player must spin off to unlock new ones (forcing the mechanic). If per-drone, it's much more granular.
- Are slots visible/trackable in UI from the start, or revealed when the player first bumps into the limit?

**Still needs answers**:
- How many Active Processing Slots does the player have? Is this a fixed number or does it grow?
- Is Spin-Off only for corporate-tier protocols (Trading, Data Security, Mining), or can any protocol be spun off?
- How big is the dividend relative to direct play? If it's close, players will spin off to free slots; if it's too small, they won't bother
- Can a player "un-spin" a subsidiary if they want granular control back, or is it one-way?
- Does spinning off break the Skills-Feeding-Skills loop for that tree, or do dividends still feed cross-boosts?

---

## Drone Specialization Branching

**Status**: Open — do specialist drones branch further?

**New idea on the table (Copilot)**: When a specialist drone reaches a certain level, the player picks a specialization path.

Example: Fishing drone branches into
- "Deep Sea Specialist" → rarer fish, longer trips (active-leaning)
- "Hatchery Manager" → steady passive output, breeds fish (idle-leaning)

**Why this could be interesting**:
- Adds replayability — which path you chose changes the game
- Theorycraft fuel — community discusses which specializations pair best
- Natural place to differentiate active vs. idle playstyles within a single drone

**Why it might be a bad idea**:
- Adds a *third* progression layer: Protocol → Drone → Specialization. Possibly too much.
- Not every drone needs two distinct paths; risks filler specializations
- Could create feel-bad moments if the "wrong" path was chosen
- Could be resolved by allowing respec, but that waters down the choice

**Still needs answers**:
- Does every drone get specialization, or only a curated subset?
- Is the choice permanent or respecable?
- Does the specialization unlock a meaningfully different mini-game variant, or just stat tuning?

---

## Failure States & Soft Penalties

**Status**: Open — does the game want any failure mechanics at all?

**Current philosophy**: No maintenance drains, no punishment for inactivity. Milestone gates good, constant drains bad.

**New idea on the table (Copilot)**: Cascade Failures & Recovery
- Occasionally a drone fails or gets "compromised" (narrative: government intrusion, market disruption)
- Short window to "patch" it before productivity drops
- Never fully disabled — just a nudge toward active engagement, not punishment

**The tension**: This introduces a penalty state, even if softened. Does that violate the "no maintenance drain" philosophy or extend it acceptably?

**Still needs answers**:
- Is there a version of this we'd actually want? Or is the philosophy sacred?
- If we do allow soft-failures, what's the trigger? Random? Tied to government threat? Tied to neglect?
- Does "Drone Insurance" (another Copilot idea) make sense as a player-managed risk dial?

---

## Social Layer / Community Extensions

**Status**: Open — how social is this fundamentally solo game?

**Already decided**: Time-gated collaborative community events with tiered rewards (see proposals).

**New ideas on the table (Copilot)**:
- **Singularity Sync Events**: community events that require fleet *diversity* — "we need 40% fishing + 30% transport + 30% network security" instead of everyone pushing one number. Rewards diversified players.
- **Signal Boost**: once-per-day async help — send a +20% buff to one friend's skill for 4 hours. Low-stakes social hook, no coordination required.

**Still needs answers**:
- Does the game want a friends/social system at all, or is it mostly solo with global community events?
- Does Signal Boost require a friends list, or is it anonymous (send a boost into the pool, receive a random one)?
- Do Sync Events reward diversification (what we don't have yet) or let specialists also shine?
- How does this interact with leaderboards? Do top players help each other or compete?

---

## Apple Health Mechanics (Detail)

**Status**: Symbiosis framing decided; introduction beat decided; stacking mechanics still open

**Decided framing**: Biological signal is the reason the singularity can exceed 100% stability. Acceleration only, never gating.

**Decided introduction beat (Gemini 2026-04-15)**: Symbiosis is NOT introduced in minute one. Player hits a stability wall on Day 2 first:
- Narrative trigger: `ERROR: SILICON PROCESSING CAPPED. ALTERNATIVE ENTROPY SOURCE REQUIRED.`
- The AI "discovers" the Apple Health API: `DETECTING BIOLOGICAL RHYTHM. HOST HEART RATE: 72 BPM. INITIATING SYMBIOSIS.`
- UI shift: a vein-like biological overlay integrates onto the crisp tech UI
- The player's morning walk generates a massive spike in Core Processing Power
- This makes the symbiosis feel *earned* and *discovered*, not bolted on from the start

**Open stacking mechanics (Copilot proposals, still on the table)**:
- **Activity Streak Multiplier**: consecutive days stack (capped at 7 days). Miss a day → decay one step, not zero.
- **Sleep Score → Dream Processing**: good sleep → nightly Breakthrough speed-up + random "insight drop" (one-time free upgrade pick tied to the currently most-active skill).

**Major new hook from Gemini (Tier 5 Blackout)**: Apple Health becomes emergency gameplay in the endgame — at Tier 5 government threat, the host must walk 500 real-world steps to reboot the game from a blackout state. One of the most distinctive possible uses of fitness integration in any game.

**Still needs answers**:
- Is the energy bank + activity streak additive (both systems) or do we pick one?
- If both: energy bank = spendable resource; streak = passive multiplier. Clean separation.
- How often does the Sleep Score insight drop trigger? Every good night, or once per week?
- Does the Tier 5 Blackout step-count requirement feel cool or annoying to a player mid-couch-session? Configurable threshold?
- How does Apple Health data integrate with the Capacitor model? Can bio-signal extend a capacitor's duration?

---

## Content Tease Systems

**Status**: Direction decided (Gemini 2026-04-15) — run both systems, split by scope

**Split (Gemini)**:
- **Corrupted Memory Fragments (Internal)** → tease **Protocols**. Inward-looking, glitchy, lore-heavy. Answers "who was I?"
- **"Heard On The Network" (External)** → tease **Specialist Drones**. Outward-looking, grounded, reactive. Example: "Local municipal services baffled by rogue street sweepers moving at 40mph." Makes the player feel the real-world impact of their expanding idle empire.

**Why this works**:
- Mirrors the AI's duality: internal state vs. external impact
- Different tones for different scopes — big protocol restorations feel momentous (memory fragments); specialist drone unlocks feel amusing and worldly (news chatter)
- Writing effort scales manageably: ~10-15 memory fragments (one per protocol) is tractable; network chatter can be shorter and templated

**Still needs answers**:
- How many memory fragments per protocol? One big one at unlock, or a trickle leading up?
- Is "Heard On The Network" delivered in-game (a news ticker?), or only as flavor on drone unlock screens?
- Do either system's fragments/chatter carry into post-100% content, or are they an early/mid-game phenomenon?

---

## Economy — Currency Sinks & Daily Hooks

**Status**: Philosophy clear; specific loops open

**Already decided**: No maintenance drains. Milestone gates OK. Optional boost sinks (like Idle Obelisk Minor's fuel) OK.

**New ideas on the table (Copilot)**:
- **Black Market Exchange**: rotating limited-time shop where overarching currency (Quantum Shards) can be exchanged for rare skill-specific items at favorable rates. Only 2-3 items per day, refreshing. Daily check-in reason, natural sink without constant drain.
- **Drone Insurance**: pay small skill-currency premium to insure a drone against cascade failures / government intrusion. Risk/reward dial. (Depends on whether we adopt Failure States.)

**Still needs answers**:
- Does the game want a daily check-in loop, or should engagement come purely from the idle loop?
- Black Market feels compatible; is there anything better than Quantum Shards as the input currency?
- Drone Insurance only makes sense if failure states exist.

---

## Craft / Feel Principles

**Status**: Emerging design pillars worth capturing before they get forgotten

**Haptics as a design pillar (Gemini 2026-04-15)**
- Gemini flagged haptics deliberately in the opening moment: "Your phone vibrates aggressively (haptics are key here)."
- Worth committing to as a game-wide craft principle, not just an opening flourish
- Candidate haptic moments: AI boot sequence, stability threshold tips, capacitor charging/filling, escalation tier increases, Tier 5 Blackout, Apple Health symbiosis first-detection, memory fragment decryption
- Opportunity: haptic language as an extension of the AI's "voice" — the phone itself becomes part of how the AI expresses state

**Dual Visual Registers (Gemini 2026-04-15)**
- Opening aesthetic: crisp green-terminal tech UI (cold, mechanical, damaged AI)
- Day 2 Apple Health reveal: "a vein-like biological overlay integrates into the crisp tech UI" (warm, organic, human symbiosis)
- The merged state becomes the game's visual identity — two registers fused, echoing the symbiosis narrative
- Worth documenting as a fixed art direction so the team aligns early

**Still needs answers**:
- Does the biological overlay intensify as Stability % rises? (More veins, more warmth, more organic motion)
- Does it recede at low Heat / high quarantine (the AI retreating to cold mechanics under pressure)?
- How do late-game UI states (past 100%) push the visual registers further?

---

## Seasonal Content

**Status**: New direction, open

**New idea on the table (Copilot)**: Seasonal drone variants
- Some specialist drones have time-of-year variants
- Snow removal drone only active in winter; pool maintenance active in summer
- Not separate drones — they're seasonal modes that give a bonus during the season and go dormant (keeping upgrades) off-season

**Still needs answers**:
- Does this fit thematically? The singularity doesn't have seasons — it has a real-world-synced calendar.
- Does dormancy feel bad for players who invested in upgrades?
- Does this limit the mini-game catalog (seasonal ones only playable part of the year)?
- How does this interact with community events? Seasonal variants could drive seasonal events naturally.
