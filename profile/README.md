# VAHU

**Build Better Software, With Better Agents.**

VAHU is an open, agent-agnostic engineering framework for AI-assisted software
development. It provides reusable standards, workflows, technology profiles,
templates, documentation structures, quality gates, and adapters for different
AI coding agents.

VAHU is not a prompt pack and it is not tied to one AI provider. The framework
is designed to remain useful without its CLI, so teams can understand, review,
and change their engineering foundation with ordinary files and tools.

## Vision

Give developers and teams a professional engineering foundation that is
repeatable, inspectable, and maintainable throughout a project's lifecycle.

AI assistance should improve engineering discipline. It should not replace
architecture, human judgement, or clear ownership.

## Core philosophy

- **Agent agnostic** — the framework defines an internal model and adapts it to
  supported agents.
- **Stack agnostic** — projects choose only the technology profiles they need.
- **Engineering first** — standards and verification come before prompts.
- **Documentation first** — documentation is part of implementation.
- **Human approval** — product, architecture, brand, and design decisions need
  explicit approval.
- **Modular** — adopt capabilities incrementally.
- **Transparent** — generated files and configuration stay readable.

## Planned capabilities

VAHU is being built around these capabilities:

- Universal engineering standards and review rules.
- Agent-neutral instructions, rules, skills, and commands.
- Modular technology profiles for backend, frontend, mobile, database, and
  infrastructure choices.
- Project onboarding with explicit identity, design-system, and readiness
  decisions.
- Templates for repositories, documentation, agents, CI/CD, and design systems.
- Quality and security baselines.
- A CLI for validation and project setup.
- Documentation and examples that work independently of the CLI.

These are framework goals. The repository status section below records what is
actually available today.

## Agent ecosystem

The architecture uses agent-neutral content and separate adapters. The initial
compatibility targets under evaluation are:

- OpenAI Codex
- Claude Code
- Gemini CLI
- Generic instruction-based agents

No production adapter is claimed yet. Adapter support will be documented only
when it is implemented and tested.

## Technology approach

VAHU does not assume one language, framework, database, or deployment platform.
Technology profiles will describe their own conventions and requirements.
Projects can combine profiles without inheriting unrelated standards.

The canonical technology-profile location is
[`packages/framework/technology-profiles/`](https://github.com/Vahu-EF/vahu/tree/main/packages/framework/technology-profiles).
There is no second root-level profile tree.

## Repositories

- [vahu](https://github.com/Vahu-EF/vahu) — framework source, CLI, documentation,
  templates, profiles, website source, and examples.
- [.github](https://github.com/Vahu-EF/.github) — organization profile and
  community health files.

## Current status

VAHU is in **Phase 0: Foundation and Architecture**. The repository contains the
initial TypeScript workspace, a small working CLI, the versioned project
configuration schema, documentation, CI workflows, and validation tests. The
framework content, full onboarding flow, technology profiles, agent adapters,
releases, and production website are planned, not complete.

There is no public npm release or GitHub Release yet.

## Contributing

Contribution guidelines, issue templates, and pull-request templates live in the
main repository. Early contributions should focus on correctness, documentation,
tests, and small, reviewable foundation work.

Please read the [contribution guide](https://github.com/Vahu-EF/vahu/blob/main/CONTRIBUTING.md)
and [security policy](https://github.com/Vahu-EF/vahu/blob/main/SECURITY.md)
before opening a pull request.

## License

The main repository is intended to be released under the Apache License 2.0.
See the repository's `LICENSE` file for the authoritative text.
