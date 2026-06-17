---
name: ducpm2303__claude-java-plugins__claude
source: https://github.com/ducpm2303/claude-java-plugins/blob/006a789364c3350c0e691f1f1e8c4fe5859cdcab/plugins/java-spring/CLAUDE.md
repo: ducpm2303/claude-java-plugins
kind: claude-md
stars: 15
last_pushed: 2026-04-06T07:43:23Z
license: unknown
score: 8
domains: [backend-api, java]
tags: [spring-boot, java, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# ducpm2303/claude-java-plugins — claude-md

**Why it's worth keeping:** Includes high-value technical nuances like avoiding @Transactional proxy bypasses and enforcing constructor injection over field injection.

**Summary:** Enforces strict architectural standards for Spring Boot development, focusing on dependency injection, layered architecture, and transaction management.

**Source credibility:** Low star count (15), but the highly specific technical constraints suggest a professional-grade toolkit.

**Recency:** Very recent; last updated 2 months ago.

**Source:** [ducpm2303/claude-java-plugins/plugins/java-spring/CLAUDE.md](https://github.com/ducpm2303/claude-java-plugins/blob/006a789364c3350c0e691f1f1e8c4fe5859cdcab/plugins/java-spring/CLAUDE.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
globs: ["**/*.java", "**/pom.xml", "**/build.gradle", "**/build.gradle.kts", "**/application.yml", "**/application.properties"]
---

# Java Spring — Spring Boot Best Practices

These rules apply whenever the java-spring plugin is active.

## Dependency Injection
- Always use **constructor injection**. Never use field injection (`@Autowired` on a field).
- Mark constructor-injected fields as `final`.
- For optional dependencies, use setter injection with `@Autowired(required = false)`.

## Layered Architecture
Enforce the Controller → Service → Repository flow:
- `@RestController` classes call `@Service` classes only — never repositories directly
- `@Service` classes call `@Repository` interfaces only — never other controllers
- Domain/entity classes have no Spring annotations

## Transactions
- Place `@Transactional` on `@Service` methods, never on `@RestController` methods
- Use `@Transactional(readOnly = true)` for read-only service methods (performance benefit)
- Avoid calling `@Transactional` methods from within the same class (proxy bypass)

## Configuration
- All configuration values come from `application.yml` or `application.properties`
- Inject config values with `@Val
```

</details>
