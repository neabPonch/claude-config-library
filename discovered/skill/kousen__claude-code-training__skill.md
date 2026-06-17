---
name: kousen__claude-code-training__skill
source: https://github.com/kousen/claude-code-training/blob/bc8bad3f61697eefe2be00b585301e0e2a9546c9/skills/spring-service/SKILL.md
repo: kousen/claude-code-training
kind: skill
stars: 234
last_pushed: 2026-05-15T15:04:29Z
license: mit
score: 9
domains: [backend-api, java, spring-boot]
tags: [scaffolding, tdd, enterprise-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# kousen/claude-code-training — skill

**Why it's worth keeping:** It enforces strict architectural patterns like constructor injection and specific error-handling strategies. It also includes smart constraints to match existing project styles (Lombok/MapStruct) and uses modern testing annotations like @MockitoBean.

**Summary:** Automates the generation of boilerplate-heavy Spring Boot service layers including CRUD logic, logging, and unit tests.

**Source credibility:** High; part of a dedicated training repo with significant stars and recent updates.

**Recency:** 

**Source:** [kousen/claude-code-training/skills/spring-service/SKILL.md](https://github.com/kousen/claude-code-training/blob/bc8bad3f61697eefe2be00b585301e0e2a9546c9/skills/spring-service/SKILL.md) · 234★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: spring-service
description: Generate a Spring Boot service class for a named entity with constructor injection, logging, exception handling, and unit tests. Invoke as /spring-service <Entity>.
paths:
  - "**/*.java"
user-invocable: true
---

# Spring Service Scaffold

Generate a `$ARGUMENTS`Service with:

- `@Service` annotation
- Constructor injection of `$ARGUMENTS`Repository (no field `@Autowired`)
- CRUD methods: `findAll()`, `findById(id)`, `create(request)`, `update(id, request)`, `delete(id)`
- Domain exceptions (e.g., `EntityNotFoundException`) thrown for missing-by-id; let `@ControllerAdvice` translate to HTTP if present
- SLF4J logging at meaningful boundaries — entry on writes, warn on validation rejection, debug on reads
- Unit tests using JUnit 5 + Mockito, with `@MockitoBean` and `@MockitoSpyBean` where appropriate
- Use modern Java idioms (records for DTOs, pattern matching, `var` where readable)

## Constraints

- Match the existing project package layout
- Don't introduce `Lombok` if the project doesn't already use it
- If the project uses MapStruct, generate a mapper interface; otherwise, write the mapping inline
- Tests should cover happy path, not-foun
```

</details>
