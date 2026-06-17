---
name: microsoft__aspire__skill
source: https://github.com/microsoft/aspire/blob/4d4e5f21fb3a92b317d7c6166222c5602adcdebe/.agents/skills/vscode-extension/SKILL.md
repo: microsoft/aspire
kind: skill
stars: 6069
last_pushed: 2026-06-15T01:37:20Z
license: mit
score: 9
domains: [vscode-extension, cli-tools, developer-experience]
tags: [typescript, microsoft, vscode, development-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# microsoft/aspire — skill

**Why it's worth keeping:** It defines critical architectural constraints regarding CLI/Extension coupling and establishes a strict 'reproduce via E2E' workflow to ensure regression testing.

**Summary:** Provides deep technical orientation for the Aspire VS Code extension, including build workflows, localization standards, and CLI compatibility requirements.

**Source credibility:** High; sourced from the official Microsoft Aspire repository which is actively maintained.

**Recency:** Extremely current, with active development documented within the last month.

**Source:** [microsoft/aspire/.agents/skills/vscode-extension/SKILL.md](https://github.com/microsoft/aspire/blob/4d4e5f21fb3a92b317d7c6166222c5602adcdebe/.agents/skills/vscode-extension/SKILL.md) · 6069★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vscode-extension
description: "Use when investigating, developing, debugging, testing, or reviewing Aspire VS Code extension behavior under extension/, including extension UI, command, debugger, RPC, DCP, MCP, and CLI-integration issues or features."
---

# Aspire VS Code Extension

This skill covers working on the Aspire VS Code extension, which lives entirely under
[extension/](../../../extension). It is a TypeScript extension built with **yarn** (pinned via
`packageManager` in `extension/package.json`) and **webpack**, and it communicates with the Aspire
CLI over RPC.

## Orientation

All commands below are run from the `extension/` directory unless noted.

| Path | What it is |
|------|------------|
| `extension/src/extension.ts` | Activation entry point |
| `extension/src/commands/` | Command implementations |
| `extension/src/views/` | Tree views, welcome views, panel UI |
| `extension/src/debugger/` | Debug adapter + per-language debuggers (dotnet, node, python, go) |
| `extension/src/server/`, `extension/src/mcp/`, `extension/src/dcp/` | RPC server, MCP provider, DCP integration |
| `extension/src/loc/strings.ts` | Localized strings (TypeScript-side) |
| `extensio
```

</details>
