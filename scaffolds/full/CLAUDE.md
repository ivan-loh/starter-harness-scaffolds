# CLAUDE

> Purpose: Be the canonical instruction file for Claude Code and agent-assisted work in this repository.
> When to update: When project workflow, required reads, validation rules, or documentation ownership changes.
> Owner: {{OWNER_NAME}}.

## Canonical Rule

- Treat this file as the canonical agent instruction file for the repo.
- Do not create or depend on `AGENTS.md` in this scaffold.
- Keep this file short, stable, and specific.
- Treat `docs/INDEX.md` as the canonical document map.
- Do not create a second file index in another document.

## Start Here

- Always read `README.md` and `docs/INDEX.md` before significant work.
- Use `docs/INDEX.md` to decide which document owns the question you are working on.

## Task Routing

- Scope, goals, non-goals, and requirements: `docs/PRD.md`
- Local commands, environment rules, and developer workflow: `docs/DEVELOPMENT.md`
- System shape, boundaries, and invariants: `docs/ARCHITECTURE.md`
- Current implementation shape and tradeoffs: `docs/DESIGN.md`
- Interfaces and contracts: `docs/API.md`
- Entities, lifecycle, and migration concerns: `docs/DATA_MODEL.md`
- Internal security controls: `docs/SECURITY.md`
- Public vulnerability reporting policy: `SECURITY.md`
- Validation strategy and required checks: `docs/TESTING.md`
- Runtime ownership and operations: `docs/OPERATIONS.md`
- Monitoring and diagnosis: `docs/OBSERVABILITY.md`
- Rollout, rollback, and release management: `docs/DEPLOYMENT.md`, `docs/RELEASE.md`, `docs/runbooks/*`
- Contribution and review workflow: `CONTRIBUTING.md`, `CODEOWNERS`, `.github/*`
- Document set rules and ownership: `docs/HARNESS_GUIDE.md`, `docs/INDEX.md`
- Feature delivery packets: `docs/specs/*`

## Required Reads By Change Type

- Read `docs/PRD.md` before changing product behavior or scope.
- Read `docs/ARCHITECTURE.md` before structural or integration changes.
- Read `docs/DESIGN.md` before changing the current technical solution shape.
- Read `docs/API.md` and `docs/DATA_MODEL.md` before changing interfaces or core entities.
- Read `docs/SECURITY.md` before changing auth, secrets, trust boundaries, or sensitive data flows.
- Read `docs/TESTING.md` before changing validation strategy or test coverage.
- Read `docs/DEVELOPMENT.md` before changing local commands, tooling, or environment expectations.
- Read `docs/OPERATIONS.md`, `docs/OBSERVABILITY.md`, and `docs/DEPLOYMENT.md` before changing runtime or release behavior.

## Working Rules

- Prefer `spec -> plan -> tasks` before large changes.
- Keep diffs focused and easy to review.
- Update the relevant docs in the same change when behavior or process changes.
- Update `docs/INDEX.md` if files are added, removed, renamed, or reassigned.
- State assumptions and unresolved risks explicitly.

## Definition Of Done

- Changed behavior is reflected in docs.
- Document structure changes are reflected in `docs/INDEX.md`.
- Validation evidence is captured.
- Remaining risks or follow-ups are recorded.
