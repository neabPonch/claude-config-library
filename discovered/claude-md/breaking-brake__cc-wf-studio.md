---
name: breaking-brake__cc-wf-studio
source: https://github.com/breaking-brake/cc-wf-studio/blob/f612b1cb0e33dbc9d19fd176f997ffcaedd9a387/CLAUDE.md
repo: breaking-brake/cc-wf-studio
kind: claude-md
stars: 5115
last_pushed: 2026-06-14T03:20:25Z
license: other
score: 8
domains: [vscode-extension, monorepo, cli-tools, typescript]
tags: [pnpm, monorepo, strict-workflow, automation-safety]
curated: 2026-06-15
curated_by: config-scout
---

# breaking-brake/cc-wf-studio — claude-md

**Why it's worth keeping:** It includes explicit 'AI prohibitions' to prevent irreversible actions like manual releases and provides highly specific command sequences for code validation.

**Summary:** Detailed technical guide for managing a pnpm monorepo used in building a VSCode extension and CLI tool.

**Source credibility:** High credibility; the repository is well-starred (5k+) and actively maintained.

**Recency:** Highly current, featuring modern tech stacks like TypeScript 5.x and React 18.2.

**Source:** [breaking-brake/cc-wf-studio/CLAUDE.md](https://github.com/breaking-brake/cc-wf-studio/blob/f612b1cb0e33dbc9d19fd176f997ffcaedd9a387/CLAUDE.md) · 5115★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# cc-wf-studio Development Guidelines

Auto-generated from all feature plans. Last updated: 2025-11-01

## Language

- GitHub Issues and Pull Requests (titles, bodies, and comments) MUST be written in English.
- This applies regardless of the conversation language used with Claude.

## Active Technologies
- ローカルファイルシステム (`.vscode/workflows/*.json`, `.claude/skills/*.md`, `.claude/commands/*.md`) (001-cc-wf-studio)
- TypeScript 5.3 (VSCode Extension Host), React 18.2 (Webview UI) (001-node-types-extension)
- ローカルファイルシステム (`.vscode/workflows/*.json`) (001-node-types-extension)
- TypeScript 5.3.0 (001-skill-node)
- File system (SKILL.md files in `~/.claude/skills/` and `.claude/skills/`), workflow JSON files in `.vscode/workflows/` (001-skill-node)
- TypeScript 5.3.0 (VSCode Extension Host), TypeScript/React 18.2 (Webview UI) + VSCode Extension API 1.80.0+, React 18.2, React Flow (visual canvas), Zustand (state management), child_process (Claude Code CLI execution) (001-mcp-node)
- Workflow JSON files in `.vscode/workflows/` directory, Claude Code MCP configuration (user/project/enterprise scopes) (001-mcp-node)
- TypeScript 5.3.0 (VSCode Extension Host), TypeScript/React 18.2 (Webvie
```

</details>
