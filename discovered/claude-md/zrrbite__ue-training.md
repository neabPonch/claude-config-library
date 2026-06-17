---
name: zrrbite__ue-training
source: https://github.com/zrrbite/ue-training/blob/c7faf0bab4133801fd0a061bd66cede15ecf1393/CLAUDE.md
repo: zrrbite/ue-training
kind: claude-md
stars: 0
last_pushed: 2025-11-29T10:56:54Z
license: unknown
score: 8
domains: [game-dev, cpp, unreal-engine]
tags: [unreal-engine, cpp, coding-standards, memory-management]
curated: 2026-06-16
curated_by: config-scout
---

# zrrbite/ue-training — claude-md

**Why it's worth keeping:** It uses critical negative constraints (e.g., 'Never use TSharedPtr with UObjects') that prevent common LLM hallucinations in specialized frameworks, alongside strict structural guidelines for repository expansion.

**Summary:** Provides high-density domain-specific rules for Unreal Engine C++ development, focusing on memory management and thread safety.

**Source credibility:** Low social proof (0 stars), but content demonstrates high-level domain expertise in Unreal Engine architecture.

**Recency:** Current; incorporates modern UE5 Task System and async patterns.

**Source:** [zrrbite/ue-training/CLAUDE.md](https://github.com/zrrbite/ue-training/blob/c7faf0bab4133801fd0a061bd66cede15ecf1393/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository is an Unreal Engine C++ training program with comprehensive modules covering:
- **Module 1:** Smart Pointers and References (UObject, TSharedPtr, TSharedRef, TWeakPtr, TUniquePtr)
- **Module 2:** Task System (Tasks::FTask, AsyncTask, parallel patterns)

Each module contains theory (README.md), practical examples, and exercises with solutions.

## Repository Structure

```
Module01_SmartPointers/
├── README.md              # Comprehensive smart pointer guide
├── Examples/              # 6 example files (01-06)
└── Exercises/             # 2 exercises with solutions

Module02_TaskSystem/
├── README.md              # Comprehensive task system guide
├── Examples/              # 4 example files (01-04)
└── Exercises/             # Exercises with solutions

README.md                  # Main training program overview
CLAUDE.md                  # This file
```

## Unreal Engine C++ Guidelines

### Coding Standards
- Follow Unreal Engine coding standards (PascalCase for classes/functions)
- Prefix classes: U (UObject), A (AActor), F (struc
```

</details>
