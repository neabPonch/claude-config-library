---
name: wado-lang__wado__skill
source: https://github.com/wado-lang/wado/blob/7431ff8f79be7ade745e87351e966bb83b9d3aba/.claude/skills/optimizer-debug/SKILL.md
repo: wado-lang/wado
kind: skill
stars: 90
last_pushed: 2026-06-16T07:05:11Z
license: mit
score: 9
domains: [compiler-engineering, systems-programming]
tags: [debugging, compiler, optimization, wasm]
curated: 2026-06-16
curated_by: config-scout
---

# wado-lang/wado — skill

**Why it's worth keeping:** It contains highly specific shell recipes for bisecting failures and a structured workflow to isolate which optimization pass corrupts the WIR pipeline.

**Summary:** This skill provides a systematic debugging playbook for inspecting compiler optimization passes via environment variables. It enables IR dumping, pass skipping (with iteration control), and internal execution tracing.

**Source credibility:** High; comes from an active systems/language project with clear expert authorship.

**Recency:** Recent; perfectly aligned with modern CLI debugging workflows.

**Source:** [wado-lang/wado/.claude/skills/optimizer-debug/SKILL.md](https://github.com/wado-lang/wado/blob/7431ff8f79be7ade745e87351e966bb83b9d3aba/.claude/skills/optimizer-debug/SKILL.md) · 90★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: optimizer-debug
description: Debug Wado optimizer (NIR/WIR pass) bugs using WADO_TRACE, WADO_DUMP_PASS_BEFORE/AFTER, WADO_LIST_PASSES, and WADO_SKIP_PASS env vars. Use when an optimization pass produces wrong code, ICEs the WIR pipeline ("invalid core Wasm module: type mismatch ..."), or when you need to see how a specific pass transforms the IR.
---

# Optimizer pass debugging

The `optimize.rs` and `wir_optimize.rs` pipelines are big — many passes,
each rewriting the IR in place. When a pass is wrong, the symptom usually
shows up two passes later as "the WIR validates but produces the wrong
behaviour" or as "the codegen finds an invalid Wasm module" deep in the
final emitter. The debug hooks below let you diff the IR around any
single pass without sprinkling `eprintln!` through pass internals.

All three are env-var-driven so they work uniformly across `wado compile`,
`wado test`, `wado run`, and Kiln invocations from `package-gale`.

## Quick recipes

### Which pass changed the IR?

```sh
WADO_LIST_PASSES=1 cargo run --bin wado --quiet -- compile -O1 file.wado -o /tmp/out.wasm 2>&1 | grep '\[pass\]'
```

Prints every pass name in execution order. Lets you correlate the
```

</details>
