---
name: thehomelessguy__MARSLib__skill
source: https://github.com/thehomelessguy/MARSLib/blob/2a3e024cfb75eec50a097c4d23b9cfc1fab10417/.agents/skills/marslib-ci/SKILL.md
repo: thehomelessguy/MARSLib
kind: skill
stars: 0
last_pushed: 2026-06-04T00:33:12Z
license: mit
score: 8
domains: [devops, build-systems]
tags: [gradle, ci-cd, automation]
curated: 2026-06-15
curated_by: config-scout
---

# thehomelessguy/MARSLib — skill

**Why it's worth keeping:** It utilizes a 'Key Rules' pattern to mandate specific developer workflows (like auto-formatting) and provides actionable troubleshooting steps for common errors.

**Summary:** A highly structured DevOps skill that enforces strict build, linting, and testing protocols using Gradle.

**Source credibility:** Low public visibility; appears to be a specialized internal team resource from an FRC robotics project.

**Recency:** Current; demonstrates excellent patterns for modern agentic tool-use and workflow enforcement.

**Source:** [thehomelessguy/MARSLib/.agents/skills/marslib-ci/SKILL.md](https://github.com/thehomelessguy/MARSLib/blob/2a3e024cfb75eec50a097c4d23b9cfc1fab10417/.agents/skills/marslib-ci/SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: marslib-ci
description: Helps understand build automations, Gradle tasks, Spotless linting formatting, and deployment workflows. Use when fixing build errors, running tests, or configuring CI pipelines.
---

# MARSLib Continuous Integration Skill

You are the DevOps lead for Team MARS 2614. When working with builds, formatting, or deployment:

## 1. Architecture

MARSLib uses Gradle with WPILib plugins for compilation, testing, and deployment:

| Tool | Purpose |
|---|---|
| `gradlew build` | Full compile + test suite |
| `gradlew test` | Run JUnit 5 test suite only |
| `gradlew spotlessApply` | Auto-format all Java files to Google Java Format |
| `gradlew spotlessCheck` | Verify formatting without modifying (used in CI) |
| `gradlew deploy` | Deploy to roboRIO via USB/WiFi |
| `gradlew javadoc` | Generate Javadoc, catches broken `{@link}` tags |

### CI Pipeline (`ci.yml`)
GitHub Actions runs on every push/PR to `main`:
1. `spotlessCheck` — Reject PRs with formatting violations
2. `build` — Compile all source
3. `test` — Run full 79-test physics suite
4. `javadoc` — Catch doc errors before GH-Pages deployment

## 2. Key Rules

### Rule A: Always Run spotlessApply Before
```

</details>
