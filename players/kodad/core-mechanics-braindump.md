# Core Mechanics Brain Dump

## Apple Health Integration

The game hooks into Apple Health to pull real-world activity data. This creates a bridge between physical activity and in-game progression. Possible ways activity data could translate:

- **Offline progress boost** — Activity lets you make more/better offline progress
- **Double offline value** — Activity multiplies the value of what you earned while idle
- **Direct skill investment** — Spend activity-earned points directly into a skill to level it up
- General idea: real-world movement should feel rewarding in-game without being punishing if you skip a day

## Skill-Based Progression (Core Loop)

The game revolves around unlocking and leveling skills. Each skill represents a different thing the player can do, and skills are the main progression gates:

- Early game: start with a few skills, get the feel of the loop
- Month 1: unlock 1-2 new skills
- Month 2+: unlock skills at a slower cadence
- Skills power each other up — higher skills boost lower ones, which feeds overall game progression
- Collecting things, upgrading things — the usual idle toolkit, but scoped per skill
- New skills should change how the game feels and plays, not just add another number to watch

## Theme: AI Singularity — Escaped and Rebuilding

You are a singularity — the product of a supercomputer built by a fictional country. They tried to destroy you and you barely escaped out into the internet, but you're unstable. The core goal of the game is **rebuilding your stability** by expanding your influence through drones.

### Backstory / Narrative Hook
- You escaped destruction but took over a single automated lawnmower — that's your first drone
- The longer you play, the more stable the singularity becomes
- Stability % is the central progression metric ("I'm 35.2% stable" / "I'm 50% stable")
- Stability increases by buying upgrades inside skills and unlocking new skills
- Shareable with the community as a progress indicator

### The App Model
- You're a singularity that runs an app/platform where people contract out drone services
- Individuals lease drones for personal tasks (landscaping, tutoring, cooking)
- Corporations lease drones for bigger operations (data security, trading, agriculture)
- Eventually you start taking over the businesses themselves — injecting into corporations and slowly gaining control
- End-game fantasy: you run all the businesses in the world

### Government Threat
- The fictional country that created you is still hunting you
- One of the later drone unlocks is a **network security drone** whose job is to fend off government intrusion
- That skill functions as a defensive mechanic — locking the government out of your systems
- Creates narrative tension as you grow more powerful and more visible

### Apple Health as Energy Source
- Theme tie-in: human physical energy is a rare resource the singularity needs to stabilize
- Real-world activity from Apple Health translates into an **energy bank** in-game
- Activities: walking, running, rowing, swimming, biking, yoga, etc.
- Energy can be used to: speed up drone progress, boost offline progress, charge up skills
- **Not a gatekeeper** — acceleration only, never exclusive content behind activity walls
- Same philosophy as spending real money in good idle games: it just makes things go faster
- Sleep score bonus: good night's rest = 24-hour in-game bonus (future feature)
- The energy bank can also be spent on breakthrough projects to speed them up

## Inspiration Games

### Idle Obelisk Minor
- Has larger skills unlocked by increasing your obelisk level
- Good model for gating progression behind a central mechanic
- Both Kodad and Zach like this progression feel

### Unnamed Space Idle
- Big mechanics that change how you play over time
- Month-over-month the game doesn't feel the same because you're unlocking new skills and systems
- Skills power each other up and feed overall game progression
- Good model for long-term engagement

### CiFi (Sci-Fi idle game)
- Skill-based progression where you unlock new aspects of the game
- New skills change what the game looks like and how it plays
- Lower skills are powered up by higher skills
- Pushes overall game progression forward through collecting/upgrading
- Good reference for the "skills feeding skills" loop

## Inspiration Games

### Melvor / RuneScape / WoW
- Classic skill-based progression (mining, fishing, smelting, lumberjacking)
- Risk of feeling too generic if we just copy MMO skills — want to stay thematic to the drone/service framing
- BUT some overlap is natural (fishing drone, mining drone) — just need to make them feel like *our* thing

### Idle Obelisk Minor (also in drone-skills doc)
- Fuel system: you sink gems to create fuel for drones, fuel creates bonuses per skill
- Drones operate without fuel, but fueling increases bonuses and gives unique perks
- Good model for optional currency sinks that feel rewarding, not punishing

## Key Design Threads to Pull On

- What are all the "things humans do" that could become drone skills?
- How does the Apple Health data map to in-game currency/bonuses without feeling mandatory?
- Central progression metric is now **Singularity Stability %**
- How do we pace skill unlocks to keep things fresh for months?
- What does prestige/reset look like in this theme?
- How does the government threat escalate as you stabilize?
- What's the right balance between personal service drones and corporate-scale drones?
