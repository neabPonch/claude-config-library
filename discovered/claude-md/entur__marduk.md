---
name: entur__marduk
source: https://github.com/entur/marduk/blob/7c646177a62c111b49fb31fe475c8c091afdfbf2/CLAUDE.MD
repo: entur/marduk
kind: claude-md
stars: 4
last_pushed: 2026-06-12T21:10:55Z
license: eupl-1.2
score: 9
domains: [backend-orchestration, data-pipeline, java-spring]
tags: [apache-camel, spring-boot, event-driven, etl]
curated: 2026-06-15
curated_by: config-scout
---

# entur/marduk — claude-md

**Why it's worth keeping:** Includes concrete 'Common Development Tasks' with code examples and maps out a complex multi-step data pipeline logic essential for maintaining system consistency.

**Summary:** Provides deep architectural context for an Apache Camel orchestration engine, including specific business workflows and extension patterns.

**Source credibility:** High; maintained by Entur, a legitimate Norwegian public transport entity.

**Recency:** Very current, utilizing Java 21 and Spring Boot 3.

**Source:** [entur/marduk/CLAUDE.MD](https://github.com/entur/marduk/blob/7c646177a62c111b49fb31fe475c8c091afdfbf2/CLAUDE.MD) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Marduk - AI Assistant Guide

## Project Overview

Marduk is a Spring Boot application that orchestrates the timetable data import pipeline for Entur (Norwegian public transport). It manages the entire workflow from receiving timetable data files through validation, import, transformation, and publication to updating journey planner graphs.

### Core Purpose
- **Primary Role**: Backend integration orchestrator for public transport timetable data
- **Data Formats**: NeTEx (primary), GTFS (legacy, being migrated)
- **Architecture Pattern**: Event-driven, message-based orchestration using Apache Camel

## Technology Stack

- **Language**: Java 21
- **Framework**: Spring Boot 3.x with Apache Camel 4.4.5
- **Build Tool**: Maven
- **Database**: PostgreSQL (with Flyway migrations)
- **Messaging**: Google Cloud PubSub
- **Storage**: Google Cloud Storage (GCS)
- **REST**: Jersey (JAX-RS)
- **Deployment**: Kubernetes (Helm charts in `helm/`)

## Project Structure

```
src/main/java/no/rutebanken/marduk/
├── App.java                    # Main Spring Boot application, extends RouteBuilder
├── Constants.java              # Application-wide constants (headers, paths, file names)
├── Utils.java
```

</details>
