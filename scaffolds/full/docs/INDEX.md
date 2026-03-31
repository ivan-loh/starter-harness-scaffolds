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
- `CONTRIBUTING.md`: change and review process
- `SECURITY.md`: public security reporting
- `CHANGELOG.md`: notable changes over time
- `CODEOWNERS`: review ownership by path

## Core Docs

- `docs/HARNESS_GUIDE.md`: how this doc set is meant to work
- `docs/DEVELOPMENT.md`: local setup, commands, and working rules
- `docs/PRD.md`: goals, scope, and requirements
- `docs/ARCHITECTURE.md`: system shape and key boundaries
- `docs/GLOSSARY.md`: common terms and naming rules
- `docs/DESIGN.md`: current technical design
- `docs/API.md`: interfaces and contract rules
- `docs/DATA_MODEL.md`: entities and data rules
- `docs/SECURITY.md`: internal security model and controls
- `docs/TESTING.md`: testing layers and required checks
- `docs/OPERATIONS.md`: runtime ownership and support
- `docs/OBSERVABILITY.md`: logs, metrics, traces, and alerts
- `docs/DEPLOYMENT.md`: rollout and rollback process
- `docs/RELEASE.md`: release process and versioning
- `docs/ROADMAP.md`: planned next work
- `docs/RISKS.md`: current risks and assumptions
- `docs/DECISIONS.md`: ADR rules and index

## Where To Look

- What is this project and why does it exist? `README.md`, `docs/PRD.md`
- How do I run it locally? `docs/DEVELOPMENT.md`
- How is it structured? `docs/ARCHITECTURE.md`, `docs/DESIGN.md`
- What interfaces or schemas does it expose? `docs/API.md`, `docs/DATA_MODEL.md`
- How do we handle internal security? `docs/SECURITY.md`
- How do people report vulnerabilities? `SECURITY.md`
- How do we test it? `docs/TESTING.md`
- How does it run, deploy, and release? `docs/OPERATIONS.md`, `docs/OBSERVABILITY.md`, `docs/DEPLOYMENT.md`, `docs/RELEASE.md`
- What should I read next? `docs/INDEX.md`, `CLAUDE.md`

## Governance And Workflow

- `CONTRIBUTING.md`: contribution rules
- `SECURITY.md`: public reporting policy
- `CHANGELOG.md`: release history
- `CODEOWNERS`: review routing
- `.github/PULL_REQUEST_TEMPLATE.md`: PR checklist
- `.github/ISSUE_TEMPLATE/*`: issue templates

## Runbooks

- `docs/runbooks/incident-template.md`: incident response template
- `docs/runbooks/rollback-template.md`: rollback template

## Feature Workflow

- `docs/specs/FEATURE_SPEC_TEMPLATE.md`: feature problem and outcome
- `docs/specs/IMPLEMENTATION_PLAN_TEMPLATE.md`: technical plan for an approved spec
- `docs/specs/TASK_BREAKDOWN_TEMPLATE.md`: small reviewable tasks
