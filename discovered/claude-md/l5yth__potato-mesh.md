---
name: l5yth__potato-mesh
source: https://github.com/l5yth/potato-mesh/blob/efd2c59fb8bba927a15e88fe0f5d730634867524/CLAUDE.md
repo: l5yth/potato-mesh
kind: claude-md
stars: 328
last_pushed: 2026-05-28T21:24:58Z
license: apache-2.0
score: 9
domains: [backend, devops, polyglot-systems]
tags: [high-rigor, architectural-guide, polyglot]
curated: 2026-06-15
curated_by: config-scout
---

# l5yth/potato-mesh — claude-md

**Why it's worth keeping:** Provides specific command execution paths for multi-environment workflows and explicit interface patterns that allow an AI to extend the system safely.

**Summary:** Defines strict technical standards and precise operational commands for a complex polyglot architecture.

**Source credibility:** High; significant stars and very recent maintenance activity in the repository.

**Recency:** Current; aligns with modern devops, containerization, and polyglot workflow standards.

**Source:** [l5yth/potato-mesh/CLAUDE.md](https://github.com/l5yth/potato-mesh/blob/efd2c59fb8bba927a15e88fe0f5d730634867524/CLAUDE.md) · 328★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
<!-- Copyright © 2025-26 l5yth & contributors -->
<!-- Licensed under the Apache License, Version 2.0 (see LICENSE) -->

# Repository Guidelines

Keep code as modular as possible to reduce duplication and improve reusability and readability — this applies to tests as well as production code. If a module grows large, split it into a submodule structure. Prefer composing small, single-purpose units over monolithic files.

Make sure all tests pass for Python (`pytest`), Ruby (`rspec`), and JavaScript (`npm test`).

All code must be 100% unit tested — every line, branch, and code path must have a unit test. "100%" is the floor, not the ceiling: smoke tests, integration tests, and end-to-end tests come on top of that. No new code ships without matching unit tests.

All code must be 100% documented according to the language's API-doc standard (PDoc for Python, RDoc for Ruby, JSDoc for JavaScript, rustdoc for Rust, dartdoc for Dart). Documentation must be sufficient to generate complete API docs from source. In addition to API-level docs, add inline comments wherever the logic is not immediately self-evident.

Every file in the repository must carry an Apache v2 license notice using the e
```

</details>
