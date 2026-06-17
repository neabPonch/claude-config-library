---
name: serithemage__serverless-openclaw
source: https://github.com/serithemage/serverless-openclaw/blob/504300de7f56c56d70abf487dccd226883f9c6c8/CLAUDE.md
repo: serithemage/serverless-openclaw
kind: claude-md
stars: 190
last_pushed: 2026-03-29T04:05:25Z
license: unknown
score: 9
domains: [cloud-infrastructure, ai-agents, serverless, aws]
tags: [aws-cdk, serverless-architecture, agentic-workflows, security-constraints]
curated: 2026-06-17
curated_by: config-scout
---

# serithemage/serverless-openclaw — claude-md

**Why it's worth keeping:** The 'Critical Constraints' section prevents expensive/insecure architecture decisions, while the DynamoDB schema and data flow diagrams ensure model accuracy during development.

**Summary:** Provides comprehensive architectural flows, deployment commands, and critical cloud constraints for an AWS server-side agent system.

**Source credibility:** Highly credible; 190 stars on a specialized open-source AI agent infrastructure project.

**Recency:** Very current (last push 3 months ago) and optimized for modern Claude Code workflows.

**Source:** [serithemage/serverless-openclaw/CLAUDE.md](https://github.com/serithemage/serverless-openclaw/blob/504300de7f56c56d70abf487dccd226883f9c6c8/CLAUDE.md) · 190★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Agent Compatibility

This repository supports both Claude Code and Codex.

- Canonical skill source: `.agents/skills/`
- Generated mirrors: `.claude/skills/` and `.codex/skills/`
- When updating a skill, edit `.agents/skills/` first and then run `npm run skills:sync`
- Use `npm run skills:check` to verify the Claude/Codex mirrors are still identical to the canonical source
- Keep `CLAUDE.md` and `AGENTS.md` aligned when agent-facing rules or shared workflows change
- Prefer agent-neutral instructions. If a workflow can use subagents, make that optional and include a sequential fallback

## Project

Serverless OpenClaw — Runs the OpenClaw AI agent on-demand on AWS serverless infrastructure. Web UI + Telegram interface. Cost target ~$1/month.

## Build & Dev Commands

```bash
npm run build          # tsc --build (all packages via project references)
npm run lint           # eslint "packages/**/*.ts"
npm run format         # prettier
npm run test           # vitest run (unit tests, excludes *.e2e.test.ts)
npm run test:e2e       # vitest e2e (CDK synth E2E tests)
npm
```

</details>
