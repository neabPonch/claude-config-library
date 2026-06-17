---
name: beriberikix__zephyr-agent-skills__skill
source: https://github.com/beriberikix/zephyr-agent-skills/blob/ed63cdfb8cdfbeb5946ea39c33f4aa6bcf3a5cce/skills/zephyr-foundations/SKILL.md
repo: beriberikix/zephyr-agent-skills
kind: skill
stars: 48
last_pushed: 2026-05-18T20:57:40Z
license: apache-2.0
score: 8
domains: [embedded-systems, c, rtos]
tags: [zephyr, embedded, devicetree, concurrency]
curated: 2026-06-15
curated_by: config-scout
---

# beriberikix/zephyr-agent-skills — skill

**Why it's worth keeping:** Includes a 'Validation Checklist' that turns passive knowledge into active agent instructions; uses high-density technical vocabulary to reduce ambiguity in C code generation.

**Summary:** Provides essential domain constraints for Zephyr RTOS development, covering macros, concurrency primitives, and Devicetree integration.

**Source credibility:** Niche but specialized repository with relevant star count for the domain.

**Recency:** Highly current, updated within the last month.

**Source:** [beriberikix/zephyr-agent-skills/skills/zephyr-foundations/SKILL.md](https://github.com/beriberikix/zephyr-agent-skills/blob/ed63cdfb8cdfbeb5946ea39c33f4aa6bcf3a5cce/skills/zephyr-foundations/SKILL.md) · 48★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: zephyr-foundations
description: Foundational skills for Zephyr RTOS development. Covers essential Embedded C patterns (BIT, CONTAINER_OF), real-time concurrency primitives (mutexes, semaphores, spinlocks), hardware literacy (datasheet-to-DTS mapping), and defensive programming. Trigger when writing core application logic, drivers, or troubleshooting foundational behavior.
---

# Zephyr Foundations

Mastering the bedrock of Zephyr is essential for writing efficient, robust, and idiomatic code.

## Core Workflows

### 1. Idiomatic C Patterns
Zephyr uses specific macros to manage memory and hardware-software mapping.
- **Reference**: **[zephyr_macros.md](references/zephyr_macros.md)**
- **Key Tools**: `CONTAINER_OF`, `BIT()`, `GENMASK()`, `ARRAY_SIZE`.

### 2. Real-Time Concurrency
Safe multi-threading and interrupt handling are critical for stability.
- **Reference**: **[concurrency.md](references/concurrency.md)**
- **Key Tools**: `k_mutex`, `k_sem`, `k_spinlock`, `atomic_t`, ISR safety rules.

### 3. Hardware Literacy (Devicetree)
Understanding how code interacts with the hardware description.
- **Reference**: **[devicetree_basics.md](references/devicetree_basics.md)**
-
```

</details>
