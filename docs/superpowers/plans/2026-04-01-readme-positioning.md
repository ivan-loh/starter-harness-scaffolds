# README Positioning Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Rewrite the root README so it explains the project in simple English, targets small product teams using AI, recommends the balanced scaffold by default, and links directly to the three scaffold repos.

**Architecture:** Keep the change focused on the root `README.md`. Replace the current structure-first opening with audience-first positioning, then keep only the setup and reference sections that still help public readers. Preserve accurate repo details while removing the folder-copy workflow as the main path.

**Tech Stack:** Markdown, GitHub repository links

---

### Task 1: Rewrite README messaging and setup flow

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Review the current README before editing**

Run:

```bash
sed -n '1,260p' README.md
```

Expected: The current README opens with `Starter Harness Engineering Scaffolds` and tells users to copy scaffold folders from this repository.

- [ ] **Step 2: Replace the README with the approved public-facing structure**

Write this content to `README.md`:

```md
# Starter Harness for AI-to-Production Projects

Help small product teams move fast with AI while keeping the repo clear enough for engineers to review, fix, and deploy.

This repository gives you starter scaffolds for new projects.

They help teams set up the basic docs, rules, and structure early.

The goal is simple: when engineers need to take a project further, the repo is easier to understand and safer to ship.

## Who This Is For

- Small product teams building new software
- Teams using AI tools to move faster in early project work
- Projects that will later need engineers to review, clean up, harden, and deploy
- Teams that want better docs and clearer handoff from day one

## Why This Exists

Many small teams can build fast with AI.

The hard part comes later.

When engineers need to fix bugs, review changes, improve the code, and deploy safely, they often inherit a repo with missing context and weak structure.

This starter harness helps teams set up the basic docs and working rules early, so the project is easier to understand and easier to ship later.

## Choose a Scaffold

If you are not sure, start with `balanced`.

- `minimal`
  Best for small repos that need the core docs and a simple working structure.
- `balanced`
  Best for most small product teams. It adds security, roadmap, risks, and contribution docs on top of the core set.
- `full`
  Best for projects that also need deeper docs for design, API, data, operations, deployment, and release work.

## Scaffold Repos

- [`starter-harness-minimal`](https://github.com/ivan-loh/starter-harness-minimal)
- [`starter-harness-balanced`](https://github.com/ivan-loh/starter-harness-balanced)
- [`starter-harness-full`](https://github.com/ivan-loh/starter-harness-full)

## How to Start

1. Pick the scaffold that fits your project.
2. Open the scaffold repo for that option.
3. Clone that repo or use it as the base for your new project.
4. Replace the placeholder text.
5. Fill in the core docs first.
6. Keep the docs updated as the project changes.

## How the Scaffolds Work

Each scaffold is a separate repository that gives you a starting set of docs for a new software project.

In every scaffold:

- `README.md` is the main file for humans
- `CLAUDE.md` is the main file for Claude Code
- `docs/INDEX.md` is the file map for the docs

## Human Workflow After Setup

1. Open the scaffold `README.md`.
2. Fill in the project name, setup, and commands.
3. Read `docs/INDEX.md` to see what each doc is for.
4. Update the core docs first.
5. Keep the docs aligned with the real repository structure.

## LLM Workflow After Setup

For another LLM working in the copied repository:

1. Read `CLAUDE.md` first.
2. Read `docs/INDEX.md` second.
3. Use `docs/INDEX.md` as the file map.
4. Read the task-specific docs after that.
5. Do not create a second file index somewhere else.
6. Update `docs/INDEX.md` and the affected docs when structure or behavior changes.

## Placeholder Tokens

The scaffold files keep a small set of placeholders:

- `{{PROJECT_NAME}}`
- `{{PROJECT_SLUG}}`
- `{{PROJECT_DESCRIPTION}}`
- `{{OWNER_NAME}}`
- `{{PRIMARY_LANGUAGE}}`
- `{{DEFAULT_BRANCH}}`
- `{{CURRENT_DATE}}`
- `{{CURRENT_YEAR}}`

These placeholders are expected in the scaffold files and should be replaced after starting from a scaffold repository.

## References

The research references and rationale for this structure live in [REFERENCES.md](REFERENCES.md).
```

- [ ] **Step 3: Review the diff for scope and wording**

Run:

```bash
git diff -- README.md
```

Expected: The diff shows a simpler, audience-first README with direct links to the three scaffold repos and no top-level copy-from-this-repo workflow.

- [ ] **Step 4: Commit the README rewrite**

Run:

```bash
git add README.md
git commit -m "docs: rewrite readme for clearer positioning"
```

Expected: Git creates a commit containing only the README rewrite.

### Task 2: Verify the updated README

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Read the updated README top to bottom**

Run:

```bash
sed -n '1,260p' README.md
```

Expected: The title, promise, audience, explanation, scaffold choice, repo links, and setup flow all read clearly in simple English.

- [ ] **Step 2: Confirm the scaffold repo links are correct**

Run:

```bash
gh repo view ivan-loh/starter-harness-minimal --json url
gh repo view ivan-loh/starter-harness-balanced --json url
gh repo view ivan-loh/starter-harness-full --json url
```

Expected: Each command returns the matching GitHub URL used in `README.md`.

- [ ] **Step 3: Confirm the new README recommends balanced by default**

Run:

```bash
rg -n 'If you are not sure, start with `balanced`\.' README.md
```

Expected: One match in the `Choose a Scaffold` section.

- [ ] **Step 4: Confirm the old copy-from-this-repo path is gone**

Run:

```bash
rg -n 'cp -R|copy that scaffold into the root of a new repository|Pick one scaffold in `scaffolds/`' README.md
```

Expected: No matches.

- [ ] **Step 5: Summarize completion status**

Report:

```text
README rewritten, scaffold links verified, default recommendation confirmed, old setup path removed.
```
