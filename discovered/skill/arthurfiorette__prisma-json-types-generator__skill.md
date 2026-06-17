---
name: arthurfiorette__prisma-json-types-generator__skill
source: https://github.com/arthurfiorette/prisma-json-types-generator/blob/95323ea53f415b339171ccbc55d1988061d7815c/skills/prisma-json-types-generator/SKILL.md
repo: arthurfiorette/prisma-json-types-generator
kind: skill
stars: 561
last_pushed: 2026-06-12T15:13:27Z
license: mit
score: 8
domains: [backend-api, database-orm, typescript]
tags: [prisma, type-safety, json, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# arthurfiorette/prisma-json-types-generator — skill

**Why it's worth keeping:** It includes high-density technical rules (AST comment syntax), a clear troubleshooting decision tree, and explicit output expectations for file edits.

**Summary:** Provides specialized instructions for using the prisma-json-types-generator to add type safety to Prisma Json fields via schema comments.

**Source credibility:** Highly credible; the source repository is well-starred and actively maintained.

**Recency:** Current; utilizes modern TypeScript/Prisma patterns and agentic workflow instructions.

**Source:** [arthurfiorette/prisma-json-types-generator/skills/prisma-json-types-generator/SKILL.md](https://github.com/arthurfiorette/prisma-json-types-generator/blob/95323ea53f415b339171ccbc55d1988061d7815c/skills/prisma-json-types-generator/SKILL.md) · 561★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: prisma-json-types-generator
description: Use when creating or updating typed Prisma `Json`, `String`, `String[]`, `Int`, or `Float` fields with prisma-json-types-generator, including `/// [Type]` and `/// ![Type]` comments, enum-like literal fields, inline vs named types, and generated types still showing `JsonValue`, `unknown`, or plain scalar types.
compatibility: Requires file read/edit access and is most useful when the Prisma schema, tsconfig, and TypeScript type declarations are available in the workspace.
---

# Prisma Json Types Generator

Make Prisma `Json`, `String`, `String[]`, `Int`, or `Float` fields type-safe with the smallest correct schema and type-definition change.

This only changes generated TypeScript types after `prisma generate`.

## Core Workflow

1. Read only what you need: the relevant Prisma schema, the existing `PrismaJson` wiring file if there is one, and `tsconfig.json` if the namespace declarations are not being picked up.
2. For first-time installation, generator wiring, or broken setup, read `references/setup.md` before editing fields.
3. Find the target field.
4. Decide whether it should use a named namespace type or a short inline type.
```

</details>
