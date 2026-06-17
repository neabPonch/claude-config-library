---
name: Sebs030__micasai-mcp-server
source: https://github.com/Sebs030/micasai-mcp-server/blob/047358354e9802303b259d807c7ef736cba85ccc/CLAUDE.MD
repo: Sebs030/micasai-mcp-server
kind: claude-md
stars: 0
last_pushed: 2026-04-29T19:04:25Z
license: unknown
score: 9
domains: [agents-ai, mcp-servers, backend-api]
tags: [mcp, typescript, firebase, google-auth]
curated: 2026-06-16
curated_by: config-scout
---

# Sebs030/micasai-mcp-server — claude-md

**Why it's worth keeping:** Includes critical runtime constraints (logging to stderr), exact code templates for tool registration, and vital infrastructure prerequisites like vector index requirements.

**Summary:** A highly detailed technical guide for a TypeScript MCP server that manages Firebase/Google OIDC authentication and Firestore integrations.

**Source credibility:** Low public visibility but contains high-density, specialized technical implementation details typical of production tools.

**Recency:** Very current; follows modern MCP SDK patterns and contemporary Firebase/Google auth workflows.

**Source:** [Sebs030/micasai-mcp-server/CLAUDE.MD](https://github.com/Sebs030/micasai-mcp-server/blob/047358354e9802303b259d807c7ef736cba85ccc/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# micasAI MCP Server – Claude Context

## Zweck

Dieser MCP Server verbindet **Claude Desktop** mit der micasAI Hausverwaltungsplattform.
Er ermöglicht natürlichsprachliche Dokumentenabfragen direkt in Claude Desktop.

Lies vor größeren Änderungen:

- `README.md` → Setup, Umgebungsvariablen, Claude Desktop Konfiguration
- `SKILL.md` → Architektur, Tool-Übersicht, Implementierungsdetails

## Stack

- **Sprache:** TypeScript (strict), ESM (`"type": "module"`)
- **Transport:** stdio (für Claude Desktop, nicht HTTP)
- **MCP SDK:** `@modelcontextprotocol/sdk` – nur `registerTool` verwenden, nie veraltete APIs
- **Firebase:** `firebase-admin` v13 – Initialisierung einmalig in `src/services/firebase.ts`
- **Validierung:** Zod mit `.strict()` auf allen Input-Schemas

## Projektstruktur

src/
├── index.ts # Einstiegspunkt: Server-Init, Tool-Registrierung, stdio-Transport
├── types.ts # Interfaces (Spiegel der Firestore-Schemas)
├── constants.ts # IMPower Tag-Gruppen, Status-Labels, CHARACTER_LIMIT
├── services/
│ ├── firebase.ts # Firebase Admin Init + alle Firestore-Queries
│ ├── semanticSearch.ts # HTTP-Client für semanticSearchDocuments Cloud Function
│ └── formatter.ts # Markdown-Format
```

</details>
