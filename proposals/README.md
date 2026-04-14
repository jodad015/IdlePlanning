# Proposals

Proposals are how Kodad and Zach pitch ideas to each other asynchronously. Think of them as lightweight RFCs — structured enough to be actionable, casual enough to not slow you down.

## Lifecycle

1. **Open** — Someone writes a proposal. The other person hasn't weighed in yet.
2. **Discussing** — Both people (or Claude) have added responses. Still working it out.
3. **Accepted** — Both agree. The proposal graduates into a decision record in `decisions/`.
4. **Revised** — The core idea changed significantly based on discussion. The proposal is updated and status resets to Discussing.
5. **Rejected** — Decided against. Keep the file so you remember why.
6. **Parked** — Good idea, wrong time. Revisit later.

## File Format

`NNN-short-description.md` (e.g., `001-core-theme-direction.md`)

Use the template below or see `_template.md`.

## Template

```markdown
# [Number] - [Title]

**Proposed by**: [Name]
**Date**: YYYY-MM-DD
**Status**: Open

## Proposal

What are you proposing? Be as detailed or as rough as you want — this is a starting point, not a final spec.

## Why

What's the motivation? What problem does this solve or what opportunity does it open?

## Open Questions

- Things you're unsure about or want the other person's take on.

## Discussion

### [Name] - [Date]
Response here. Keep it conversational.
```

## When a Proposal Gets Accepted

Create a corresponding decision record in `decisions/` that captures the final agreed-upon direction and rationale. Link back to the proposal for context.
