---
name: epicweb-dev__epic-stack__skill
source: https://github.com/epicweb-dev/epic-stack/blob/faaa21779c66002ba4c50890828b1b917cadbef2/docs/skills/epic-permissions/SKILL.md
repo: epicweb-dev/epic-stack
kind: skill
stars: 5535
last_pushed: 2026-06-02T16:17:04Z
license: mit
score: 9
domains: [web-development, security, backend]
tags: [rbac, permissions, typescript, access-control]
curated: 2026-06-15
curated_by: config-scout
---

# epicweb-dev/epic-stack — skill

**Why it's worth keeping:** Uses 'Good vs Avoid' comparison patterns to teach the philosophy of explicit vs. implicit checks; covers the full lifecycle from Prisma schema to client-side visibility.

**Summary:** Provides a comprehensive pattern for implementing Role-Based Access Control (RBAC) using explicit permission strings.

**Source credibility:** High; part of a highly-regarded, active, and starred full-stack starter kit (Epic Stack).

**Recency:** 

**Source:** [epicweb-dev/epic-stack/docs/skills/epic-permissions/SKILL.md](https://github.com/epicweb-dev/epic-stack/blob/faaa21779c66002ba4c50890828b1b917cadbef2/docs/skills/epic-permissions/SKILL.md) · 5535★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: epic-permissions
description: Guide on RBAC system and permissions for Epic Stack
categories:
  - permissions
  - rbac
  - access-control
---

# Epic Stack: Permissions

## When to use this skill

Use this skill when you need to:

- Implement role-based access control (RBAC)
- Validate permissions on server-side or client-side
- Create new permissions or roles
- Restrict access to routes or actions
- Implement granular permissions (`own` vs `any`)

## Patterns and conventions

### Permissions Philosophy

Following Epic Web principles:

**Explicit is better than implicit** - Always explicitly check permissions.
Don't assume a user has access based on implicit rules or hidden logic. Every
permission check should be visible and clear in the code.

**Example - Explicit permission checks:**

```typescript
// ✅ Good - Explicit permission check
export async function action({ request }: Route.ActionArgs) {
	const userId = await requireUserId(request)

	// Explicitly check permission - clear and visible
	await requireUserWithPermission(request, 'delete:note:own')

	// Permission check is explicit and obvious
	await prisma.note.delete({ where: { id: noteId } })
}

// ❌ Avoid - Impl
```

</details>
