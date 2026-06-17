---
name: w8fyz__Fiber__fiber-skill
source: https://github.com/w8fyz/Fiber/blob/b79f1e89355d9fb7a388ba00508796f470ac4c68/FIBER-SKILL.md
repo: w8fyz/Fiber
kind: skill
stars: 2
last_pushed: 2026-05-07T22:29:09Z
license: unknown
score: 8
domains: [backend-api, security]
tags: [java, framework-map, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# w8fyz/Fiber — skill

**Why it's worth keeping:** The granular mapping of package structures to class responsibilities allows an AI agent to understand complex cross-cutting concerns like OAuth2 and session management without needing to parse every file manually.

**Summary:** Provides a comprehensive architectural map of the Fiber Java web framework, detailing its annotation-driven routing, security protocols, and service hierarchies.

**Source credibility:** Niche project with high documentation density suggesting a well-structured codebase.

**Recency:** Very current, leveraging modern Java 21+ features.

**Source:** [w8fyz/Fiber/FIBER-SKILL.md](https://github.com/w8fyz/Fiber/blob/b79f1e89355d9fb7a388ba00508796f470ac4c68/FIBER-SKILL.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: fiber-framework
description: >-
  Work with the Fiber Java web framework: create controllers, endpoints, authentication,
  sessions, validation, security, middleware, file uploads, and email. Use when the user
  works with FiberServer, @Controller, @RequestMapping, ResponseEntity, AuthenticationService,
  SessionService, or any sh.fyz.fiber class.
---

# Fiber Framework

Fiber is a Java 21+ RESTful API framework built on Jetty 11 with annotation-driven routing, built-in JWT authentication, OAuth2, server-side sessions, CORS, CSRF, rate limiting, validation, file uploads, and email templating.

## Project Structure

```
src/main/java/sh/fyz/fiber/
├── FiberServer.java                            # Entry point, server lifecycle, service registry
├── annotations/
│   ├── auth/
│   │   ├── IdentifierField.java                # Marks login identifier fields on user entity
│   │   └── PasswordField.java                  # Marks BCrypt password field on user entity
│   ├── dto/
│   │   └── IgnoreDTO.java                      # Exclude field from DTO serialization
│   ├── params/
│   │   ├── AuthenticatedUser.java              # Inject current authenticated user
│   │   ├── Curren
```

</details>
