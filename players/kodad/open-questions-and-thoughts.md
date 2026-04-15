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

**Status**: Needs ideation

The player starts as a damaged singularity that escaped into a lawnmower. What do the first minutes, hours, and days actually feel like?

**Minute 0-5 (The Hook)**:
- How much narrative before gameplay? Quick cutscene? Text crawl? Jump straight in?
- First action is presumably mowing -- does the mini-game tutorial happen here?
- How quickly does the player understand the core loop (do task → earn currency → upgrade → do task better)?

**First session (~30 min)**:
- How many systems are visible? Just Landscaping + its first sub-drone?
- When do upgrades start feeling meaningful?
- Is the overarching currency (Quantum Shards / Core Processing Power) visible yet or hidden?
- Does the player see Singularity Stability % from the start?

**Day 1**:
- When does the second specialist drone within Landscaping unlock?
- When does the player first leave the app and come back to meaningful offline progress?
- Is Apple Health integration surfaced on day 1 or held back?

**Week 1**:
- When does the second category unlock? (This is the big moment -- the game opens up)
- When does the player first feel "skills feeding skills"?
- How many active drones are they managing?
- Is the government threat hinted at yet?

**Key tension**: Show too much too fast = overwhelming. Drip too slowly = players quit before the loop clicks. Where's the sweet spot?

**Still needs answers**:
- What's the unlock trigger for the second category? Time played? Stability %? Specific milestone?
- Should early pacing feel fast (hook them) or deliberate (teach them)?
- How do we make the lawnmower phase feel fun and not like a tutorial prison?

---

## Mini-Games

**Status**: Needs ideation

Each specialist drone has an active mini-game (one-thumb, portrait mode). 5 rough concepts exist; 30+ drone types need them.

**Still needs answers**:
- Do some mini-games share core mechanics with different skins? (e.g., "timing tap" for both fishing and package delivery)
- How does mini-game performance affect idle output? Multiplier? Bonus currency? Nothing?
- What keeps a mini-game fun after the 50th play? Scaling difficulty? Random modifiers? Leaderboards?
- How complex should late-game mini-games be compared to early ones?
- Do mini-games evolve as you upgrade the drone? (New obstacles, new mechanics within the same game)

---

## Government Threat Mechanic

**Status**: Concept only, no gameplay design

The fictional country that created you is hunting you. Network security drone defends against intrusion. But how?

**Still needs answers**:
- Is this a passive threat (background timer/events) or active gameplay?
- Does the threat escalate with Singularity Stability %? (More stable = more visible = more attacks)
- What happens if the government "breaks through"? Temporary debuff? Lose progress? Narrative event?
- Is the security drone always running defense, or do you actively manage it during attack events?
- How does this interact with community events? Could government attacks be a shared threat?

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

**Status**: Acknowledged as important, no design yet

**Still needs answers**:
- Is there an asymptotic stability ceiling (100%) or does it go infinite?
- What keeps a player going after unlocking all categories?
- Infinite scaling within categories? Seasonal resets? Expanding content?
- Does PvP (combat drone) serve as the endgame activity?
- Community events as endgame engagement driver?
