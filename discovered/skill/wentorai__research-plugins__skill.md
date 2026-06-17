---
name: wentorai__research-plugins__skill
source: https://github.com/wentorai/research-plugins/blob/9e6584e2d0a74cf8992f470a45c2f07c862bf72c/skills/domains/cs/distributed-systems-guide/SKILL.md
repo: wentorai/research-plugins
kind: skill
stars: 234
last_pushed: 2026-06-14T02:50:06Z
license: mit
score: 8
domains: [computer-science, distributed-systems, backend]
tags: [consensus, replication, cap-theorem, raft]
curated: 2026-06-15
curated_by: config-scout
---

# wentorai/research-plugins — skill

**Why it's worth keeping:** It uses Python classes to define formal logical models (Raft, Vector Clocks), which provides the agent with much higher-precision mental models than prose alone.

**Summary:** A dense knowledge-base providing theoretical frameworks and code-based implementation patterns for distributed systems design.

**Source credibility:** High; the source repository is well-starred and actively maintained.

**Recency:** 

**Source:** [wentorai/research-plugins/skills/domains/cs/distributed-systems-guide/SKILL.md](https://github.com/wentorai/research-plugins/blob/9e6584e2d0a74cf8992f470a45c2f07c862bf72c/skills/domains/cs/distributed-systems-guide/SKILL.md) · 234★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: distributed-systems-guide
description: "Distributed systems design patterns and analysis for CS research"
metadata:
  openclaw:
    emoji: "🌐"
    category: "domains"
    subcategory: "cs"
    keywords: ["distributed-systems", "consensus", "replication", "fault-tolerance", "scalability", "cap-theorem"]
    source: "wentor"
---

# Distributed Systems Guide

A skill for researching and designing distributed systems, covering consensus algorithms, replication strategies, consistency models, fault tolerance, and performance analysis. Provides theoretical foundations and practical implementations relevant to systems research.

## Consistency Models

### Consistency Hierarchy

```
Strongest
  |  Linearizability (atomic, real-time ordering)
  |  Sequential consistency (program order respected)
  |  Causal consistency (causally related ops ordered)
  |  PRAM / FIFO consistency (per-process order)
  |  Eventual consistency (converges if updates stop)
Weakest
```

### CAP Theorem and PACELC

The CAP theorem states that during a network partition, a distributed system must choose between consistency and availability:

| System | Partition Behavior | Normal Behavior | Classification
```

</details>
