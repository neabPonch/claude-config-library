---
name: usetero__edge
source: https://github.com/usetero/edge/blob/2567e8983a73069806476a1e4aef8fbe095f3a80/Claude.md
repo: usetero/edge
kind: claude-md
stars: 14
last_pushed: 2026-06-14T18:11:19Z
license: apache-2.0
score: 9
domains: [systems-programming, edge-computing]
tags: [zig, data-oriented-design, performance, memory-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# usetero/edge — claude-md

**Why it's worth keeping:** Uses 'Good vs Bad' comparative code examples and a pre-coding checklist to ensure adherence to cache-friendly architecture.

**Summary:** Enforces strict Data-Oriented Design (DoD) principles and memory optimization strategies for high-performance Zig development.

**Source credibility:** High; reflects specialized knowledge of low-level system design and modern Zig patterns.

**Recency:** 

**Source:** [usetero/edge/Claude.md](https://github.com/usetero/edge/blob/2567e8983a73069806476a1e4aef8fbe095f3a80/Claude.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Tero Edge - Project Overview

## Architecture

This is a Zig project implementing an edge computing runtime with a hybrid architectural approach:

- **Data-Oriented Design (DoD)**: Primary focus for performance-critical paths
- **Functional Programming**: For composability and testability
- **Object-Oriented Programming**: Where it provides clarity without sacrificing performance

## Data-Oriented Design Principles

### Core Philosophy
**The CPU is fast, but memory is slow.** All design decisions must optimize for memory access patterns and cache coherency.
**Predictable memory usage is the goal.** Each binary should have a predictable memory footprint based on throughput.

### Key Strategies

#### 1. Identify and Optimize Uniform Data
- Group similar data together in memory
- Minimize the size of each individual item
- Process data in bulk rather than one item at a time

#### 2. Use Indexes Instead of Pointers
```zig
// BAD: Pointer-heavy approach (64 bits per reference)
const Node = struct {
    data: Data,
    next: ?*Node,
    parent: ?*Node,
};

// GOOD: Index-based approach (typically 32 bits or less)
const NodeId = u32;
const Node = struct {
    data: Data,
    next: ?Node
```

</details>
