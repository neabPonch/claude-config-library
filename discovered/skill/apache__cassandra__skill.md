---
name: apache__cassandra__skill
source: https://github.com/apache/cassandra/blob/308adc4f8235438c1980c295ae59a827979da11a/.claude/skills/cassandra-injvm-dtest/SKILL.md
repo: apache/cassandra
kind: skill
stars: 9776
last_pushed: 2026-06-14T14:53:02Z
license: apache-2.0
score: 9
domains: [distributed-systems, java, testing]
tags: [cassandra, integration-testing, in-jvm, distributed-databases]
curated: 2026-06-15
curated_by: config-scout
---

# apache/cassandra — skill

**Why it's worth keeping:** The file offers specific, copy-pasteable code patterns for varying cluster complexities (multi-DC, feature-based) and an exhaustive list of valid configuration keys to prevent hallucination.

**Summary:** Provides highly structured setup patterns and configuration parameters for writing in-JVM distributed tests in Apache Cassandra.

**Source credibility:** Extremely high; part of the official Apache Cassandra repository with massive community trust.

**Recency:** Current; includes very recent features like Accord/CEP-15 configuration.

**Source:** [apache/cassandra/.claude/skills/cassandra-injvm-dtest/SKILL.md](https://github.com/apache/cassandra/blob/308adc4f8235438c1980c295ae59a827979da11a/.claude/skills/cassandra-injvm-dtest/SKILL.md) · 9776★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cassandra-injvm-dtest
version: "1.0.0"
description: Comprehensive guide for writing Apache Cassandra in-JVM distributed tests (dtests). Use when creating tests that simulate multi-node Cassandra clusters within a single JVM for faster integration testing. Covers cluster creation (single-node, multi-node, multi-datacenter), configuration (all cassandra.yaml parameters, features, network topology), instance lifecycle (startup/shutdown/restart), query execution, message filtering for failure scenarios, running code on instances, ClusterUtils utilities, and debugging classloader-related issues (serialization failures, same-class-different-classloader problems).
---

# Apache Cassandra In-JVM DTest Writer

## Overview

Write comprehensive distributed tests for Apache Cassandra using the in-JVM dtest framework. This framework enables multi-node cluster simulation within a single JVM using isolated classloaders, providing fast and reliable integration testing without actual network communication.

## Core Concepts

### Framework Architecture

The in-JVM dtest framework uses **classloader isolation** to run multiple Cassandra instances in one JVM:

- **Shared ClassLoader**: Commo
```

</details>
