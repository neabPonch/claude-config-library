---
name: UC-Davis-molecular-computing__automata-solid
source: https://github.com/UC-Davis-molecular-computing/automata-solid/blob/65192920d27e96667ba5ed05b8d4b667e36354bf/CLAUDE.md
repo: UC-Davis-molecular-computing/automata-solid
kind: claude-md
stars: 4
last_pushed: 2026-04-06T18:37:54Z
license: unknown
score: 9
domains: [web-frontend, typescript]
tags: [vitest, playwright, workflow-optimization, type-safety]
curated: 2026-06-15
curated_by: config-scout
---

# UC-Davis-molecular-computing/automata-solid — claude-md

**Why it's worth keeping:** It teaches the agent 'anti-patterns' (like avoiding `npm test` due to timeouts) and enforces high-quality TypeScript patterns using custom utility functions instead of unsafe operators.

**Summary:** Provides architectural context and critical workarounds for common tool behaviors that cause AI agents to hang or timeout. It includes specific commands to bypass watch-mode and interactive reporter issues.

**Source credibility:** Strong; maintained academic/research repository with recent updates.

**Recency:** Current; addresses modern tooling issues like Vitest watch mode and Playwright reporter behaviors.

**Source:** [UC-Davis-molecular-computing/automata-solid/CLAUDE.md](https://github.com/UC-Davis-molecular-computing/automata-solid/blob/65192920d27e96667ba5ed05b8d4b667e36354bf/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a TypeScript rewrite of an automata simulator web application.

The TypeScript version should:
- Use **SolidJS** framework with **Elm Architecture** pattern (Model-View-Update)
- Follow imperative logic patterns from the Dart implementation
- Use **YAML format** for automata specifications instead of custom parsers
- Implement core automata classes: DFA, NFA, TM (Turing Machine), CFG, Regex

## Core Architecture

### Automata Classes Structure (from Dart reference)
- `AbstractAutomaton`: Base class with states, input alphabet, start state, accept states
- `DFA`: Deterministic Finite Automaton with transition function delta
- `NFA`: Non-deterministic Finite Automaton 
- `TM`: Turing Machine with tape operations
- `CFG`: Context-Free Grammar
- `Regex`: Regular Expression processor

### Key Methods (from automata-dart/lib/src/)
- `accepts(input: string)`: Test if automaton accepts input string
- `deltaExtended()`: Extended transition function for strings
- `statesVisited()`: Track states during string processing
- Validation methods for ensu
```

</details>
