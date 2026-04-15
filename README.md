# IdlePlanning

Collaborative planning repo for an idle game. Three planners (Kodad, Zach, and Ethan) use this space for divergent thinking, then converge with the help of Claude Code agents. Three AI contributors (Claude, Copilot, Gemini) also participate — reading the repo, brainstorming when asked, and adding advisory input on proposals. Only the three planners approve decisions.

## How This Repo Works

### The Workflow

1. **Diverge** -- Write freely in your personal space (`players/kodad/`, `players/zach/`, or `players/ethan/`). Don't worry about format, overlap, or polish. Brain dump mechanics, reference games, sketches, half-baked ideas.
2. **Propose** -- When you have an idea you want the others' take on, write a proposal in `proposals/`. For smaller things, drop a question in `questions/`.
3. **Discuss** -- Respond to each other's proposals and questions async. Claude can help challenge, refine, and poke holes. Proposals typically need input from all three planners before they graduate to a decision.
4. **Synthesize** -- When you're ready to converge, ask Claude Code to read all three scratch spaces and pull out overlaps, tensions, and surprises. Synthesized output goes into `design/`.
5. **Decide** -- When a proposal is accepted or a synthesis leads to a concrete decision, record it in `decisions/` so you don't relitigate it later.

### Directory Structure

```
players/
  kodad/          # Kodad's scratch space -- raw ideas, notes, references
  zach/           # Zach's scratch space -- raw ideas, notes, references
  ethan/          # Ethan's scratch space -- raw ideas, notes, references
contributors/
  claude/         # Claude's brainstorm space (AI, non-voting)
  copilot/        # Copilot's brainstorm space (AI, non-voting)
  gemini/         # Gemini's brainstorm space (AI, non-voting)
proposals/        # Async proposals between planners (lightweight RFCs)
questions/        # Quick async questions for the other planners
design/           # Synthesized design docs (core loop, progression, theme, etc.)
technical/        # Architecture, stack, platform, and implementation planning
decisions/        # Numbered decision records with rationale
```

### Working With Claude Code

**Starting a planning session:**
Just open the repo and start talking. Claude Code has instructions (in CLAUDE.md) for how to operate in this planning context.

**Useful things to ask Claude Code:**
- "Read through all the player scratch spaces and find common themes"
- "What tensions exist between Kodad's, Zach's, and Ethan's ideas?"
- "Claude, brainstorm X in your scratch space" (writes to `contributors/claude/`)
- "Paste this Gemini output into Gemini's space with a note about the prompt"
- "Synthesize our thoughts on [topic] into a design doc"
- "What open questions should we resolve next?"
- "Poke holes in this mechanic: [description]"
- "Help me think through the second-order effects of [mechanic]"
- "Create a decision record for [choice we just made]"
- "Compare the tradeoffs of [framework A] vs [framework B] for this kind of game"
- "What technical constraints does [mechanic] create?"
- "Draft a technical plan for [system]"

**Adding your own ideas:**
You can write directly in your player folder, or ask Claude Code to capture your thoughts as you talk through them.

### Conventions

- **Scratch files**: Any format, any name. Your space, your rules.
- **Design docs**: Markdown. One topic per file. Keep them living documents.
- **Technical docs**: Markdown. One topic per file. Cover tradeoffs, not just choices.
- **Decision records**: Numbered (`001-topic.md`). Include context, options considered, decision, and rationale. Used for both design and technical decisions.
