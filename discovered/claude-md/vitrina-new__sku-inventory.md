---
name: vitrina-new__sku-inventory
source: https://github.com/vitrina-new/sku-inventory/blob/6a26fdd4d66f9b09e22d3191ecc929f41cfb3a43/claude.md
repo: vitrina-new/sku-inventory
kind: claude-md
stars: 0
last_pushed: 2025-12-19T15:50:31Z
license: unknown
score: 8
domains: [backend-api, java-spring]
tags: [rest-api, domain-driven-design, sku-management]
curated: 2026-06-16
curated_by: config-scout
---

# vitrina-new/sku-inventory — claude-md

**Why it's worth keeping:** Includes critical business-logic patterns like the SKU generation algorithm and exact dependency versions to prevent AI hallucinations.

**Summary:** A highly structured project specification providing deep domain knowledge and strict technical constraints.

**Source credibility:** Professional architecture but lacks social proof (0 stars).

**Recency:** 

**Source:** [vitrina-new/sku-inventory/claude.md](https://github.com/vitrina-new/sku-inventory/blob/6a26fdd4d66f9b09e22d3191ecc929f41cfb3a43/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SKU Management API Service

A cloud-native RESTful API service for creating and managing Stock Keeping Units (SKUs) for retail operations. Built with Java 20+, Spring Boot 3.x, containerized with Docker, and instrumented with OpenTelemetry.

## Technology Stack

| Component | Technology | Version |
|-----------|------------|---------|
| Language | Java | 20+ (prefer 21 LTS) |
| Framework | Spring Boot | 3.2+ |
| Build Tool | Gradle (Kotlin DSL) | 8.5+ |
| Container | Docker | Multi-stage build |
| Observability | OpenTelemetry | 1.30+ |
| API Docs | SpringDoc OpenAPI | 2.3+ |
| Database | PostgreSQL | 15+ |
| Testing | JUnit 5, Testcontainers | Latest |

## Project Structure

```
sku-service/
├── build.gradle.kts
├── settings.gradle.kts
├── Dockerfile
├── docker-compose.yml
├── src/
│   ├── main/
│   │   ├── java/com/retailer/sku/
│   │   │   ├── SkuServiceApplication.java
│   │   │   ├── config/
│   │   │   │   ├── OpenApiConfig.java
│   │   │   │   └── OpenTelemetryConfig.java
│   │   │   ├── controller/
│   │   │   │   └── SkuController.java
│   │   │   ├── service/
│   │   │   │   ├── SkuService.java
│   │   │   │   └── SkuServiceImpl.java
│   │   │   ├── repository/
│   │
```

</details>
