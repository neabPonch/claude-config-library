---
name: khaneliman__khanelinix__skill
source: https://github.com/khaneliman/khanelinix/blob/44fa50ec72fad088a08b2d0262b1d345e2c2cd64/modules/common/ai-tools/skills/writing-nix/SKILL.md
repo: khaneliman/khanelinix
kind: skill
stars: 334
last_pushed: 2026-06-15T01:09:37Z
license: unknown
score: 9
domains: [devops, infrastructure-as-code]
tags: [nix, style-guide, devops]
curated: 2026-06-15
curated_by: config-scout
---

# khaneliman/khanelinix — skill

**Why it's worth keeping:** The 'Output Contract' ensures predictable results, while the 'Style Authority' provides clear conflict-resolution logic for local vs. skill guidelines. The structure is highly transferable as it teaches how to manage specialized knowledge via reference files.

**Summary:** This skill enforces idiomatic, explicit Nix coding standards through structured style rules and a strict output contract. It prioritizes module merge semantics and scope clarity over decorative abstractions.

**Source credibility:** High; derived from a well-maintained personal Nix configuration repository used for real systems.

**Recency:** Current; the use of an output contract and structured validation matches modern agentic tool patterns.

**Source:** [khaneliman/khanelinix/modules/common/ai-tools/skills/writing-nix/SKILL.md](https://github.com/khaneliman/khanelinix/blob/44fa50ec72fad088a08b2d0262b1d345e2c2cd64/modules/common/ai-tools/skills/writing-nix/SKILL.md) · 334★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: writing-nix
description: Write idiomatic and maintainable Nix code. Use when creating or refactoring Nix expressions, Home Manager or NixOS modules, overlays, packages, and flake outputs, especially when deciding module merge semantics, binding locality, option defaults, and conditional structure.
---

# Writing Nix

Write boring, explicit Nix that follows this skill's opinionated style. Prefer
module merge semantics, narrow scopes, and simple attrset composition over
decorative abstractions.

## Quick Start

1. Read repository docs only for hard constraints or project-specific layout. Do
   not weaken the style rules in this skill unless the user explicitly asks.
2. Identify the task shape and load only the relevant reference files:
   - [references/module-style.md](references/module-style.md): module templates,
     option design, merge priority, `mkDefault`, `mkForce`, and `mkMerge`.
   - [references/bindings.md](references/bindings.md): `let` locality,
     single-use bindings, `inherit (...)`, and bulky inline expressions.
   - [references/assertions-and-warnings.md](references/assertions-and-warnings.md):
     when to fail evaluation, when to warn, and when simpler
```

</details>
