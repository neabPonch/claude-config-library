---
name: artubss__SKILLS-CLAUDE-CODE__skill
source: https://github.com/artubss/SKILLS-CLAUDE-CODE/blob/ac67ed85889b15fa9e784e2a93a83f8916870698/favorites/tpl-backend-elixir-phoenix/SKILL.md
repo: artubss/SKILLS-CLAUDE-CODE
kind: skill
stars: 7
last_pushed: 2026-05-16T15:21:14Z
license: unknown
score: 8
domains: [backend-api, web-development]
tags: [elixir, phoenix, architecture, patterns]
curated: 2026-06-15
curated_by: config-scout
---

# artubss/SKILLS-CLAUDE-CODE — skill

**Why it's worth keeping:** It enforces critical patterns like 'Contexts as public API' and provides concrete, production-ready implementations of Ecto changesets and error handling.

**Summary:** Establishes strict architectural guardrails and idiomatic coding standards for Elixir Phoenix applications.

**Source credibility:** The repo appears to be a curated collection of project templates with recent maintenance.

**Recency:** Current; utilizes modern Elixir 1.16 and OTP 26 standards.

**Source:** [artubss/SKILLS-CLAUDE-CODE/favorites/tpl-backend-elixir-phoenix/SKILL.md](https://github.com/artubss/SKILLS-CLAUDE-CODE/blob/ac67ed85889b15fa9e784e2a93a83f8916870698/favorites/tpl-backend-elixir-phoenix/SKILL.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tpl-backend-elixir-phoenix
description: Template do pack (backend/10-elixir-phoenix.md). Orienta o agente em APIs, servicos e arquitetura backend alinhado a esse contexto.
metadata:
  version: 1.0.0
  source_template: backend/10-elixir-phoenix.md
  generated_by: install_pack_templates_as_claude_skills
---

# PROJECT: Elixir Phoenix API + LiveView App

Skill gerado a partir do pack `templates-claude-code`. Arquivo de origem: `backend/10-elixir-phoenix.md`. Use como baseline e adapte ao projeto antes de mudancas grandes.

## Conteudo do template

## STACK
- **Language:** Elixir 1.16 / OTP 26
- **Framework:** Phoenix 1.7 + Phoenix LiveView 0.20
- **Database:** PostgreSQL via Ecto 3.11
- **Testing:** ExUnit + Mox + Wallaby (E2E)
- **Linting:** Credo + Dialyzer
- **Auth:** phx_gen_auth (sessions) or Guardian (JWT)

---

## PROJECT STRUCTURE
```
lib/
├── my_app/                   # Core business logic (Contexts)
│   ├── accounts/
│   │   ├── accounts.ex       # Public context API
│   │   ├── user.ex           # Ecto schema
│   │   └── user_token.ex
│   ├── blog/
│   │   ├── blog.ex
│   │   └── post.ex
│   └── workers/
│       └── email_worker.ex   # GenServer / Oban job
├── my_
```

</details>
