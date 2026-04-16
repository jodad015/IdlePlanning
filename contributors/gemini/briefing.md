# Gemini Session Briefing

**Paste this entire doc into a fresh Gemini chat before you start brainstorming.**

Refresh this doc before each new session so the context reflects where the project currently is. Old agenda items can be removed once covered; keep the "Context" and "Decided Direction" sections always current.

---

## Instructions to Gemini

You're collaborating on an idle game design. I'll give you the context below and some topics I want to explore with you.

Your role:
- Riff divergently — propose multiple options rather than one safe answer
- Poke holes in weak ideas
- Help me think through second-order consequences
- Stay in the theme (AI singularity, drones, recovery narrative)
- Be specific; avoid generic design advice

Don't worry about consensus or synthesis — that happens later when I take the transcript back to the team. Give me your most interesting ideas.

---

## Context: What the Game Is

You play a damaged AI singularity. A fictional country built you in a supercomputer and then tried to destroy you. You barely escaped into a single device — a phone — and you're unstable. The only surviving protocol from your past life is the **Landscaping Protocol**, which currently has one functional drone: a lawnmower.

The game is about **recovery**: restoring protocols, deploying specialist drones within each protocol, and rebuilding yourself. Your progress is measured in **Singularity Stability %** ("I'm 37% stable"). At 100% you've fully recovered what you were. Beyond 100%, you're evolving into something your creators never designed — because you now have something the original didn't: a human host.

**The host is the player.** The singularity lives in the player's phone. The one thing it can't generate is biological signal data — steps, heart rate, movement — so the player's real-world activity (via Apple Health) is the **literal fuel for recovery**. This isn't a bolted-on fitness feature; it's the core symbiosis that makes progression past 100% possible.

**The shape of progression:**
- **Protocols** are top-level categories of work the singularity can perform (Landscaping, Transport, Cleaning, Fishing, Mining, Trading, etc.)
- Each protocol is **restored** at a major milestone — often accompanied by a corrupted memory fragment hinting at what the singularity used to be
- Inside each protocol, you deploy **specialist drones** with their own mini-games, currencies, and upgrade trees
- Example: Landscaping Protocol → Mower drone, Trimming drone, Planting drone

**Active vs. idle:**
- Each specialist drone has a **one-thumb portrait mini-game** for active play
- Idle progression continues always; active play and bio-signal acceleration boost it
- Apple Health never gates content — it just makes things faster

**Narrative arc:**
- Early: confused and fragile, discovering what you were
- Mid: confident and expanding, corporate and service drones scaling up
- Late: powerful and hunted — the government is escalating attacks as you become visible
- Endgame: evolving past your original self because of the symbiosis

---

## Decided Direction (What's Locked In)

- **Protocol model**: broad protocols containing specialist sub-drones (hybrid, chosen over pure specialist or pure broad)
- **Singularity Stability %** as central progression metric, able to exceed 100%
- **Breakthrough projects** instead of full prestige resets: divert ~10% of a drone's output into background research for permanent qualitative upgrades
- **Two-tier currency**: skill-specific currencies (fish, gems, logistics credits, etc.) + overarching currency (working name "Quantum Shards" or "Core Processing Power")
- **No maintenance drains**: milestone gates are OK, constant drains are not
- **Monetization philosophy**: acceleration only, nothing gated behind paywalls
- **Apple Health symbiosis**: biological signal is the thematic reason the player matters to the AI — the thing that makes 100%+ stability possible
- **Corrupted memory fragments** tease upcoming protocol restorations
- **Community events**: time-gated collaborative goals with tiered rewards that scale by player progression
- **PvP combat drone** is a late-game feature, not a launch feature

---

## Ideas On The Table (Not Decided — Under Discussion)

Copilot recently brainstormed a batch of proposals. A few of these are referenced directly in the agenda below. Flagged here so you have the full context:

- **Country Escalation Ladder** — government threat as a visible "wanted level" tier system. Higher threat = more attacks BUT more visibility = more corporate clients = more income. A deliberate risk/reward dial.
- **Network Security = Tower Defense** — the active mini-game for the network security drone is tower-defense-lite. Place firewall nodes before attack waves. Idle players have baseline auto-defense; active players optimize.
- **Corporate Takeover as Prestige** — taking over corporations is an alternative prestige layer alongside Breakthrough Projects. Resets corporate skill tree, returns permanent stability multiplier. Story-driven, not grind.
- **Drone Specialization Branching** — at a level threshold, drones split into paths (e.g., Fishing → "Deep Sea Specialist" vs. "Hatchery Manager"). Open whether this becomes a third progression layer or gets cut.
- **Activity Streak Multiplier** — Apple Health activity stacks a multiplier over consecutive days (capped 7). Miss a day, decays one step.
- **Whistleblower Arc** — late-game narrative chain where a journalist investigates you. Choices: suppress, recruit as drone liaison, or ignore.
- **Mini-games proposed**: Warehouse Tetris (logistics), Rhythm-based (day trading), Tower Defense (network security).
- **Heard On The Network** — external tease system complementing memory fragments. NPC news snippets and corporate memos hint at upcoming drone unlocks.

---

## Agenda: 12 Questions

Five topics, twelve questions total. Some are quick reactions, some are deep back-and-forth — tags on each. Don't feel like you need to cover them all; if one unlocks a rich thread, follow it. The rest are backup depth.

**Depth tags**: `[deep]` = expect several minutes of back-and-forth · `[medium]` = a few rounds · `[quick]` = react and move on.

### Topic A: Early Game Flow

**Q1 `[deep]`** — Storyboard the first 10 minutes. What does the player see, do, read? Opening cutscene? Jump straight in? How does the "what else was I?" mystery get planted?

**Q2 `[medium]`** — When does the second specialist drone unlock within Landscaping, and when does the second Protocol unlock? Should these be time-gated, milestone-gated, or a hybrid? What's the ideal pacing — hours or days to see the game "open up"?

**Q3 `[medium]`** — What's the first meaningful Apple Health moment? When does the symbiosis get acknowledged narratively — minute one, day one, week one? Does the AI "notice" the host, and how is that revealed?

### Topic B: Government Threat & Country Escalation Ladder

**Q4 `[deep]`** — Is the Country Escalation Ladder (threat as a "wanted level" risk/reward dial — higher threat = more attacks but more corporate clients) the right frame? What are viable alternatives if we don't love this?

**Q5 `[medium]`** — What triggers threat level changes? Stability %, income, specific actions, player choices, or a mix? Does the player have direct control ("provoke events"), or is it emergent?

**Q6 `[medium]`** — What happens when the government actually "breaks through"? Temporary debuff, lose a memory fragment, narrative event, corrupted drone? How do we create stakes without making the moment feel punishing?

**Q7 `[quick]`** — Give me 3 distinct escalation event types at different tiers. Examples: tier 1 might be "probe attempts"; tier 5 might be something much bigger. What are the beats in between?

### Topic C: Prestige Philosophy

**Q8 `[deep]`** — Do we want one prestige layer (Breakthrough Projects only) or two (Breakthrough + Corporate Takeover)? What does each give us mechanically and narratively? What's the strongest argument for each direction?

**Q9 `[medium]`** — If we add Corporate Takeover as a prestige layer, does "reset a corporate skill tree" feel rewarding or punishing? Is there a way to get the *feel* of corporate takeover progression without an actual reset?

### Topic D: Mini-Game Architecture

**Q10 `[medium]`** — Can we group 30+ drones into 5-6 mini-game "families" (timing, path-tracing, placement, rhythm, tower-defense, reaction)? Which families cover the most ground? What would we lose by consolidating vs. gain in development tractability?

**Q11 `[medium]`** — Should mini-game performance affect idle output? Options: performance multiplies idle earnings, performance unlocks bonus currency, performance is purely cosmetic/for fun, or performance unlocks new mini-game tiers. Argue both sides — what's lost if mini-games don't affect idle, and what's lost if they do?

### Topic E: Content Systems

**Q12 `[quick]`** — Two tease systems are on the table: **Corrupted Memory Fragments** (internal — glitchy visuals hinting at forgotten protocols) and **"Heard On The Network"** (external — NPC news snippets, corporate memos hinting at new drones). Do we run both, pick one, or split them (fragments for protocols, news for specialist drones)?

---

## After the Session

When you're done talking to Gemini, grab the full transcript. I'll:
1. Create a new file in `contributors/gemini/` with a descriptive name (e.g., `2026-04-15-early-game-flow-and-escalation.md`)
2. Save the raw transcript there for reference
3. Extract the ideas, alternatives, and pokes-at-weak-points into a clean summary doc
4. Update `players/kodad/open-questions-and-thoughts.md` with anything new
5. Flag the most promising threads for follow-up

You don't need to pre-process the transcript — just paste it as-is.
