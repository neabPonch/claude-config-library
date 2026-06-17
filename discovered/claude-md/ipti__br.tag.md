---
name: ipti__br.tag
source: https://github.com/ipti/br.tag/blob/6270c6075283de3b5cd9f0647c8ba345fe89a3b3/CLAUDE.md
repo: ipti/br.tag
kind: claude-md
stars: 20
last_pushed: 2026-06-15T16:25:24Z
license: gpl-2.0
score: 9
domains: [engineering-workflows, ai-agents, devops]
tags: [modular, playbook-driven, workflow-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# ipti/br.tag — claude-md

**Why it's worth keeping:** The hierarchy of System Rules → Task Playbooks → Completion Checklists is an elite pattern. This prevents context bloat and ensures specialized procedures (like migrations) are strictly followed through dedicated sub-files.

**Summary:** Acts as a high-level operational router that directs the agent to specialized sub-documents for specific workflows. It shifts from static instructions to a modular 'Command Center' architecture.

**Source credibility:** Solid real-world project with recent activity and a specific niche use case.

**Recency:** Highly current; the modular structure optimizes how Claude Code crawls local file paths for context.

**Source:** [ipti/br.tag/CLAUDE.md](https://github.com/ipti/br.tag/blob/6270c6075283de3b5cd9f0647c8ba345fe89a3b3/CLAUDE.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# TAG — Guia para o Claude

Este projeto usa `.agents/` como mapa operacional. Leia as regras abaixo antes de qualquer tarefa.

## Regras sempre ativas

@.agents/rules/system-overview.md
@.agents/rules/php-standards.md
@.agents/rules/design-system-usage.md
@.agents/rules/migrations.md
@.agents/rules/legacy-routing-and-assets.md
@.agents/rules/e2e-testing.md

## Playbooks disponíveis

Antes de iniciar uma tarefa, identifique o playbook correspondente e siga-o:

| Tarefa | Playbook |
|---|---|
| Corrigir bug | `.agents/playbooks/bugfix.md` |
| Verificar qualidade de código | `.agents/playbooks/code-quality.md` |
| Criar ou aplicar migration SQL | `.agents/playbooks/database-migration.md` |
| Migrar controller legado para módulo | `.agents/playbooks/module-migration.md` |
| Refatorar UI para o design system TAG | `.agents/playbooks/ui-refactor.md` |
| Preparar release / PR | `.agents/playbooks/release.md` |
| Executar testes E2E | `.agents/playbooks/e2e-testing.md` |

## Checklists de encerramento

Antes de declarar qualquer tarefa concluída, aplique o checklist adequado:

- Qualquer tarefa → `.agents/checklists/task-done.md`
- Migração de módulo → `.agents/checklists/module-migration
```

</details>
