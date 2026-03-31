# README Positioning Design

## Summary

Rewrite the root `README.md` so it presents this repository as a simple starter harness for small product teams that build fast with AI and later need engineers to review, fix, and deploy the project.

The new README should read like a public landing page first and an internal usage guide second.

## Goal

Make the repository easier to understand and easier to recommend by:

- explaining the problem it solves in simple English
- naming the main audience clearly
- giving a clear default scaffold choice
- sending users to the separate scaffold repos instead of telling them to copy folders from this repo

## Audience

The README should speak to:

- small product teams starting new software projects
- teams using AI tools to move faster in early project work
- teams that expect engineers to later review, clean up, harden, and deploy the project

## Positioning

Primary positioning:

`Starter Harness for AI-to-Production Projects`

Core promise:

`Help small product teams move fast with AI while keeping the repo clear enough for engineers to review, fix, and deploy.`

## Writing Style

- Use simple English.
- Keep paragraphs short.
- Prefer plain, practical wording over buzzwords.
- Avoid dismissive terms like `vibe coders`.
- Keep the tone calm, useful, and direct.

## Approved README Structure

1. Title
2. One-line promise
3. Short intro
4. `Who This Is For`
5. `Why This Exists`
6. `Choose a Scaffold`
7. Direct links to the scaffold repos
8. `How to Start`
9. Existing lower-level reference sections that still help users, rewritten as needed in simpler English

## Approved Section Content

### Top message

Title:

`Starter Harness for AI-to-Production Projects`

One-line promise:

`Help small product teams move fast with AI while keeping the repo clear enough for engineers to review, fix, and deploy.`

Short intro:

`This repository gives you starter scaffolds for new projects.`

`They help teams set up the basic docs, rules, and structure early.`

`The goal is simple: when engineers need to take a project further, the repo is easier to understand and safer to ship.`

### Who This Is For

- small product teams building new software
- teams using AI tools to move faster in early project work
- projects that will later need engineers to review, clean up, harden, and deploy
- teams that want better docs and clearer handoff from day one

The README should not include a `Not for` section.

### Why This Exists

`Many small teams can build fast with AI.`

`The hard part comes later.`

`When engineers need to fix bugs, review changes, improve the code, and deploy safely, they often inherit a repo with missing context and weak structure.`

`This starter harness helps teams set up the basic docs and working rules early, so the project is easier to understand and easier to ship later.`

### Choose a Scaffold

Lead-in:

`If you are not sure, start with balanced.`

Options:

- `minimal`: Best for small repos that need the core docs and a simple working structure.
- `balanced`: Best for most small product teams. It adds security, roadmap, risks, and contribution docs on top of the core set.
- `full`: Best for projects that also need deeper docs for design, API, data, operations, deployment, and release work.

### Scaffold Repo Links

The README should link directly to:

- `minimal`: `https://github.com/ivan-loh/starter-harness-minimal`
- `balanced`: `https://github.com/ivan-loh/starter-harness-balanced`
- `full`: `https://github.com/ivan-loh/starter-harness-full`

### How to Start

1. Pick the scaffold that fits your project.
2. Open the scaffold repo for that option.
3. Clone that repo or use it as the base for your new project.
4. Replace the placeholder text.
5. Fill in the core docs first.
6. Keep the docs updated as the project changes.

## Explicit Changes From The Current README

- Replace the current opening, which explains the folder structure first, with audience-first positioning.
- Stop telling users to copy scaffold folders out of this repository as the main setup flow.
- Point users to the separate scaffold repositories instead.
- Keep the README useful for real setup work, but make promotion and first-time understanding the top priority.

## Decisions

- Do not add a `Not for` section.
- Do not add a `What This Helps With Later` section.
- Keep the message focused on AI-to-production handoff for small product teams.

## Verification

Before implementation is considered done:

- read the new README top to bottom for plain English and flow
- confirm all three scaffold repo links are correct
- confirm the default recommendation is `balanced`
- confirm the README no longer tells users to copy folders from this repo as the main path
