---
name: actionbook__rust-skills__skill
source: https://github.com/actionbook/rust-skills/blob/fa60f7931223646fb71c4586b4a6c8545016076a/skills/rust-trait-explorer/SKILL.md
repo: actionbook/rust-skills
kind: skill
stars: 1240
last_pushed: 2026-05-24T23:33:30Z
license: unknown
score: 8
domains: [systems-programming, rust]
tags: [trait-exploration, lsp-navigation, rust]
curated: 2026-06-15
curated_by: config-scout
---

# actionbook/rust-skills — skill

**Why it's worth keeping:** It provides explicit multi-step reasoning chains (Workflows) that guide the agent through complex discovery tasks instead of just listing tools. It also defines highly structured output templates like implementation tables and hierarchy visualizations to ensure technical clarity.

**Summary:** A specialized protocol for navigating Rust trait implementations and hierarchies using LSP-driven workflows.

**Source credibility:** High; the repository is well-starred and recently active.

**Recency:** Current; uses standard LSP operation patterns compatible with modern coding agents.

**Source:** [actionbook/rust-skills/skills/rust-trait-explorer/SKILL.md](https://github.com/actionbook/rust-skills/blob/fa60f7931223646fb71c4586b4a6c8545016076a/skills/rust-trait-explorer/SKILL.md) · 1240★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rust-trait-explorer
description: "Explore Rust trait implementations using LSP. Triggers on: /trait-impl, find implementations, who implements, trait 实现, 谁实现了, 实现了哪些trait"
argument-hint: "<TraitName|StructName>"
allowed-tools: ["LSP", "Read", "Glob", "Grep"]
---

# Rust Trait Explorer

Discover trait implementations and understand polymorphic designs.

## Usage

```
/rust-trait-explorer <TraitName|StructName>
```

**Examples:**
- `/rust-trait-explorer Handler` - Find all implementors of Handler trait
- `/rust-trait-explorer MyStruct` - Find all traits implemented by MyStruct

## LSP Operations

### Go to Implementation

Find all implementations of a trait.

```
LSP(
  operation: "goToImplementation",
  filePath: "src/traits.rs",
  line: 10,
  character: 11
)
```

**Use when:**
- Trait name is known
- Want to find all implementors
- Understanding polymorphic code

## Workflow

### Find Trait Implementors

```
User: "Who implements the Handler trait?"
    │
    ▼
[1] Find trait definition
    LSP(goToDefinition) or workspaceSymbol
    │
    ▼
[2] Get implementations
    LSP(goToImplementation)
    │
    ▼
[3] For each impl, get details
    LSP(documentSymbol) for methods
```

</details>
