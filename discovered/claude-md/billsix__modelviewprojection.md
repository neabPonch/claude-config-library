---
name: billsix__modelviewprojection
source: https://github.com/billsix/modelviewprojection/blob/c1f9d6d4038c9e3d6cf5ace81dbd29931e864830/CLAUDE.md
repo: billsix/modelviewprojection
kind: claude-md
stars: 2
last_pushed: 2026-06-15T02:32:25Z
license: other
score: 9
domains: [graphics-programming, education, computer-science]
tags: [opengl, pedagogy, mathematics, instructional-design]
curated: 2026-06-15
curated_by: config-scout
---

# billsix/modelviewprojection — claude-md

**Why it's worth keeping:** It uses 'negative constraints' (e.g., 'don't clean up by introducing classes') and mandatory terminology rules to prevent the AI from breaking the project's educational intent.

**Summary:** Provides deep pedagogical context and strict mathematical vocabulary constraints to ensure AI-generated code adheres to a specific teaching philosophy.

**Source credibility:** High; authored by an instructor specifically to guide development/porting of his own curriculum.

**Recency:** Very current; contains specific updates dated as late as June 2026.

**Source:** [billsix/modelviewprojection/CLAUDE.md](https://github.com/billsix/modelviewprojection/blob/c1f9d6d4038c9e3d6cf5ace81dbd29931e864830/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MVP — context for Claude

This is **modelviewprojection**, an OpenGL graphics course taught by William "Bill" Six (billsix@gmail.com) from his own codebase. The repo *is* the textbook (Sphinx book in `book/docs/`, one chapter per demo). Teaching philosophy is **"mistake-driven development"** (stated in README) — demos are deliberately procedural, with module-level globals, so students read top-to-bottom. Don't "clean up" by introducing classes/abstractions unless asked.

External sources Bill draws from: **OpenGL SuperBible v4** (main porting source — see `ports/openglsuperbiblev4/`), *Mathematics for 3D Game Programming*, *Computer Graphics: Principles and Practice*.

---

## Central abstraction — Cayley graphs + `InvertibleFunction`

The whole curriculum is built on **one substituted abstraction**: instead of 4×4 matrices, transformations are `InvertibleFunction`s on `Vector2`/`Vector3`, and coordinate systems form a **Cayley graph** where nodes are spaces and directed edges are these functions.

> **Note (2026-06-08):** `mathutils.py` is now a **façade over the `gacalc` geometric-algebra library** — `Vector2`/`Vector3` are gacalc's graded vector types (the old in-repo `Vector2
```

</details>
