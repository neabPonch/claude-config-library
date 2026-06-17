---
name: oven-sh__bun__claude
source: https://github.com/oven-sh/bun/blob/2d8d5da90efea45290ce3fd209ca3b169f888f89/src/jsc/bindings/v8/CLAUDE.md
repo: oven-sh/bun
kind: claude-md
stars: 93187
last_pushed: 2026-06-15T05:05:21Z
license: other
score: 9
domains: [systems-programming, javascript-runtime, cpp, low-level]
tags: [v8, bindings, c++, bun, interop]
curated: 2026-06-15
curated_by: config-scout
---

# oven-sh/bun — claude-md

**Why it's worth keeping:** Contains highly specific, cross-platform command-line snippets for extracting mangled symbols (GCC/Clang vs. MSVC) which is critical for this complex task.

**Summary:** Provides exhaustive, low-level instructions for implementing V8 C++ API compatibility layers within Bun, covering implementation, symbol mangling, and testing.

**Source credibility:** High; source is the official Bun repository, a high-performance industry-standard runtime.

**Recency:** Current; the repository has active maintenance and recent commits.

**Source:** [oven-sh/bun/src/jsc/bindings/v8/CLAUDE.md](https://github.com/oven-sh/bun/blob/2d8d5da90efea45290ce3fd209ca3b169f888f89/src/jsc/bindings/v8/CLAUDE.md) · 93187★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# V8 C++ API Implementation Guide

This directory contains Bun's implementation of the V8 C++ API on top of JavaScriptCore. This allows native Node.js modules that use V8 APIs to work with Bun.

## Architecture Overview

Bun implements V8 APIs by creating a compatibility layer that:

- Maps V8's `Local<T>` handles to JSC's `JSValue` system
- Uses handle scopes to manage memory lifetimes similar to V8
- Provides V8-compatible object layouts that inline V8 functions can read
- Manages tagged pointers for efficient value representation

For detailed background, see the blog series:

- [Part 1: Introduction and challenges](https://bun.com/blog/how-bun-supports-v8-apis-without-using-v8-part-1.md)
- [Part 2: Memory layout and object representation](https://bun.com/blog/how-bun-supports-v8-apis-without-using-v8-part-2.md)
- [Part 3: Garbage collection and primitives](https://bun.com/blog/how-bun-supports-v8-apis-without-using-v8-part-3.md)

## Directory Structure

```
src/jsc/bindings/v8/
├── v8.h                    # Main header with V8_UNIMPLEMENTED macro
├── v8_*.h                  # V8 compatibility headers
├── V8*.h                   # V8 class headers (Number, String, Object, etc.)
```

</details>
