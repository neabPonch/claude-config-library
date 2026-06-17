---
name: sazardev__goca__improved-goca-skill
source: https://github.com/sazardev/goca/blob/8aaeb51ba7ee75af315f55e6bb48054b626dd33e/.opencode/plans/improved-goca-skill.md
repo: sazardev/goca
kind: skill
stars: 201
last_pushed: 2026-06-14T21:38:00Z
license: mit
score: 9
domains: [backend-api, go-lang, cli-tools, software-architecture]
tags: [scaffolding, clean-architecture, code-generation]
curated: 2026-06-16
curated_by: config-scout
---

# sazardev/goca — skill

**Why it's worth keeping:** It includes architectural violation rules, specific multi-step workflow patterns, and a detailed error-tracing table that allows an agent to troubleshoot generation failures independently.

**Summary:** A highly specialized skill file that provides the Goca CLI tool's full operational context to an agent.

**Source credibility:** Strong; the documentation is structured professionally for a growing Go project (201 stars).

**Recency:** Current; mentions modern integration capabilities like MCP servers.

**Source:** [sazardev/goca/.opencode/plans/improved-goca-skill.md](https://github.com/sazardev/goca/blob/8aaeb51ba7ee75af315f55e6bb48054b626dd33e/.opencode/plans/improved-goca-skill.md) · 201★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Goca CLI — AI Agent Skill

## Description
Specialized skill for AI agents using **Goca** (Go Clean Architecture Code Generator). Provides complete command reference, workflow patterns, error tracing, and architecture rules based on the actual codebase.

**Activate when:** user mentions `goca`, Clean Architecture code generation, Go project scaffolding, or any goca subcommand.

---

## Clean Architecture — Layer Map

Dependencies point **inward** — each layer only knows the layer below it:

```
HTTP Handler → UseCase Interface → Repository Interface → Domain Entity
   adapter        business logic       persistence          pure logic
```

### Generated directories:

| Layer | Path | Depends On |
|-------|------|------------|
| Domain | `internal/domain/` | Nothing (pure Go) |
| UseCase | `internal/usecase/` | Domain + Repository interfaces |
| Repository | `internal/repository/` | Domain |
| Handler | `internal/handler/` | UseCase interfaces |
| DI | `internal/di/` | All layers (wires concretes) |
| Messages | `internal/messages/` | Nothing |
| Interfaces | `internal/interfaces/` | Nothing (contracts only) |
| Middleware | `internal/middleware/` | Nothing |

**Violations to preve
```

</details>
