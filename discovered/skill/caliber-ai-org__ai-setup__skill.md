---
name: caliber-ai-org__ai-setup__skill
source: https://github.com/caliber-ai-org/ai-setup/blob/d59ae5bcf4d8f9ad61e5ebad265a5cbd4d132662/skills/adding-a-command/SKILL.md
repo: caliber-ai-org/ai-setup
kind: skill
stars: 1129
last_pushed: 2026-05-20T12:24:52Z
license: mit
score: 9
domains: [cli-tools, typescript, devops]
tags: [cli, commander-js, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# caliber-ai-org/ai-setup — skill

**Why it's worth keeping:** Uses a high-quality 'Critical/Instructions/Examples/Common Issues' structure and defines precise architectural contracts like the unique '__exit__' error pattern and ESM import rules.

**Summary:** Provides rigorous engineering standards for adding new CLI commands, covering registration logic, specific error handling patterns, and telemetry wrapping.

**Source credibility:** High; source repo has 1k+ stars and specific focus on AI agent configurations.

**Recency:** Very current, utilizing modern TypeScript and ESM module resolution patterns.

**Source:** [caliber-ai-org/ai-setup/skills/adding-a-command/SKILL.md](https://github.com/caliber-ai-org/ai-setup/blob/d59ae5bcf4d8f9ad61e5ebad265a5cbd4d132662/skills/adding-a-command/SKILL.md) · 1129★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: adding-a-command
description: Creates a new CLI command following the Commander.js pattern in src/commands/. Handles command registration in src/cli.ts, telemetry tracking via tracked() wrapper, and option parsing. Use when user says add command, new CLI command, create subcommand, or adds files to src/commands/. Do NOT use for modifying existing commands or fixing bugs in existing commands.
paths:
  - src/commands/**/*.ts
  - src/cli.ts
---
# Adding a Command

## Critical

- **Export pattern**: Command must export a named async function: `export async function myCommand(options?: OptionType)`. Never use default exports.
- **Registration in cli.ts**: Every command must be imported and registered with `.command()` chain in `src/cli.ts`, wrapped with `tracked()` for telemetry.
- **Error signaling**: Use `throw new Error('__exit__')` to exit gracefully without printing the error message. Use chalk for user-facing messages.
- **Options typing**: Commands receiving options must define a TypeScript interface for those options. Pass options as a destructured object parameter.

## Instructions

1. **Create the command file** at `src/commands/{commandName}.ts` with named async exp
```

</details>
