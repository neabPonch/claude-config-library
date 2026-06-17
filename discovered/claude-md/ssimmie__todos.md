---
name: ssimmie__todos
source: https://github.com/ssimmie/todos/blob/d3d04882cf841ba4fec8f1bc2112f6844e25166f/CLAUDE.md
repo: ssimmie/todos
kind: claude-md
stars: 16
last_pushed: 2026-05-14T07:21:53Z
license: mit
score: 8
domains: [backend-api, java]
tags: [build-status, environment-config, maven]
curated: 2026-06-16
curated_by: config-scout
---

# ssimmie/todos — claude-md

**Why it's worth keeping:** Includes exact environment variable exports to suppress JVM warnings and precise 'current state' metrics that prevent the agent from wasting time on known non-blocking issues.

**Summary:** Provides a highly detailed technical status of the project's build ecosystem, including module-specific health and known linting issues.

**Source credibility:** Moderate; a small, actively maintained microservice repo (16 stars).

**Recency:** Very recent; reflects modern Spring Boot 3/Java 17 standards.

**Source:** [ssimmie/todos/CLAUDE.md](https://github.com/ssimmie/todos/blob/d3d04882cf841ba4fec8f1bc2112f6844e25166f/CLAUDE.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Development Notes

## Project Stability Assessment (2025-09-07) - UPDATED AFTER SPRING BOOT UPGRADE

### ✅ **UPGRADED AND STABLE - SPRING BOOT 3.2.12 + JAVA 17**

The project has been successfully upgraded to Spring Boot 3.2.12 with Java 17, resolving the ProcessorMetrics container issues.

### Build Status by Module

#### 🟢 **domain** - STABLE  
- **Compilation**: ✅ SUCCESS (5.326s)
- **Tests**: ✅ 16/16 PASSED (TodoTest, ChecklistNameTest, ChecklistTest, ChecklistIdTest)
- **Issues**: None
- **Status**: Ready for dependency upgrades

#### 🟡 **application** - STABLE WITH MINOR ISSUES
- **Compilation**: ✅ SUCCESS (24.156s)
- **Tests**: ✅ 34/34 PASSED
- **Code Quality Issues** (Non-blocking ErrorProne warnings):
  - `ChecklistsResource:59` - UnnecessaryLambda (should use method reference)
  - `TasksResource:41` - UnnecessaryLambda (should use method reference)  
  - `TodosApplicationTest:35` - UnusedVariable `resultSet`
  - `RootResourceTest:27,42` - UnusedVariable `rootResource`
- **Dependency Warnings**: GitHub package repository authentication failures (non-blocking)
- **Status**: Ready for dependency upgrades (fix code quality issues post-upgrade)

#### 🟢 **acceptance-tests** -
```

</details>
