# Starter Harness Engineering Scaffolds

> Purpose: Explain the scaffold variants, how to copy one into a new repository, and how humans or LLMs should use it after copying.
> When to update: When the scaffold layout, references, or variant boundaries change.
> Owner: Template maintainers.

## Overview

This repository contains three documentation scaffolds for new software projects.

Each scaffold is a folder that you copy into a new repository and then edit by hand.

In every scaffold:

- `README.md` is the main file for humans
- `CLAUDE.md` is the main file for Claude Code
- `docs/INDEX.md` is the file map for the docs

No scaffold includes `.cursor`, `AGENTS.md`, or generator scripts.

## Choose A Scaffold

- `scaffolds/minimal`
  - for smaller repos that still need planning, architecture, development, and testing docs
- `scaffolds/balanced`
  - for the usual app-repo case with contribution, security, and governance files
- `scaffolds/full`
  - for systems that also need interface, runtime, deployment, release, and operations docs

## Copy A Scaffold

1. Clone this repository.
2. Pick one scaffold in `scaffolds/`.
3. Copy that scaffold into the root of a new repository.
4. Replace the placeholders.
5. Remove any files you do not need.
6. Update `docs/INDEX.md` if you add, remove, rename, or move docs.

```bash
cp -R scaffolds/balanced/. ../my-new-project/
```

If you publish this repository on GitHub, you can also mark it as a template repository and generate new repositories from it in the GitHub UI.

## Human Workflow After Copying

1. Open the copied `README.md`.
2. Fill in the project name, setup, and commands.
3. Read `docs/INDEX.md` to see what each doc is for.
4. Update the core docs first.
5. Keep the docs aligned with the real repository structure.

## LLM Workflow After Copying

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

These placeholders are expected in the scaffold files and should be replaced after copying a scaffold into a real repository.

## References

The research references and rationale for this structure live in [REFERENCES.md](REFERENCES.md).
