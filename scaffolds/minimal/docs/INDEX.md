# Documentation Index

> Purpose: Map the docs, explain what each document is for, and show where the main answers live.
> When to update: When files are added, removed, renamed, or reassigned.
> Owner: {{OWNER_NAME}}.

## Main Rules

- `docs/INDEX.md` is the file map for the docs.
- `README.md` is the main file for humans.
- `CLAUDE.md` is the main file for Claude Code.
- `docs/PRD.md` owns product scope and requirements.
- `docs/ARCHITECTURE.md` owns system structure.
- `docs/TESTING.md` owns testing rules.

## Reading Order

- Humans: `README.md` -> `docs/INDEX.md` -> `docs/DEVELOPMENT.md` -> `docs/PRD.md` -> task-specific docs
- LLMs: `CLAUDE.md` -> `docs/INDEX.md` -> task-specific docs

## Root Files

- `README.md`: start here if you are a person
- `CLAUDE.md`: start here if you are Claude Code

## Core Docs

- `docs/DEVELOPMENT.md`: local setup, commands, and working rules
- `docs/PRD.md`: goals, scope, and requirements
- `docs/ARCHITECTURE.md`: system shape and key boundaries
- `docs/TESTING.md`: testing layers and required checks

## Where To Look

- What is this project and why does it exist? `README.md`, `docs/PRD.md`
- How do I run it locally? `docs/DEVELOPMENT.md`
- How is it structured? `docs/ARCHITECTURE.md`
- How do we test it? `docs/TESTING.md`
- What should I read next? `docs/INDEX.md`, `CLAUDE.md`

## Feature Workflow

- `docs/specs/FEATURE_SPEC_TEMPLATE.md`: feature problem and outcome
- `docs/specs/IMPLEMENTATION_PLAN_TEMPLATE.md`: technical plan for an approved spec
- `docs/specs/TASK_BREAKDOWN_TEMPLATE.md`: small reviewable tasks
