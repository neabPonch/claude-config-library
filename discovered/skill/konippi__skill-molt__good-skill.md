---
name: konippi__skill-molt__good-skill
source: https://github.com/konippi/skill-molt/blob/3e224ecb9b5e3b8789bef2a56490dbea7e831725/examples/good-skill.md
repo: konippi/skill-molt
kind: skill
stars: 0
last_pushed: 2026-04-18T14:50:16Z
license: mit
score: 9
domains: [backend-api, devops, testing]
tags: [e2e, docker, workflow-template]
curated: 2026-06-17
curated_by: config-scout
---

# konippi/skill-molt — skill

**Why it's worth keeping:** Uses negative triggers to prevent misuse, includes conditional error handling ('If... then'), and documents silent failure modes that an LLM wouldn't otherwise know.

**Summary:** A highly structured workflow for orchestrating Docker-based end-to-end tests including environment setup and teardown.

**Source credibility:** Low star count but high-quality human curation evident in the meta-analysis provided.

**Recency:** Current; aligns perfectly with modern agentic CLI workflows.

**Source:** [konippi/skill-molt/examples/good-skill.md](https://github.com/konippi/skill-molt/blob/3e224ecb9b5e3b8789bef2a56490dbea7e831725/examples/good-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Good Skill Example

This is an example of a well-written skill extracted from a real session.

## The Skill

```markdown
---
name: e2e-testing
description: >-
  Use when running end-to-end tests, setting up test environments, or
  debugging test failures in this project. Handles Docker prerequisites,
  database seeding, and test isolation. Do NOT use for unit tests or
  component tests.
---

# E2E Testing

## Workflow

1. Verify Docker is running: `docker info > /dev/null 2>&1`
   - If Docker is not running → start it and wait 10 seconds
2. Start the test database: `docker compose up -d test-db`
3. Set the environment: `export DATABASE_URL=postgresql://test:test@localhost:5433/testdb`
4. Run migrations: `pnpm db:migrate`
5. Seed test data: `pnpm db:seed --env test`
6. Run tests: `pnpm test:e2e`
   - If tests hang for >60 seconds → Docker likely crashed. Run `docker compose logs test-db`
7. Tear down: `docker compose down -v`

## Rules

- Always use port 5433 for test DB (5432 is the dev DB)
- Never run e2e tests against the dev database — seed data will corrupt it
- The `--env test` flag on seed is required — without it, seed uses production fixtures

## Gotchas

- `pnpm test:e2e
```

</details>
