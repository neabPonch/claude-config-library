---
name: aphp__Cohort360-QueryExecutor
source: https://github.com/aphp/Cohort360-QueryExecutor/blob/e7ba4ac76e350babdd0210cae79d0b6d0bb40d38/CLAUDE.md
repo: aphp/Cohort360-QueryExecutor
kind: claude-md
stars: 2
last_pushed: 2026-06-04T12:49:39Z
license: mpl-2.0
score: 8
domains: [backend, data-engineering]
tags: [scala, spark, fhir]
curated: 2026-06-16
curated_by: config-scout
---

# aphp/Cohort360-QueryExecutor — claude-md

**Why it's worth keeping:** Maps functional responsibility to specific directory structures and provides essential JVM module-access flags required for Spark stability that are often overlooked.

**Summary:** High-density architectural breakdown and specialized runtime command instructions for a Scala/Spark engine.

**Source credibility:** Low star count but highly specialized domain content suggests a professional-grade engineering tool.

**Recency:** Very current; uses modern Spark 3.4 and Scala versions.

**Source:** [aphp/Cohort360-QueryExecutor/CLAUDE.md](https://github.com/aphp/Cohort360-QueryExecutor/blob/e7ba4ac76e350babdd0210cae79d0b6d0bb40d38/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the Cohort Requester (Spark Job Server) - a Scala/Spark application that executes FHIR queries to identify patient cohorts. It serves as the query execution engine for the Cohort360 project, processing complex medical data queries with temporal constraints and returning patient counts or cohort lists.

## Build and Development Commands

### Build
```bash
# Clean and build the project
mvn clean package

# Build without tests
mvn clean compile

# Build with Maven wrapper
./mvnw clean package
```

### Testing
```bash
# Run tests
mvn test

# Run tests with Maven wrapper  
./mvnw test

# Clean and run full verification (includes tests)
mvn clean verify
./mvnw clean verify
```

### Run Application
```bash
# Build and run locally
mvn clean package
java \
  --add-opens=java.base/java.lang=ALL-UNNAMED \
  --add-opens=java.base/java.lang.invoke=ALL-UNNAMED \
  --add-opens=java.base/java.lang.reflect=ALL-UNNAMED \
  --add-opens=java.base/java.io=ALL-UNNAMED \
  --add-opens=java.base/java.net=ALL-UNNAMED \
  --add-opens=java.base/java.nio=ALL-UNNAMED
```

</details>
