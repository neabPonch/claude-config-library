---
name: opensabre__opensabre-framework
source: https://github.com/opensabre/opensabre-framework/blob/435555b6fc33c5b7e1eb177253ee5167d56562b9/CLAUDE.md
repo: opensabre/opensabre-framework
kind: claude-md
stars: 397
last_pushed: 2026-06-07T09:08:07Z
license: apache-2.0
score: 8
domains: [backend-api, microservices, java]
tags: [spring-boot, architectural-patterns, maven]
curated: 2026-06-15
curated_by: config-scout
---

# opensabre/opensabre-framework — claude-md

**Why it's worth keeping:** The 'Key Architectural Patterns' section is exceptional; it defines specific data shapes (Result<T>, BasePo/Vo) that prevent an LLM from generating non-compliant boilerplate.

**Summary:** Provides detailed architectural patterns, module structures, and coding standards for a complex Spring Cloud microservices ecosystem.

**Source credibility:** High; a well-starred, actively maintained enterprise microservices framework.

**Recency:** Very current; utilizes Spring Boot 3.4.1 and modern Java standards.

**Source:** [opensabre/opensabre-framework/CLAUDE.md](https://github.com/opensabre/opensabre-framework/blob/435555b6fc33c5b7e1eb177253ee5167d56562b9/CLAUDE.md) · 397★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Opensabre is a microservices development platform based on Spring Cloud 2023, integrating Spring Security, Spring Cloud Alibaba, and other components. It provides foundational RBAC permission management, authorization authentication, gateway management, service governance, audit logging, and other system management applications.

## Build and Development Commands

### Building the Project
```bash
# Build all modules
mvn clean install

# Build with tests
mvn clean install -DskipTests=false

# Skip tests for faster builds
mvn clean install -DskipTests=true

# Deploy to Maven Central (requires deploy profile)
mvn clean deploy -Pdeploy
```

### Testing
```bash
# Run all tests
mvn test

# Run tests for specific module
cd opensabre-web && mvn test

# Run single test class
mvn test -Dtest=UserContextHolderTest
```

### Code Quality
```bash
# Generate JavaDoc
mvn javadoc:javadoc

# Generate flattened POM (for deployment)
mvn flatten:flatten
```

## Architecture and Module Structure

### Core Modules

- **opensabre-base-dependencies**: Central dependency
```

</details>
