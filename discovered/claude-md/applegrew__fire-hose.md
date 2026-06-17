---
name: applegrew__fire-hose
source: https://github.com/applegrew/fire-hose/blob/e0aee9153648e51658ee2cea045cc1c1367386f6/CLAUDE.MD
repo: applegrew/fire-hose
kind: claude-md
stars: 0
last_pushed: 2026-01-26T19:19:47Z
license: unknown
score: 9
domains: [backend, infrastructure, data-engineering]
tags: [kafka, kubernetes, streaming, quarkus]
curated: 2026-06-15
curated_by: config-scout
---

# applegrew/fire-hose — claude-md

**Why it's worth keeping:** Includes critical 'low-level' context like exact port-forwarding commands, infrastructure setup scripts, and explicit cross-service data flow logic that allows an AI to debug complex orchestration issues.

**Summary:** A highly detailed operational guide for a complex distributed streaming architecture involving Kafka, Flink, and Kubernetes.

**Source credibility:** High-quality technical documentation suggesting a professional-grade or serious engineering project despite low star count.

**Recency:** Very current; utilizes modern stack versions like Quarkus 3.x and Kafka 4.1.1.

**Source:** [applegrew/fire-hose/CLAUDE.MD](https://github.com/applegrew/fire-hose/blob/e0aee9153648e51658ee2cea045cc1c1367386f6/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FireHose: Project Sentinel

## Project Overview
FireHose is a **Generic Real-time Alerting Engine** designed for high-velocity event ingestion and dynamic rule evaluation. It enables proactive monitoring by matching a live event firehose against broadcasted user rules without requiring code redeploys.

![FireHose System Design](./FireHose.jpg)

## Tech Stack
- **Container Runtime:** Colima (open-source Docker Desktop alternative)
- **Streaming Bus:** Apache Kafka 4.1.1 (Strimzi Operator, KRaft mode)
- **Processing Engine:** Apache Flink (Stateful Stream Processing)
- **Orchestration:** Kubernetes (Minikube with Flink Kubernetes Operator)
- **API Gateway:** Kong (local) / AWS API Gateway (production)
- **Logic:** Broadcast State Pattern for dynamic rule evaluation
- **Event Ingester:** Quarkus 3.x microservice (Gradle, SmallRye Reactive Messaging)
- **Query Service:** Quarkus 3.x microservice (Hibernate ORM Panache, PostgreSQL, Redis caching)

## Quick Start
```bash
# Full infrastructure setup (idempotent, safe to re-run)
./development/setup.sh

# Run infrastructure tests only
./development/setup.sh --test

# Build and deploy application services
./development/start.sh

# Deploy s
```

</details>
