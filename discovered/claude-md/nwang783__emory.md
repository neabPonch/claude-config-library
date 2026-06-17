---
name: nwang783__emory
source: https://github.com/nwang783/emory/blob/c6683177984f36dd3ac308abe3a3145f43d72c6f/CLAUDE.md
repo: nwang783/emory
kind: claude-md
stars: 1
last_pushed: 2026-03-22T15:52:40Z
license: unknown
score: 7
domains: [agents-ai, cli-tools, monorepo]
tags: [skill-registry, agentic-workflows]
curated: 2026-06-16
curated_by: config-scout
---

# nwang783/emory — claude-md

**Why it's worth keeping:** It demonstrates an excellent pattern of defining slash-style command skills, providing the LLM with high-level action triggers for complex tasks.

**Summary:** Establishes project topology and provides a structured registry of specialized 'gstack' skills for agentic workflows.

**Source credibility:** Low star count; appears to be a highly specialized or private developer environment.

**Recency:** Current; updated within the last 3 months.

**Source:** [nwang783/emory/CLAUDE.md](https://github.com/nwang783/emory/blob/c6683177984f36dd3ac308abe3a3145f43d72c6f/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Emory — agent context

Monorepo: Electron + React desktop (`apps/desktop`), shared packages (`packages/core`, `packages/db`), Swift iOS app (`emory/`). Domain docs live under [`docs/README.md`](docs/README.md).

## gstack

**`.agents/`** is gitignored. Install [gstack](https://github.com/garrytan/gstack) locally under **`.agents/skills/gstack/`** and run `./setup --host codex` (see [`docs/agents/gstack.md`](docs/agents/gstack.md)). Optionally materialize **`gstack-*`** / **`gstack-workflow`** stubs under **`.agents/skills/`** for Cursor discovery.

- Use **gstack’s browser workflow** (`/browse`, `/qa`, etc.) when following gstack skills — after install, see **`.agents/skills/gstack/BROWSER.md`**, or [BROWSER.md upstream](https://github.com/garrytan/gstack/blob/main/BROWSER.md). On Windows, Playwright uses **Node** (not Bun) per upstream notes.
- If skills or the browse binary seem stale after pulling: from Git Bash run  
  `cd .agents/skills/gstack && ./setup --host codex`
- Full setup notes: [`docs/agents/gstack.md`](docs/agents/gstack.md)

**Available gstack skills (slash-style prompts):**  
`/office-hours`, `/plan-ceo-review`, `/plan-eng-review`, `/plan-design-review`, `/desig
```

</details>
