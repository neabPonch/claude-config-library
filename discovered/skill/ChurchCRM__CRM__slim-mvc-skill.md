---
name: ChurchCRM__CRM__slim-mvc-skill
source: https://github.com/ChurchCRM/CRM/blob/2834ffd98c15c7f1b647b186f51be467bf782ac5/.agents/skills/churchcrm/slim-mvc-skill.md
repo: ChurchCRM/CRM
kind: skill
stars: 895
last_pushed: 2026-06-15T15:36:13Z
license: mit
score: 8
domains: [backend-api, web-architecture, security]
tags: [slim-php, mvc-migration, architectural-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# ChurchCRM/CRM — skill

**Why it's worth keeping:** Effective use of architectural mapping, security-per-group considerations, and explicit 'keep vs move' logic for large-scale refactoring tasks.

**Summary:** Maps existing Slim MVC route structures and provides specific middleware implementation patterns for data validation.

**Source credibility:** High; based on a well-maintained open-source ChMS project.

**Recency:** Current/Modern

**Source:** [ChurchCRM/CRM/.agents/skills/churchcrm/slim-mvc-skill.md](https://github.com/ChurchCRM/CRM/blob/2834ffd98c15c7f1b647b186f51be467bf782ac5/.agents/skills/churchcrm/slim-mvc-skill.md) · 895★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
title: "Slim MVCs — Routes, Uses, Security & Migration Guidance"
intent: "Inventory Slim MVCs and provide migration guidance for group apps"
tags: ["slim","mvc","routing","migration","security"]
prereqs: ["routing-architecture.md","slim-4-best-practices.md"]
complexity: "intermediate"
---

**Slim MVCs — Skill: Routes, Uses, Security & Migration Guidance**

Overview
- **Purpose:** Inventory current Slim MVCs (route groups / folders), explain what each is used for, list security and operational considerations, and provide a migration plan to create new MVC apps/groups (SundaySchool, Congregation) and move appropriate `v2` and `api` functionality into them.

Middleware: FamilyMiddleware <!-- learned: 2026-03-03 -->

- **Purpose:** When an API route accepts a `familyId` path parameter, prefer attaching the `FamilyMiddleware` to centralize lookup, validation, and error responses. The middleware loads the `Family` model and attaches it to the request as the `family` attribute so handlers receive a validated object.

Example:

```php
// attach middleware to the route
$group->get('/neighbors/{familyId:[0-9]+}', 'getMapNeighbors')->add(\ChurchCRM\Slim\Middleware\Api\FamilyMiddleware::cl
```

</details>
