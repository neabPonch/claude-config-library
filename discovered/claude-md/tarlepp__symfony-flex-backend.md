---
name: tarlepp__symfony-flex-backend
source: https://github.com/tarlepp/symfony-flex-backend/blob/d187582d1c0302d5f210ebbb9b7d1a878281b457/CLAUDE.md
repo: tarlepp/symfony-flex-backend
kind: claude-md
stars: 291
last_pushed: 2026-06-15T05:42:25Z
license: mit
score: 9
domains: [backend-api, php]
tags: [symfony, rest-api, docker, test-driven-development]
curated: 2026-06-15
curated_by: config-scout
---

# tarlepp/symfony-flex-backend — claude-md

**Why it's worth keeping:** The 'Development Workflow' section gives the AI a deterministic step-by-step algorithm for creating new features, while the command catalog eliminates guesswork for testing and quality checks.

**Summary:** A high-quality blueprint that defines a strict resource-based architecture and provides an exhaustive list of automation commands via Makefile.

**Source credibility:** Highly credible; a well-starred (291) community template with very recent updates.

**Recency:** Extremely current, utilizing PHP 8.4 and Symfony 7.4 standards.

**Source:** [tarlepp/symfony-flex-backend/CLAUDE.md](https://github.com/tarlepp/symfony-flex-backend/blob/d187582d1c0302d5f210ebbb9b7d1a878281b457/CLAUDE.md) · 291★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# General Guidelines for Interacting with Claude

- This is a Symfony JSON REST API backend template with Docker setup for local
  development.
- Check the README.md for detailed installation and usage instructions.
- Use `make` commands to manage Docker containers and application tasks.
- For frontend integration, refer to the "Frontend?" section in the README.md.
- For additional resources and links, see the "Resources" and "External links
  / resources" sections.

# Project Architecture

- **Type:** JSON REST API Backend
- **Pattern:** Resource-based REST architecture with service layer
- **Authentication:**
  - JWT (Lexik JWT Bundle)
  - API key authentication
- **ORM:** Doctrine ORM with migrations
  - Migrations located in `migrations/`
  - Entities in `src/Entity/`
  - Repositories in `src/Repository/`
  - MariaDB database
- **Key Layers:**
  - Controller Layer: `src/Controller/` and `src/Rest/`
  - Service Layer: `src/Service/` and `src/Resource/`
  - Repository Layer: `src/Repository/`
  - Entity Layer: `src/Entity/`
  - DTO Layer: `src/DTO/`
  - Security Layer: `src/Security/`
  - AutoMapper: `src/AutoMapper/`
  - Value Resolvers: `src/ValueResolver/`
  - Decorators: `src
```

</details>
