---
name: devlint__GitWand__claude
source: https://github.com/devlint/GitWand/blob/1f583529bf20a6b0ae99b089dfac1b1b933253de/packages/mcp/CLAUDE.md
repo: devlint/GitWand
kind: claude-md
stars: 100
last_pushed: 2026-06-11T22:35:51Z
license: mit
score: 8
domains: [agents-ai, mcp-servers, cli-tools]
tags: [mcp, typescript, tool-calling]
curated: 2026-06-14
curated_by: config-scout
---

# devlint/GitWand — claude-md

**Why it's worth keeping:** Uses structured tables to map tools/resources and includes explicit rules for writing 'AI-readable' descriptions to optimize agent tool-calling precision.

**Summary:** Defines the architecture, tool inventory, and development standards for an MCP server package designed to extend AI capabilities.

**Source credibility:** High; active repo with professional structure and clear technical intent.

**Recency:** Current; contains specific setup instructions for Claude Code configuration.

**Source:** [devlint/GitWand/packages/mcp/CLAUDE.md](https://github.com/devlint/GitWand/blob/1f583529bf20a6b0ae99b089dfac1b1b933253de/packages/mcp/CLAUDE.md) · 100★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
@../../CLAUDE.md

# packages/mcp — @gitwand/mcp

Serveur MCP (Model Context Protocol) exposant les capacités GitWand aux agents AI (Claude Code, Cursor, Windsurf). Thin wrapper autour de `@gitwand/core` — toute logique de résolution reste dans `core`.

## Architecture

```
src/
├── server.ts       # Setup MCP (transport stdio)
├── tools/          # Outils MCP (actions)
└── resources/      # Ressources MCP (données lisibles)
```

**Transport :** stdio (standard MCP)

**3 catégories d'exposition :**
- **Tools** — Actions déclenchables par l'agent
- **Resources** — Données lisibles en temps réel
- **Prompts** — Templates de contexte

## Tools disponibles

| Outil | Description |
|-------|-------------|
| `gitwand_status` | Lister les fichiers en conflit avec confidence scores |
| `gitwand_preview_merge` | Simuler un merge sans l'appliquer |
| `gitwand_resolve_conflicts` | Résoudre les conflits d'un fichier ou de tout le repo |
| `gitwand_explain_hunk` | DecisionTrace complet pour un hunk précis |
| `gitwand_apply_resolution` | Appliquer une résolution fournie par l'agent à un hunk |
| `gitwand_resolve_hunk` | v2.5 — inverser la boucle : GitWand demande à l'agent connecté de proposer l
```

</details>
