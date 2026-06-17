---
name: dill-lk__Claude-Skillls__claude-skill
source: https://github.com/dill-lk/Claude-Skillls/blob/9679fb56622f507dac2f44d78b761faa1e023b18/api-design/claude.skill.md
repo: dill-lk/Claude-Skillls
kind: skill
stars: 2
last_pushed: 2026-03-30T17:06:09Z
license: mit
score: 8
domains: [backend-api, architecture]
tags: [api-design, rest, graphql, grpc, openapi]
curated: 2026-06-16
curated_by: config-scout
---

# dill-lk/Claude-Skillls — skill

**Why it's worth keeping:** Includes advanced engineering-specific patterns like idempotency, rate limiting, and error-response standardization that go beyond basic CRUD instructions.

**Summary:** A comprehensive framework for designing and reviewing diverse API architectures including REST, GraphQL, and gRPC.

**Source credibility:** Low star count but high content quality suggests a human-curated technical resource rather than an auto-generated dump.

**Recency:** Highly current; utilizes modern standards such as OpenAPI 3.0 and proto3.

**Source:** [dill-lk/Claude-Skillls/api-design/claude.skill.md](https://github.com/dill-lk/Claude-Skillls/blob/9679fb56622f507dac2f44d78b761faa1e023b18/api-design/claude.skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill: API Design

Design, review, and evolve APIs — REST, GraphQL, gRPC, and event-driven — using Claude as a collaborative API architect.

---

## Overview

Claude can help you design clear, consistent, versioned, and developer-friendly APIs. This skill covers resource modelling, endpoint design, error conventions, versioning strategy, and OpenAPI specification generation.

---

## Task Patterns

### 1. Design a REST API from a Domain Model

**Prompt template:**
```
Design a RESTful API for [domain/feature name].

Domain entities and relationships:
- [entity 1]: [attributes]
- [entity 2]: [attributes]
- Relationship: [describe]

Operations required:
- [CRUD operation list]
- [any non-CRUD operations, e.g., approve, publish, archive]

Requirements:
- Follow REST conventions (resource-based URIs, correct HTTP verbs)
- Return appropriate HTTP status codes
- Use consistent JSON response envelopes
- Support pagination for collection endpoints
```

---

### 2. Generate an OpenAPI / Swagger Specification

**Prompt template:**
```
Generate a complete OpenAPI 3.0 specification (YAML) for the following API:

[Describe endpoints, request/response shapes, and authentication]

Include:
- Al
```

</details>
