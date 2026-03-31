# References

> Purpose: Capture the research sources and rationale that informed this starter harness template.
> When to update: When the scaffold structure changes for reasons grounded in new guidance or better source material.
> Owner: Template maintainers.

## How To Read This

- These sources do not all prescribe this exact folder structure.
- Some files in this template are direct platform conventions.
- Other files are informed conventions based on engineering practice and source synthesis.
- Inference: when a source supports a pattern rather than a file name directly, that relationship is noted below.

## Canonical Agent File

- Anthropic Claude Code memory docs
  - `CLAUDE.md` files provide persistent instructions for a project, and Claude reads them at the start of every session.
  - Source: https://code.claude.com/docs/en/memory

## Repository Surface

- GitHub README docs
  - GitHub positions `README.md` as the place to explain why a project is useful, how to get started, where to get help, and who maintains it.
  - Source: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes

- GitHub contributor-guidelines docs
  - `CONTRIBUTING.md` is a first-class way to communicate how changes should be proposed and merged.
  - Source: https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors

- GitHub security-policy docs
  - Root `SECURITY.md` is the public vulnerability-reporting policy and should contain supported versions and reporting instructions.
  - Source: https://docs.github.com/en/code-security/how-tos/report-and-fix-vulnerabilities/configure-vulnerability-reporting/adding-a-security-policy-to-your-repository

- GitHub CODEOWNERS docs
  - `CODEOWNERS` assigns responsible reviewers by path and can be enforced with branch protection.
  - Source: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners

- GitHub issue and pull request template docs
  - PR and issue templates are platform-recognized workflow files for standardizing change and defect intake.
  - Source: https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates

- GitHub template-repository docs
  - GitHub supports template repositories for creating new repos with the same directory structure and files.
  - Source: https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-template-repository

## Planning Workflow

- GitHub spec-driven development post
  - The `spec -> plan -> tasks` workflow informed the `docs/specs/` templates included in all variants.
  - Source: https://github.blog/ai-and-ml/generative-ai/spec-driven-development-with-ai-get-started-with-a-new-open-source-toolkit/

## Writing And Document Structure

- Google technical writing docs
  - Scope and non-scope statements help both readers and writers keep a document useful and focused.
  - Inference: this supports the small purpose headers and tight document ownership model used throughout the scaffold.
  - Source: https://developers.google.com/tech-writing/one/documents

## Architecture And Decisions

- C4 model
  - Context and container diagrams are usually sufficient for most software teams.
  - Inference: this informed the architecture template’s guidance to start with system-context and container views.
  - Source: https://c4model.com/diagrams

- Martin Fowler on ADRs
  - ADRs should be short, capture one important decision, and be superseded instead of rewritten.
  - Source: https://martinfowler.com/bliki/ArchitectureDecisionRecord.html

## Security Engineering

- Microsoft Security Development Lifecycle
  - Threat modeling should start by defining components and interactions and using data-flow diagrams to identify and prioritize threats.
  - Inference: this informed the internal `docs/SECURITY.md` template and its trust-boundary and threat-model sections.
  - Source: https://learn.microsoft.com/en-us/compliance/assurance/assurance-microsoft-security-development-lifecycle

## Release Hygiene

- Keep a Changelog
  - Changelogs should record notable changes in a curated, release-oriented way rather than acting as a raw commit dump.
  - Source: https://keepachangelog.com/en/1.1.0/
