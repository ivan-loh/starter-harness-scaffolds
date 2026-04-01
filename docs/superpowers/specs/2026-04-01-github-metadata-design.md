# GitHub Metadata Design

## Summary

Set up clean, minimal GitHub metadata for the starter harness landing repo and the three template repos.

The metadata should make the repo network easier to discover, easier to understand, and easier to use without turning it into a heavy marketing surface.

## Goal

Improve the public GitHub setup by:

- making the landing repo clearly act as the chooser and explainer
- making the three template repos clearly act as direct starting points
- using short, simple descriptions
- adding lightweight discovery topics
- linking the template repos back to the landing repo
- using one consistent license across all repos

## Repo Roles

### Landing repo

Repo:

`starter-harness-scaffolds`

Role:

Landing and chooser repo. It should explain the system, point people to the right template repo, and not act like the main template itself.

This repo should stay a normal repository, not a GitHub template repository.

### Template repos

Repos:

- `starter-harness-minimal`
- `starter-harness-balanced`
- `starter-harness-full`

Role:

Direct template repositories that users start from.

These repos should remain GitHub template repositories.

## Descriptions

### Landing repo description

`Docs-first starter harnesses for AI-to-production projects, with minimal, balanced, and full templates.`

### Template repo descriptions

`starter-harness-minimal`

`Minimal docs-first starter harness template for new software projects.`

`starter-harness-balanced`

`Balanced docs-first starter harness template for small product teams.`

`starter-harness-full`

`Full docs-first starter harness template for projects that need deeper engineering and operations docs.`

## Homepage URLs

### Landing repo

Leave the homepage URL blank for now because there is no external project site yet.

### Template repos

Set the homepage URL for all three template repos to:

`https://github.com/ivan-loh/starter-harness-scaffolds`

This gives template-repo visitors a clear way back to the landing repo.

## Topics

Keep the topic set small and clear.

### Shared base topics

- `template-repository`
- `project-template`
- `documentation`
- `documentation-template`
- `developer-tools`
- `claude-code`
- `starter-kit`
- `ai-engineering`

### Landing repo extra topic

- `software-projects`

### Template repo variant topic

Add one variant-specific topic to each template repo:

- `starter-harness-minimal`: `minimal`
- `starter-harness-balanced`: `balanced`
- `starter-harness-full`: `full`

## License

Use the `MIT` license for:

- `starter-harness-scaffolds`
- `starter-harness-minimal`
- `starter-harness-balanced`
- `starter-harness-full`

The license should exist both in the GitHub metadata and in each repository as a root `LICENSE` file.

## README Direction

The landing repo `README.md` already contains hard links to:

- `starter-harness-minimal`
- `starter-harness-balanced`
- `starter-harness-full`

No extra README rewrite is needed for this metadata change unless verification shows a missing or broken link.

## Explicit Decisions

- Do not make `starter-harness-scaffolds` a template repo.
- Keep `starter-harness-scaffolds` as the landing and chooser repo.
- Keep the metadata minimal and consistent.
- Do not add a homepage URL to the landing repo yet.
- Set each template repo homepage URL back to the landing repo.
- Use `MIT` across all four repos.

## Verification

Before this work is considered done:

- confirm `starter-harness-scaffolds` is not a template repo
- confirm all three template repos are template repos
- confirm each repo has the approved description
- confirm the landing repo homepage is blank
- confirm each template repo homepage points to the landing repo
- confirm each repo has the expected topic set
- confirm each repo has an MIT license
- confirm the landing repo README still hard-links to all three template repos
