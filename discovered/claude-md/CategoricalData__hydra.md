---
name: CategoricalData__hydra
source: https://github.com/CategoricalData/hydra/blob/f6585868f65aaf9b0446abae47997c336a01c27a/CLAUDE.md
repo: CategoricalData/hydra
kind: claude-md
stars: 171
last_pushed: 2026-06-15T18:30:33Z
license: apache-2.0
score: 9
domains: [systems-programming, compiler-design, tooling]
tags: [workflow-automation, state-persistence, environment-verification]
curated: 2026-06-15
curated_by: config-scout
---

# CategoricalData/hydra — claude-md

**Why it's worth keeping:** Implements a 'local plan' pattern for persistent task memory and includes rigorous environment/worktree verification steps essential for agentic safety.

**Summary:** Defines architectural truth sources and enforces strict operational workflows to manage complex self-hosting build processes. It uses unique session-identification and local plan files for state management.

**Source credibility:** High; the repo is active, highly specialized, and demonstrates sophisticated build-system requirements.

**Recency:** Current; reflects modern agentic workflow needs like worktree awareness and state tracking.

**Source:** [CategoricalData/hydra/CLAUDE.md](https://github.com/CategoricalData/hydra/blob/f6585868f65aaf9b0446abae47997c336a01c27a/CLAUDE.md) · 171★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# LLM quickstart guide for Hydra

This document orients an LLM assistant (or human reader) to the Hydra project.
It provides just enough context to begin working, then links to detailed documentation.
Prefer consulting linked docs over relying on summaries here.

## What is Hydra?

Hydra is a functional programming language based on the LambdaGraph data model.
It explores an isomorphism between typed lambda calculus and labeled hypergraphs:
**programs are graphs, and graphs are programs.**

Hydra is self-hosting: the kernel is defined in Haskell-based DSLs and code-generated
into eight host languages spanning five implementation families:
Haskell, Java, Python, Scala, and Lisp (Clojure, Common Lisp, Emacs Lisp, Scheme — sharing one coder).
All eight pass the common test suite as targets; Haskell, Java, Python, Scala, and the JVM/native
Lisp dialects also self-host (Emacs Lisp is still maturing as a host — see README implementation
status).

The Java and Python coder DSL sources (`packages/hydra-{java,python}/`) are
authored in Java and Python respectively (host-native), and are now the **sole** source of truth: the
Haskell DSL copies under `packages/hydra-{java,python}/src/main/has
```

</details>
