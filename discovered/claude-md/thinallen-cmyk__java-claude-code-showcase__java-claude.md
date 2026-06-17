---
name: thinallen-cmyk__java-claude-code-showcase__java-claude
source: https://github.com/thinallen-cmyk/java-claude-code-showcase/blob/86045bd9f6b31c3eac9c54aa7dc45448d19cadfd/JAVA_CLAUDE.md
repo: thinallen-cmyk/java-claude-code-showcase
kind: claude-md
stars: 1
last_pushed: 2026-01-10T11:04:01Z
license: unknown
score: 8
domains: [backend-api, web-frontend, fullstack]
tags: [java, springboot, vuejs, maven, npm]
curated: 2026-06-15
curated_by: config-scout
---

# thinallen-cmyk/java-claude-code-showcase — claude-md

**Why it's worth keeping:** Provides essential CLI command mappings (test/lint/build) and explicit 'Critical Rules' that guide the AI away from common anti-patterns like silent exception handling or SQL injection.

**Summary:** A comprehensive full-stack configuration for a Java Spring Boot and Vue.js application.

**Source credibility:** Low signal; repository is sparse with minimal social proof.

**Recency:** Current; uses modern stacks like Java 17+ and Vue 3 Composition API.

**Source:** [thinallen-cmyk/java-claude-code-showcase/JAVA_CLAUDE.md](https://github.com/thinallen-cmyk/java-claude-code-showcase/blob/86045bd9f6b31c3eac9c54aa7dc45448d19cadfd/JAVA_CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Java Spring Boot + Vue.js Project

> This is an example CLAUDE.md file showing how to configure Claude Code for a Java/Spring Boot/Maven/Vue/PostgreSQL project.

## Quick Facts

- **Stack**: Java 17+, Spring Boot 3.x, Maven, Vue 3, PostgreSQL
- **Backend Test Command**: `mvn test`
- **Frontend Test Command**: `npm run test`
- **Backend Lint Command**: `mvn checkstyle:check`
- **Frontend Lint Command**: `npm run lint`
- **Build Command**: `mvn clean install`

## Key Directories

- `backend/src/main/java/com/company/project/` - Spring Boot controllers, services, repositories
- `backend/src/test/java/com/company/project/` - Backend tests
- `frontend/src/components/` - Vue components
- `frontend/src/views/` - Vue views/pages
- `frontend/src/services/` - API client services
- `frontend/src/composables/` - Vue composables
- `backend/src/main/resources/` - Configuration, SQL migrations, static assets
- `docker/` - Docker configurations
- `sql/` - Database migration scripts (Flyway/Liquibase)
- `tests/e2e/` - End-to-end tests

## Code Style

### Java
- Follow Spring Boot conventions and Java 17+ features
- Use Spring annotations appropriately (`@Service`, `@Controller`, `@Repository`, et
```

</details>
