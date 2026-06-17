---
name: JamieMason__syncpack__skill
source: https://github.com/JamieMason/syncpack/blob/078dc6caa13c771f18988b623420e7de292fbc31/.claude/skills/fix-bug/SKILL.md
repo: JamieMason/syncpack
kind: skill
stars: 2063
last_pushed: 2026-05-19T07:25:10Z
license: mit
score: 9
domains: [cli-tools, rust]
tags: [debugging, workflow, troubleshooting]
curated: 2026-06-15
curated_by: config-scout
---

# JamieMason/syncpack — skill

**Why it's worth keeping:** The use of diagnostic mapping tables (Symptom -> Likely Cause) and specific component-to-file lookups provides an agent with essential 'tribal knowledge'. The workflow (Observe/Hypothesise/Experiment/Validate/Verify) is a perfect template for structured agentic debugging.

**Summary:** A highly structured debugging protocol that uses the scientific method to investigate issues within the syncpack codebase. It maps symptoms directly to likely causes and file locations.

**Source credibility:** Very high; based on a widely used, well-maintained tool with significant GitHub stars.

**Recency:** Current; utilizes modern Rust tooling and developer workflows.

**Source:** [JamieMason/syncpack/.claude/skills/fix-bug/SKILL.md](https://github.com/JamieMason/syncpack/blob/078dc6caa13c771f18988b623420e7de292fbc31/.claude/skills/fix-bug/SKILL.md) · 2063★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: fix-bug
description: Debug and fix bugs in Syncpack using scientific debugging methodology. Use when a test is failing, unexpected behaviour occurs, or investigating issues. Covers hypothesis-driven debugging and TDD-based fixes.
---

# Fix Bug

Guide for debugging and fixing bugs in Syncpack.

## Scientific Debugging Workflow

1. **Observe** — Understand the symptom precisely
2. **Hypothesise** — Form a theory about the root cause
3. **Experiment** — Test the hypothesis with targeted changes
4. **Validate** — Confirm the fix with tests
5. **Verify** — Run full test suite

## Step 1: Observe

Gather information before changing code:

```bash
# Run the failing test with output
cargo test test_name -- --nocapture

# Run with backtrace
RUST_BACKTRACE=1 cargo test test_name

# Test against fixture
cd fixtures/fluid-framework
cargo run -- lint
```

Questions to answer:

- What is the exact error message?
- What input triggers it?
- What is the expected vs actual behaviour?

## Step 2: Hypothesise

Common root causes by symptom:

| Symptom              | Likely Cause                                            |
| -------------------- | ------------------------------------------
```

</details>
