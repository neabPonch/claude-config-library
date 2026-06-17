---
name: ray-project__ray__skill
source: https://github.com/ray-project/ray/blob/ca01ff18205845a807d5a7b4fdadd4193aabe5a2/.claude/skills/rebuild/SKILL.md
repo: ray-project/ray
kind: skill
stars: 42880
last_pushed: 2026-06-15T07:10:54Z
license: apache-2.0
score: 9
domains: [machine-learning, distributed-systems, developer-tools]
tags: [build-automation, bazel, python, cpp, polyglot]
curated: 2026-06-15
curated_by: config-scout
---

# ray-project/ray — skill

**Why it's worth keeping:** It demonstrates the 'diff-driven build' pattern which is highly transferable for any large polyglot repository. It also includes practical environmental tuning like resource-constrained Bazel configurations.

**Summary:** This skill provides a decision tree for rebuilding Ray based on `git diff` analysis to determine if Python, C++, or Dashboard components need updates. It optimizes developer time by distinguishing between fast editable installs and heavy Bazel builds.

**Source credibility:** Extremely high; Ray is a Tier-1 industry standard AI compute engine with massive community backing.

**Recency:** Very recent, as the source repository is actively maintained.

**Source:** [ray-project/ray/.claude/skills/rebuild/SKILL.md](https://github.com/ray-project/ray/blob/ca01ff18205845a807d5a7b4fdadd4193aabe5a2/.claude/skills/rebuild/SKILL.md) · 42880★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rebuild
description: Rebuild Ray from source — determines the right build mode based on what changed
---

# Rebuild Ray

Canonical build docs: doc/source/ray-contribute/development.rst
Use the user's configured Python from CLAUDE.local.md, or fall back to `which python`.
Update this skill if any changes are detected in development.rst.

## Determine what to rebuild

1. Check what files changed: `git diff --name-only HEAD` (or ask the user)
2. Pick the appropriate build mode:
   - **Only .py files changed** (no .h, .cc, .pyx, .pxd) → Python-only rebuild (not required if installed with `pip install -e .` — editable mode auto-picks up Python changes)
   - **.h, .cc, .pyx, .pxd files changed** → C++/Cython rebuild
   - **Dashboard files changed** (python/ray/dashboard/client/) → Dashboard rebuild first
   - **First time / clean build** → Full source build

**Running Python tests that exercise C++ changes:** When a Python test depends on
C++ or Cython code (raylet, GCS, core_worker, etc.), run the C++/Cython rebuild
below before running the test. Editable Python installs do not rebuild the compiled
extensions, so stale binaries will run otherwise.

## Python-only rebuild

For
```

</details>
