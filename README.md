# IdlePlanning

Collaborative planning repo for an idle game. Two planners (Kodad and Zach) use this space for divergent thinking, then converge with the help of Claude Code agents.

## How This Repo Works

### The Workflow

1. **Diverge** -- Write freely in your personal space (`players/kodad/` or `players/zach/`). Don't worry about format, overlap, or polish. Brain dump mechanics, reference games, sketches, half-baked ideas.
2. **Synthesize** -- When you're ready to converge, ask Claude Code to read both scratch spaces and pull out overlaps, tensions, and surprises. Synthesized output goes into `design/`.
3. **Decide** -- When a synthesis leads to a concrete decision, record it in `decisions/` so you don't relitigate it later.

### Directory Structure

```
players/
  kodad/       # Kodad's scratch space -- raw ideas, notes, references
  zach/        # Zach's scratch space -- raw ideas, notes, references
design/        # Synthesized design docs (core loop, progression, theme, etc.)
technical/     # Architecture, stack, platform, and implementation planning
decisions/     # Numbered decision records with rationale
```

### Working With Claude Code

**Starting a planning session:**
Just open the repo and start talking. Claude Code has instructions (in CLAUDE.md) for how to operate in this planning context.

**Useful things to ask Claude Code:**
- "Read through both player scratch spaces and find common themes"
- "What tensions exist between Kodad's and Zach's ideas?"
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
