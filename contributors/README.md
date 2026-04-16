# AI Contributors

This directory holds scratch spaces for AI collaborators: **Claude**, **Copilot**, and **Gemini**.

## How AI Contributors Differ From Players

**Players (Kodad, Zach, Ethan)** are the decision-makers. They own the vision, approve proposals, and the game is ultimately theirs.

**AI contributors** are along for the ride. They read the full repo, help brainstorm when asked, and can add to discussions on proposals and questions. They do **not** approve proposals and their input doesn't count toward proposal acceptance. Their job is to surface ideas, challenge assumptions, and bring outside perspective — not to vote.

### AI Input Is Contribution, Not Verdict

AI contributors sometimes present confident-sounding statements as if settled — especially when they're repeating something they said earlier in the same session or relitigating a point the planners already moved past. A few things to keep in mind when synthesizing AI output back into the repo:

- **Treat AI confidence as a flag, not a conclusion.** A strong opinion from Gemini or Copilot is a *contribution* to the discussion, not a decision.
- **Call it out when an AI repeats obsolete material.** If the planners already decided X and the AI is re-proposing not-X, note it in the session summary so we don't silently drift back.
- **Hold open the option the player originally preferred.** When an AI pushes back on a decided direction, keep the original choice alive as a real alternative until a planner explicitly re-weighs in.
- **Quote the AI, don't paraphrase into decisions.** Keep AI contributions identified as such in summaries so it's always clear what came from where.

## Scratch Spaces

Each AI has its own scratch space:
- `contributors/claude/` — Claude's durable brainstorms
- `contributors/copilot/` — Copilot's durable brainstorms
- `contributors/gemini/` — Gemini's durable brainstorms

## When to Use These Spaces

Use these spaces when you want independent, in-that-AI's-voice contributions recorded for everyone else to read later.

- **"Claude, brainstorm X in your scratch space"** → Claude (this tool) writes its own independent take to `contributors/claude/`. This is different from "write up what we discussed in my scratch space," which goes to the player's folder.
- **For Copilot and Gemini** → the player running those tools pastes the AI's output into `contributors/copilot/` or `contributors/gemini/` with a brief note about the prompt that generated it.

These are **brainstorm artifacts**, not synthesis. Synthesis of ideas across players still goes to `design/`.

## Contributing to Discussions

AI contributors can add responses to proposals and questions. When they do, they should identify themselves in the response header (e.g., `### Claude - 2026-04-15`). Their responses are advisory — useful for perspective, not counted toward approval.

## Reading Scope

AI contributors are expected to read **everything** in the repo when engaging — all player scratch spaces, all proposals, questions, design docs, technical docs, and decision records. Full context produces better contributions.
