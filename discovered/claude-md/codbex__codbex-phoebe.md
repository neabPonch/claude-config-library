---
name: codbex__codbex-phoebe
source: https://github.com/codbex/codbex-phoebe/blob/aee49a7195e4607433788b2e43da037405457d86/CLAUDE.md
repo: codbex/codbex-phoebe
kind: claude-md
stars: 0
last_pushed: 2026-06-12T12:09:33Z
license: epl-2.0
score: 9
domains: [backend, java, devops]
tags: [maven, spring-boot, architecture-mapping, build-instructions]
curated: 2026-06-16
curated_by: config-scout
---

# codbex/codbex-phoebe — claude-md

**Why it's worth keeping:** It includes specific 'gotcha' instructions (e.g., updating HTML when changing proxy paths) and maps high-level architecture directly to specific code locations/classes.

**Summary:** This file provides deep architectural context, specific Maven build profiles, and critical maintenance warnings for a complex Spring Boot/Airflow integration.

**Source credibility:** Low social proof via stars, but the technical depth suggests a professional enterprise-grade codebase.

**Recency:** Highly current, referencing Java 21 and modern Spring Cloud Gateway configurations.

**Source:** [codbex/codbex-phoebe/CLAUDE.md](https://github.com/codbex/codbex-phoebe/blob/aee49a7195e4607433788b2e43da037405457d86/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Phoebe is **the data-centric workflow platform based on Apache Airflow**
([product page](https://www.codbex.com/products/)) — a customizable Web IDE for Apache
Airflow workflow development built on the **codbex platform / Eclipse Dirigible** (via the
`com.codbex.platform:codbex-platform-parent` parent POM). It is a Spring Boot application: at
runtime the Java app and an Apache Airflow instance run side by side (in the same Docker
container in production), and Phoebe embeds Airflow's web UI by reverse-proxying to it.

## Build & test commands

Build profiles (`quick-build`, `unit-tests`, `integration-tests`, `tests`, `format`) are
**inherited from the parent platform POM**, not defined in this repo.

```shell
mvn -T 1C clean install -P quick-build   # build the executable jar (skips tests/checks)
mvn clean install -P unit-tests          # unit tests
mvn clean install -P integration-tests   # integration tests (Selenium-based UI tests)
mvn clean install -P tests               # all tests
mvn verify -P format                     # format the code (run b
```

</details>
