---
name: entur__damu
source: https://github.com/entur/damu/blob/6a189ae8b5e779c60fb373a4e094554fb4cc8af4/CLAUDE.MD
repo: entur/damu
kind: claude-md
stars: 2
last_pushed: 2026-06-02T20:07:22Z
license: eupl-1.2
score: 8
domains: [backend-java, data-pipeline]
tags: [spring-boot, apache-camel, maven, integration-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# entur/damu — claude-md

**Why it's worth keeping:** The 'Working with Claude' section is excellent; it defines patterns for common tasks and proactively lists operational gotchas like memory requirements and strict formatting rules.

**Summary:** Provides high-level architecture, build/test workflows, and specific guidance for AI agents on how to modify core components like Camel routes.

**Source credibility:** High: maintained by Entur, a professional organization in the public transport sector.

**Recency:** Current: uses modern tech stack including Java 21 and Spring Boot/Camel 4.

**Source:** [entur/damu/CLAUDE.MD](https://github.com/entur/damu/blob/6a189ae8b5e779c60fb373a4e094554fb4cc8af4/CLAUDE.MD) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Damu - NeTEx to GTFS Converter

## Project Overview

Damu is a Spring Boot application that converts NeTEx (Network Timetable Exchange) datasets into GTFS (General Transit Feed Specification) datasets. It serves as a critical integration component in the Entur public transport data pipeline, handling conversion, validation, and aggregation of transit data.

## Architecture

### Technology Stack
- **Java 21** - Core language
- **Spring Boot** - Application framework
- **Apache Camel 4.8.9** - Integration framework and routing
- **Google Cloud Platform**:
  - Cloud Storage (GCS) - File storage
  - Pub/Sub - Messaging
- **Maven** - Build tool

### Key Dependencies
- `netex-gtfs-converter-java` (v2.1.105) - Core NeTEx to GTFS conversion
- `gtfs-validator-main` (v6.0.0) - GTFS validation
- `entur-helpers` (v5.47.0) - Google Cloud integration utilities
- `zt-zip` (v1.17) - ZIP file handling

### Integration Flow
1. **Trigger**: Chouette or Uttu completes a NeTEx export
2. **Notification**: Marduk notifies Damu via Google Pub/Sub
3. **Download**: Damu downloads NeTEx dataset from GCS
4. **Convert**: NeTEx is converted to GTFS
5. **Validate**: GTFS is validated using MobilityData validat
```

</details>
