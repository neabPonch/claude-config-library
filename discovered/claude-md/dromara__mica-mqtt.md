---
name: dromara__mica-mqtt
source: https://github.com/dromara/mica-mqtt/blob/84dd011ad4cab4720332bd76828e47dc01ac5d98/CLAUDE.md
repo: dromara/mica-mqtt
kind: claude-md
stars: 481
last_pushed: 2026-06-16T01:07:20Z
license: apache-2.0
score: 9
domains: [backend, java, iot, networking]
tags: [architecture-mapping, maven-commands, coding-standards, protocol-specs]
curated: 2026-06-16
curated_by: config-scout
---

# dromara/mica-mqtt — claude-md

**Why it's worth keeping:** Includes critical 'negative' constraints (e.g., NO Lombok), explicit dependency flow mapping to prevent architectural rot, and essential thread-safety warnings specific to the underlying async framework.

**Summary:** A comprehensive technical manual that bridges high-level project goals with low-level implementation constraints for a Java MQTT library.

**Source credibility:** High; comes from a well-maintained, starred Java project with professional documentation structure.

**Recency:** Current; includes modern context like GraalVM support and up-to-date Maven profiles.

**Source:** [dromara/mica-mqtt/CLAUDE.md](https://github.com/dromara/mica-mqtt/blob/84dd011ad4cab4720332bd76828e47dc01ac5d98/CLAUDE.md) · 481★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**mica-mqtt** is a high-performance, low-latency MQTT IoT component for Java 8+, maintained by the Dromara organization. It provides both client and server (broker) implementations supporting MQTT v3.1, v3.1.1, and v5.0 protocols.

**Key Features:**
- Lightweight core (only 500KB)
- Built on t-io async networking framework
- WebSocket MQTT sub-protocol support (compatible with mqtt.js)
- HTTP REST API for server management
- Shared subscriptions and queue subscriptions
- Client/Server support for Spring Boot, Solon, and JFinal
- GraalVM native compilation support
- **Clustering via `mica-mqtt-broker` module** (t-io cluster for node-to-node communication)

**Documentation:** https://mica-mqtt.dreamlu.net/guide/
**Demo Server:** mqtt.dreamlu.net (username: mica, password: mica)

## Common Commands

### Build & Test
```bash
# Full build with tests (includes example module via develop profile)
mvn clean install

# Build without tests
mvn package -DskipTests

# Run all tests
mvn test

# Run specific test class
mvn -Dtest=TopicFilterTypeTest test

# Ru
```

</details>
