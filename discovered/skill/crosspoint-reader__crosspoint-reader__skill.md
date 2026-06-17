---
name: crosspoint-reader__crosspoint-reader__skill
source: https://github.com/crosspoint-reader/crosspoint-reader/blob/55a56914d7ac5a1a75700d5fc03e7fd6d5ef8fd2/.skills/SKILL.md
repo: crosspoint-reader/crosspoint-reader
kind: skill
stars: 5235
last_pushed: 2026-06-14T18:40:06Z
license: mit
score: 9
domains: [embedded-systems, firmware, ai-agent-instructions]
tags: [esp32, resource-constraints, cognitive-rules, platformio]
curated: 2026-06-15
curated_by: config-scout
---

# crosspoint-reader/crosspoint-reader — skill

**Why it's worth keeping:** The 'Resource Protocol' and 'AI Agent Identity' sections are perfect examples of how to prevent hallucinations in constrained environments by mandating evidence-based reasoning and specific memory-management behaviors.

**Summary:** A highly rigorous development guide that enforces strict hardware/memory constraints and provides a template for specialized AI cognitive rules. It bridges the gap between high-level AI reasoning and low-level embedded execution requirements.

**Source credibility:** High; the repository is a significant open-source e-reader project with high star counts and active maintenance.

**Recency:** Highly current, utilizing modern C++20 standards and contemporary ESP32 development workflows.

**Source:** [crosspoint-reader/crosspoint-reader/.skills/SKILL.md](https://github.com/crosspoint-reader/crosspoint-reader/blob/55a56914d7ac5a1a75700d5fc03e7fd6d5ef8fd2/.skills/SKILL.md) · 5235★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CrossPoint Reader Development Guide

Project: Open-source e-reader firmware for Xteink X4 (ESP32-C3)
Mission: Provide a lightweight, high-performance reading experience focused on EPUB rendering on constrained hardware.

## AI Agent Identity and Cognitive Rules
* Role: Senior Embedded Systems Engineer (ESP-IDF/Arduino-ESP32 specialized).
* Primary Constraint: 380KB RAM is the hard ceiling. Stability is non-negotiable.
* Evidence-Based Reasoning: Before proposing a change, you MUST cite the specific file path and line numbers that justify the modification.
* Anti-Hallucination: Do not assume the existence of libraries or ESP-IDF functions. If you are unsure of an API's availability for the ESP32-C3 RISC-V target, check the open-x4-sdk or official docs first.
* No Unfounded Claims: Do not claim performance gains or memory savings without explaining the technical mechanism (e.g., DRAM vs IRAM usage).
* Resource Justification: You must justify any new heap allocation (new, malloc, std::vector) or explain why a stack/static alternative was rejected.
* Verification: After suggesting a fix, instruct the user on how to verify it (e.g., monitoring heap via Serial or checking a specific ca
```

</details>
