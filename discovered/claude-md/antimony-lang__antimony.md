---
name: antimony-lang__antimony
source: https://github.com/antimony-lang/antimony/blob/0a199f1424bea24c5342bdc19d1ac6dd92b0cd8f/CLAUDE.md
repo: antimony-lang/antimony
kind: claude-md
stars: 168
last_pushed: 2026-04-27T12:58:19Z
license: apache-2.0
score: 9
domains: [systems-programming, compilers, cli-tools]
tags: [rust, compiler-design, high-granularity]
curated: 2026-06-15
curated_by: config-scout
---

# antimony-lang/antimony — claude-md

**Why it's worth keeping:** The high granularity of 'Conventions'—specifically how to name test helpers and handle error propagation—ensures the LLM maintains highly consistent code style in complex systems logic.

**Summary:** Provides exhaustive technical context including exact dependency versions, strict naming conventions, and structural architectural patterns for a compiler project.

**Source credibility:** A growing niche programming language project with active maintenance (pushed 2 months ago).

**Recency:** Highly current, utilizing recent Rust versions and modern dependency specifications.

**Source:** [antimony-lang/antimony/CLAUDE.md](https://github.com/antimony-lang/antimony/blob/0a199f1424bea24c5342bdc19d1ac6dd92b0cd8f/CLAUDE.md) · 168★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
<!-- GSD:project-start source:PROJECT.md -->
## Project

**Antimony**

Antimony is a personal-project compiled programming language with a multi-backend architecture (JS, C, QBE, LLVM, x86). The immediate goal is to mature the QBE backend until two milestones are reached: a bootstrapped compiler (the Antimony compiler written in Antimony and compiled via QBE) and a Doom port written in Antimony.

**Core Value:** The QBE backend must become capable enough that real systems programs — including the compiler itself — can be written in Antimony and compiled correctly.

### Constraints

- **Tech Stack**: QBE as the primary backend — all systems-level work must target QBE
- **Bootstrap**: The bootstrapped compiler must be a full rewrite (not a subset), compiled via QBE
- **Personal project**: No team, no deadlines — prioritize learning and correctness over velocity
<!-- GSD:project-end -->

<!-- GSD:stack-start source:codebase/STACK.md -->
## Technology Stack

## Languages
- Rust 1.93 - Core compiler implementation, lexer, parser, code generators, CLI
- Python 3.8 - Documentation build tooling
- C - Backend/intermediate language target for compilation
- JavaScript - Backend/intermediate
```

</details>
