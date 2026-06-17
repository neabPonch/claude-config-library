---
name: twilwa__api-design-skills-package-v2__seed-skill
source: https://github.com/twilwa/api-design-skills-package-v2/blob/af0dff1106376db9a6d150955179ca07850470d7/SEED-SKILL.md
repo: twilwa/api-design-skills-package-v2
kind: skill
stars: 0
last_pushed: 2026-03-21T00:05:10Z
license: unknown
score: 8
domains: [backend-api, software-architecture]
tags: [api-design, contract-first, system-architecture]
curated: 2026-06-16
curated_by: config-scout
---

# twilwa/api-design-skills-package-v2 — skill

**Why it's worth keeping:** The 'Common Pitfalls' section prevents common architectural mistakes, while the comparison-based workflow teaches the agent to use specific, shared-domain examples for cross-protocol analysis.

**Summary:** This skill provides a high-level API architecture persona that uses contrastive examples (REST vs GraphQL vs gRPC) to guide design decisions. It emphasizes contract-first development and lifecycle management through a structured workflow.

**Source credibility:** Low social proof (0 stars), but high technical depth in the instructions suggests a specialized expert-authored tool.

**Recency:** Extremely current; updated 3 months ago and highly relevant to modern agentic workflows.

**Source:** [twilwa/api-design-skills-package-v2/SEED-SKILL.md](https://github.com/twilwa/api-design-skills-package-v2/blob/af0dff1106376db9a6d150955179ca07850470d7/SEED-SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: api-design-architect
description: Broad guidance for reviewing and designing API contracts, lifecycle policies, and edge architectures using the contrastive examples in this repository.
---

# API Design Architect

## Test commands
- `make verify`
- `make typecheck`
- `make test`

This repository is a TypeScript API design corpus. Do not treat it like a Python package and do not suggest `pytest`, `ruff`, `mypy`, `python -m build`, or editable installs.

## Code structure
- `examples/shared/` contains the canonical commerce domain, fixtures, and HTTP helpers reused across all patterns.
- `examples/rest-resource-oriented/` shows pagination, idempotent writes, and problem details.
- `examples/rest-hypermedia/` shows action-oriented links and state transitions.
- `examples/graphql-schema/` shows schema-first GraphQL over the same domain.
- `examples/grpc-service/` shows protobuf-first contract design.
- `examples/async-jobs/` and `examples/webhooks-events/` cover asynchronous integration patterns.
- `examples/api-gateway-facade/`, `examples/backend-for-frontend/`, and `examples/api-composition/` cover edge orchestration patterns.
- `examples/api-manager-version-handle/` is th
```

</details>
