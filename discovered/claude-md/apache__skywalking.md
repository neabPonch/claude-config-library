---
name: apache__skywalking
source: https://github.com/apache/skywalking/blob/c94b4e00d35dfa543c10fa6bd282903a205f523f/CLAUDE.md
repo: apache/skywalking
kind: claude-md
stars: 24834
last_pushed: 2026-06-15T05:38:19Z
license: apache-2.0
score: 9
domains: [backend, java]
tags: [architecture, style-guide, java]
curated: 2026-06-15
curated_by: config-scout
---

# apache/skywalking — claude-md

**Why it's worth keeping:** It includes high-signal 'prohibited patterns' (like one-line delegate methods) and a unique naming philosophy that prioritizes concrete verbs over metaphors.

**Summary:** Provides deep architectural context for a custom Java SPI module system and strict, opinionated code style constraints.

**Source credibility:** Highly credible; Apache SkyWalking is a major, well-maintained open-source APM project with significant community adoption.

**Recency:** Current; the repository shows active maintenance and follows modern AI guidance patterns.

**Source:** [apache/skywalking/CLAUDE.md](https://github.com/apache/skywalking/blob/c94b4e00d35dfa543c10fa6bd282903a205f523f/CLAUDE.md) · 24834★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - AI Assistant Guide for Apache SkyWalking

This file provides guidance for AI assistants working with the Apache SkyWalking codebase.

## Project Overview

Apache SkyWalking is an open-source APM (Application Performance Monitoring) system designed for microservices, cloud-native, and container-based architectures. It provides distributed tracing, service mesh telemetry analysis, metrics aggregation, alerting, and observability capabilities.

## Repository Structure

```
skywalking/
├── oap-server/                    # OAP (Observability Analysis Platform) backend server
│   ├── server-core/               # Core module with fundamental services
│   ├── server-library/            # Shared libraries (module system, util, etc.)
│   ├── server-receiver-plugin/    # Data receivers (gRPC, HTTP, Kafka, etc.)
│   ├── server-storage-plugin/     # Storage implementations (BanyanDB, Elasticsearch, etc.)
│   ├── server-cluster-plugin/     # Cluster coordination (Zookeeper, K8s, etc.)
│   ├── server-query-plugin/       # Query interfaces (GraphQL)
│   ├── server-alarm-plugin/       # Alerting system
│   ├── server-fetcher-plugin/     # Data fetchers
│   ├── server-configuration/
```

</details>
