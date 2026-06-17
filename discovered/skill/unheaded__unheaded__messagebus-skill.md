---
name: unheaded__unheaded__messagebus-skill
source: https://github.com/unheaded/unheaded/blob/9bc3489f3b6488b933156a1596422e347362554d/skills/messagebus-SKILL.md
repo: unheaded/unheaded
kind: skill
stars: 2
last_pushed: 2026-06-03T22:23:24Z
license: gpl-3.0
score: 9
domains: [backend-infrastructure, cli-tools, systems-programming]
tags: [message-bus, grpc, protocol-spec, infrastructure]
curated: 2026-06-16
curated_by: config-scout
---

# unheaded/unheaded — skill

**Why it's worth keeping:** Uses a superior pattern of providing a 'Session Start Protocol' (referencing PROGRESS.md/CLAUDE.md) and explicit file tree mappings to guide agent navigation.

**Summary:** Provides comprehensive context for the Wotan message bus infrastructure, covering protocols (REST/gRPC), architecture, and specific code locations.

**Source credibility:** High-quality engineering evident in the technical depth, despite low star count.

**Recency:** Very current; includes modern patterns for integrating with agentic workflows.

**Source:** [unheaded/unheaded/skills/messagebus-SKILL.md](https://github.com/unheaded/unheaded/blob/9bc3489f3b6488b933156a1596422e347362554d/skills/messagebus-SKILL.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: unheaded-messagebus
description: |
  Infrastructure message bus skill for Unheaded. Understands the Wotan Protocol (BP/1), REST control plane, gRPC data plane, ring buffer architecture, pub/sub patterns, and subscriber approval workflow. Use this skill when working on message bus features, inter-service communication, event-driven patterns, or debugging message flow. Knows where the code lives, what's shipped, and what's planned. NOTE: This is different from unheaded-wotan (the coordinator skill). This is for the MESSAGE BUS infrastructure component. Triggers: message bus, messagebus, pubsub, pub/sub, gRPC streaming, ring buffer, topics, subscribers, events, inter-service, messaging, BP/1, wotan server, wotan client.
---

# Unheaded Message Bus

**The infrastructure message bus that ties everything together.**

The Wotan message bus is Unheaded's nervous system - every service talks through it. This skill knows the protocol, the architecture, and the code.

> **Note**: Don't confuse this with `unheaded-wotan` - that's the coordinator skill that helps navigate between team skills. THIS skill is about the infrastructure message bus component (the code in `/wotan/`).

## Wha
```

</details>
