---
name: neondatabase__appdotbuild-agent__claude
source: https://github.com/neondatabase/appdotbuild-agent/blob/e087bb0e8b8c442580aacffb89b56d504909bdb8/edda/edda_templates/trpc_bundle/template/%7B%7B.project_name%7D%7D/CLAUDE.md
repo: neondatabase/appdotbuild-agent
kind: claude-md
stars: 757
last_pushed: 2026-05-16T18:34:13Z
license: apache-2.0
score: 9
domains: [fullstack, typescript, databricks, web-frontend]
tags: [trpc, databricks, tailwind, react]
curated: 2026-06-15
curated_by: config-scout
---

# neondatabase/appdotbuild-agent — claude-md

**Why it's worth keeping:** Uses 'Wrong vs. Correct' code blocks to prevent common errors with the Databricks client; provides explicit negative constraints (e.g., forbidding Vitest) to ensure testing consistency.

**Summary:** A highly specific instruction set for a tRPC/Databricks full-stack template that enforces strict type safety and styling patterns.

**Source credibility:** Strongly credible; comes from a popular repository (757 stars) used for generating working applications.

**Recency:** Very current; pushed within the last month.

**Source:** [neondatabase/appdotbuild-agent/edda/edda_templates/trpc_bundle/template/{{.project_name}}/CLAUDE.md](https://github.com/neondatabase/appdotbuild-agent/blob/e087bb0e8b8c442580aacffb89b56d504909bdb8/edda/edda_templates/trpc_bundle/template/%7B%7B.project_name%7D%7D/CLAUDE.md) · 757★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
TypeScript full-stack template with tRPC for type-safe API communication between React frontend and Node.js backend. Use this when building type-safe TypeScript applications with the following structure:
- server/: Node.js backend with tRPC API
- client/: React frontend with tRPC client

## Testing Guidelines:

**CRITICAL**: Use Node.js native test runner only. Do NOT import vitest, jest, or supertest.
Put tests next to the code (e.g. src/*.test.ts)

```typescript
import { test } from "node:test";
import { strict as assert } from "node:assert";
```

## Databricks Type Handling:

- **executeQuery REQUIRES Zod schema**: Pass the Zod schema object as second parameter, NOT a TypeScript type annotation
  ```typescript
  // ❌ WRONG - Do NOT use generic type parameter
  const result = await client.executeQuery<MyType>(sql);

  // ✅ CORRECT - Pass Zod schema as parameter
  const mySchema = z.object({ id: z.number(), name: z.string() });
  const result = await client.executeQuery(sql, mySchema);
  ```
- **QueryResult access**: `executeQuery()` returns `{rows: T[], rowCount: number}`. Always use `.rows` property: `const {rows} = await client.executeQuery(...)` or `result.rows.map(...)`
- **T
```

</details>
