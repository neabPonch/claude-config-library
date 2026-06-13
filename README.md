# claude-config-library

A curated, community-researched collection of `CLAUDE.md` files, skill definitions, and workflow practices for Claude Code — organized by domain and stack, with a built-in advisor that generates tailored configs for your project.

---

## What's in here

| Directory | Contents |
|-----------|----------|
| [`claude-md/`](claude-md/) | CLAUDE.md templates by domain and stack |
| [`skills/`](skills/) | Skill definitions (`.md` skill files) by domain and stack |
| [`workflows/`](workflows/) | Workflow practices, patterns, and integration guides |
| [`advisor/`](advisor/) | The "choose your own adventure" config generator |

---

## Quick start — Advisor

**Option A: Claude Code (recommended)**

```bash
git clone https://github.com/YOUR_USERNAME/claude-config-library
cd claude-config-library
claude
```

Then just ask:

> *"I'm building a Next.js SaaS with a Python FastAPI backend and Postgres. Generate my CLAUDE.md and skill files."*

The repo's own `CLAUDE.md` instructs Claude to act as an advisor, read the library, and compose a tailored config set.

**Option B: Standalone prompt**

Paste the contents of [`advisor/prompts/advisor.md`](advisor/prompts/advisor.md) into any Claude session and follow the questionnaire.

---

## Taxonomy

Configs are organized along two axes:

- **Domain** — what you're building (web-frontend, backend-api, data-ml, devops-infra, mobile, security, agents-ai, game-dev, data-engineering, cli-tools)
- **Stack** — the specific technologies (react-nextjs, python-fastapi, go, rust, node-express, django, swift-ios, android-kotlin)

A project may draw from multiple domains and stacks. The advisor handles composition.

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). The short version: add a CLAUDE.md or skill file under the right domain/stack folder, update [`catalog.json`](catalog.json), and open a PR.

---

## Scope

This repo covers:
- **CLAUDE.md files** — project-level instructions, tone, conventions, tool permissions, anti-patterns
- **Skill files** — reusable `/skill` definitions for recurring tasks
- **Workflow practices** — how to structure work with Claude Code (PR flows, debugging approaches, test strategies)
- **Advisor logic** — prompts and templates for generating configs on demand
