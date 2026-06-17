---
name: FStarLang__pulse-verified-gc__extraction-skill
source: https://github.com/FStarLang/pulse-verified-gc/blob/fa82ce6a592434a9d322ddb5bb597aa7f457dfa6/EXTRACTION_SKILL.md
repo: FStarLang/pulse-verified-gc
kind: skill
stars: 5
last_pushed: 2026-06-14T23:50:27Z
license: unknown
score: 9
domains: [systems-programming, formal-verification, compilers]
tags: [fstar, pulse, c-extraction, karamel, verified-code]
curated: 2026-06-16
curated_by: config-scout
---

# FStarLang/pulse-verified-gc — skill

**Why it's worth keeping:** It documents critical 'gotchas' like the module extraction naming quirk and provides a rigorous mapping of high-level types to low-level C representations. The structural breakdown of 'Spec vs Low-level' layers is an excellent pattern for technical documentation.

**Summary:** A highly specialized guide for extracting verified F*/Pulse code into C using the KaRaMeL compiler. It covers full-pipeline execution, complex bundling syntax, and coding patterns to ensure successful translation.

**Source credibility:** High; originates from a specialized repository for verified garbage collectors with recent activity.

**Recency:** Current; reflects specific nuances of the F*/Pulse toolchain required for modern extraction.

**Source:** [FStarLang/pulse-verified-gc/EXTRACTION_SKILL.md](https://github.com/FStarLang/pulse-verified-gc/blob/fa82ce6a592434a9d322ddb5bb597aa7f457dfa6/EXTRACTION_SKILL.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: krmlextraction
description: Extract verified F*/Pulse code to C using KaRaMeL, including bundling, naming, coding patterns, and build integration
---

## Invocation
This skill is used when:
- Extracting verified F* or Pulse code to C via KaRaMeL
- Configuring `-bundle` options for controlling C output structure
- Designing F*/Pulse module hierarchies for clean C extraction
- Debugging extraction issues (missing symbols, naming, includes)
- Building and testing extracted C code

## Overview

KaRaMeL (krml) translates a subset of F* (called Low*) and Pulse to C.
The pipeline is:

1. **F* verification** — `fstar.exe` checks `.fst`/`.fsti` files
2. **F* extraction to .krml** — `fstar.exe --codegen krml --extract ModuleName`
3. **KaRaMeL translation to C** — `krml` reads `.krml` files and produces `.c`/`.h`

## Two-Phase Extraction

### Phase 1: F* → .krml

Each module is extracted individually:

```bash
# Regular F* modules
fstar.exe --codegen krml --extract 'MyModule' --odir _output MyModule.fst

# #lang-pulse modules produce out.krml instead of ModuleName.krml
fstar.exe --codegen krml --extract 'My.Pulse.Module' --odir _output pulse/My.Pulse.Module.fst
# IMPORTANT: rename o
```

</details>
