---
name: vicanso__zedis__skill
source: https://github.com/vicanso/zedis/blob/eae6c2f543d1f01a3754fdd91b11066f29c92c85/.claude/skills/gpui-entity/SKILL.md
repo: vicanso/zedis
kind: skill
stars: 1888
last_pushed: 2026-06-14T13:39:38Z
license: apache-2.0
score: 8
domains: [rust, gui, state-management]
tags: [gpui, rust, entity-pattern, concurrency]
curated: 2026-06-15
curated_by: config-scout
---

# vicanso/zedis — skill

**Why it's worth keeping:** It uses explicit 'Good vs Bad' code comparisons to teach an agent how to avoid specific pitfalls like retain cycles and nested update panics.

**Summary:** Provides comprehensive patterns for `Entity`-based state management within the GPUI framework used for high-performance UI.

**Source credibility:** High; derived from a highly-starred, actively maintained Rust/GPUI project (zedis).

**Recency:** Extremely current; the source repo was updated within the last month.

**Source:** [vicanso/zedis/.claude/skills/gpui-entity/SKILL.md](https://github.com/vicanso/zedis/blob/eae6c2f543d1f01a3754fdd91b11066f29c92c85/.claude/skills/gpui-entity/SKILL.md) · 1888★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: gpui-entity
description: Entity management and state handling in GPUI. Use when working with entities, managing component state, coordinating between components, handling async operations with state updates, or implementing reactive patterns. Entities provide safe concurrent access to application state.
---

## Overview

An `Entity<T>` is a handle to state of type `T`, providing safe access and updates.

**Key Methods:**
- `entity.read(cx)` → `&T` - Read-only access
- `entity.read_with(cx, |state, cx| ...)` → `R` - Read with closure
- `entity.update(cx, |state, cx| ...)` → `R` - Mutable update
- `entity.downgrade()` → `WeakEntity<T>` - Create weak reference
- `entity.entity_id()` → `EntityId` - Unique identifier

**Entity Types:**
- **`Entity<T>`**: Strong reference (increases ref count)
- **`WeakEntity<T>`**: Weak reference (doesn't prevent cleanup, returns `Result`)

## Quick Start

### Creating and Using Entities

```rust
// Create entity
let counter = cx.new(|cx| Counter { count: 0 });

// Read state
let count = counter.read(cx).count;

// Update state
counter.update(cx, |state, cx| {
    state.count += 1;
    cx.notify(); // Trigger re-render
});

// Weak reference (
```

</details>
