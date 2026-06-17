---
name: Loxodromics__LillUgsi
source: https://github.com/Loxodromics/LillUgsi/blob/0a01ba6a12a91e62c491bc5e8330f3c0adc8c810/CLAUDE.md
repo: Loxodromics/LillUgsi
kind: claude-md
stars: 1
last_pushed: 2026-01-25T17:07:11Z
license: mit
score: 9
domains: [graphics-programming, cpp-systems]
tags: [vulkan, pbr, architecture, cpp]
curated: 2026-06-15
curated_by: config-scout
---

# Loxodromics/LillUgsi — claude-md

**Why it's worth keeping:** The 'Graphics Programming Notes' prevent common LLM hallucinations regarding depth buffering and PBR energy conservation, while the '@file' indexing pattern is a top-tier technique for navigating large codebases.

**Summary:** Provides rigorous C++20 coding standards alongside critical domain-specific graphics knowledge regarding PBR math and Vulkan state. It uses a sophisticated multi-file indexing system to help the AI navigate complex subsystems.

**Source credibility:** A high-quality personal project focused on specialized graphics architecture.

**Recency:** Current; reflects modern C++20 and Vulkan workflows.

**Source:** [Loxodromics/LillUgsi/CLAUDE.md](https://github.com/Loxodromics/LillUgsi/blob/0a01ba6a12a91e62c491bc5e8330f3c0adc8c810/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LillUgsi is a C++ Vulkan learning renderer built for educational purposes. It features a modular architecture with modern C++ practices, physically-based rendering (PBR), and a comprehensive scene management system.

## Coding Style Guidelines

- Use camelCase for methods and variables, PascalCase for classes and enums
- Use kPascalCase for constants
- Use all lowercase letters for filenames without underscores or hyphens
- Use lowercase with underscores for namespaces
- Follow Qt's coding style guidelines, but access all members via this-> instead of prefixing with m_
- Use "pointer-to-type" style
- Use K&R brace placement
- Place implementation (.cpp) and header (.h) files next to each other in the src directory
- Use three slashes (///) for comments to differentiate from commented code
- Use tabs for indentation with 4-space tab stops
- Comments should explain complex algorithms, business decisions, and non-obvious code patterns. Do not comment self-explanatory code like simple getters, setters, or obvious operations. Focus on WHY the code exi
```

</details>
