---
title: Agent Skills
description: Official Agent Skills from Velella. Extend AI coding assistants with authoritative software end-of-life and deprecation intelligence.
layout: doc
permalink: /skills/
---

Universal capabilities for AI coding assistants. Give Claude Code, Cursor, Copilot, Codex, Windsurf and Antigravity authoritative software lifecycle intelligence.

## Official catalog

Install with the open `skills` CLI into any agent project with a single command.

### velella-sh/ebb

Audits dependencies, runtimes, Docker bases, and GitHub Actions for deprecation and end-of-life before coding agents install or upgrade them. Prevents AI hallucination of deprecated APIs and abandoned packages.

```bash
npx skills add velella-sh/ebb
```

Supported agents: Claude Code, Cursor, GitHub Copilot, Codex, Windsurf, Antigravity.

- [View on skills.sh](https://skills.sh/velella-sh/ebb/ebb)
- [Documentation](https://velella.sh/ebb/skills)
- [Source code](https://github.com/velella-sh/ebb/tree/main/skills/ebb)

## Upcoming skills

Next-generation autonomous guardrails and documentation engines currently in development.

- **velella-sh/offing** (planned): automated migration recipes and code remediation when end-of-life packages or deprecated methods are detected.
- **velella-sh/mizzen** (planned): deterministic documentation validator and schema enforcement for agent-generated Markdown and API references.

## How skills work

Built on the open standard specified by skills.sh and Claude Code plugins.

1. **Declarative Markdown.** Every skill contains a standard `SKILL.md` defining precise trigger conditions, inputs, and output formats.
2. **Zero-dependency CLI.** Runs offline and locally via `ebb check` or `lookup` without mandatory network calls or external tracking.
3. **Structured output.** Returns clear, actionable statuses (`supported`, `deprecated`, `end-of-life`) and cited migration sources.
