# Harness Guide

> Purpose: Explain how this document system is supposed to work and how to keep it useful over time.
> When to update: When canonical-source rules, template usage, or anti-drift practices change.
> Owner: {{OWNER_NAME}}.

## Design Principles

- Keep one clear owner per question.
- Prefer short, durable docs over long narrative dumps.
- Update the doc that owns the truth instead of duplicating it elsewhere.

## Canonical Sources

- `README.md`: human entry point
- `CLAUDE.md`: canonical agent instruction file
- `docs/INDEX.md`: doc map and ownership guide
- `docs/PRD.md`: product intent and scope
- `docs/ARCHITECTURE.md`: durable system structure

## Anti-Drift Rules

- Update docs in the same change as the code when possible.
- Delete stale guidance instead of layering contradictory notes on top.
- Record important tradeoffs in durable docs, not only in ephemeral chat.
