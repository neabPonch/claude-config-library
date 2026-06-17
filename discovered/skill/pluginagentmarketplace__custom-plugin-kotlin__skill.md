---
name: pluginagentmarketplace__custom-plugin-kotlin__skill
source: https://github.com/pluginagentmarketplace/custom-plugin-kotlin/blob/cc703d88715618fef4d7196f3bb68b86a9717873/skills/kotlin-ktor/SKILL.md
repo: pluginagentmarketplace/custom-plugin-kotlin
kind: skill
stars: 7
last_pushed: 2026-01-05T11:55:42Z
license: other
score: 7
domains: [backend-api, kotlin]
tags: [ktor, kotlin, routing, authentication]
curated: 2026-06-16
curated_by: config-scout
---

# pluginagentmarketplace/custom-plugin-kotlin — skill

**Why it's worth keeping:** The inclusion of a Troubleshooting table provides the agent with expert-level logic to resolve common framework errors. The 'Topic' parameterization allows for highly targeted knowledge retrieval.

**Summary:** A structured skill definition for Ktor development covering routing, JWT authentication, and unit testing.

**Source credibility:** Low-profile repository (7 stars) likely serving as a specialized plugin marketplace.

**Recency:** Current; uses modern Ktor patterns and up-to-date versioning.

**Source:** [pluginagentmarketplace/custom-plugin-kotlin/skills/kotlin-ktor/SKILL.md](https://github.com/pluginagentmarketplace/custom-plugin-kotlin/blob/cc703d88715618fef4d7196f3bb68b86a9717873/skills/kotlin-ktor/SKILL.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kotlin-ktor
description: Ktor framework - routing, authentication, WebSockets
version: "1.0.0"
sasmp_version: "1.3.0"
bonded_agent: 05-kotlin-backend
bond_type: PRIMARY_BOND

execution:
  timeout_ms: 30000
  retry:
    max_attempts: 3
    backoff: exponential
    initial_delay_ms: 1000

parameters:
  required:
    - name: topic
      type: string
      validation: "^(routing|plugins|auth|websocket|testing)$"
  optional:
    - name: ktor_version
      type: string
      default: "2.3.8"

logging:
  level: info
  events: [skill_invoked, topic_loaded, error_occurred]
---

# Kotlin Ktor Skill

Build production-ready backends with Ktor.

## Topics Covered

### Routing
```kotlin
fun Application.module() {
    install(ContentNegotiation) { json() }
    routing {
        route("/api/v1") {
            get("/users") { call.respond(userService.findAll()) }
            get("/users/{id}") {
                val id = call.parameters["id"]?.toLongOrNull()
                    ?: throw BadRequestException("Invalid ID")
                call.respond(userService.findById(id) ?: throw NotFoundException())
            }
        }
    }
}
```

### JWT Authentication
```kotlin
install(Authentica
```

</details>
