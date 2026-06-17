---
name: marvinrichter__clarc__skill
source: https://github.com/marvinrichter/clarc/blob/a8355b036a977300dfce1758af1c0d7e3371a26b/skills/c-testing/SKILL.md
repo: marvinrichter/clarc
kind: skill
stars: 10
last_pushed: 2026-04-27T07:59:08Z
license: mit
score: 9
domains: [systems-programming, c-language, testing]
tags: [c, unit-testing, memory-safety, cmake]
curated: 2026-06-15
curated_by: config-scout
---

# marvinrichter/clarc — skill

**Why it's worth keeping:** The inclusion of specific '--wrap' linker flag instructions for mocking and the ASan vs. Valgrind strategy makes it a highly practical guide for agents.

**Summary:** Provides production-grade C testing patterns including Unity unit tests, CMocka function mocking via linker wraps, and memory safety workflows using ASan/Valgrind.

**Source credibility:** High-quality engineering content from a recent repository focused on production workflows.

**Recency:** 

**Source:** [marvinrichter/clarc/skills/c-testing/SKILL.md](https://github.com/marvinrichter/clarc/blob/a8355b036a977300dfce1758af1c0d7e3371a26b/skills/c-testing/SKILL.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: c-testing
description: "C testing patterns: Unity framework (TEST_ASSERT_*), CMocka mocking with __wrap_ and linker flag, Valgrind leak checking, AddressSanitizer, CMake CTest integration, test organization, and running tests with sanitizers. Use when writing or reviewing C tests."
---

# C Testing

## When to Activate

- Writing C unit tests with Unity or CMocka
- Setting up CMake CTest integration
- Running tests with AddressSanitizer or Valgrind
- Mocking C functions for isolation testing
- Adding test coverage to a C library that currently has no automated tests and needs to be validated before a release
- Replacing a slow Valgrind CI step with a fast AddressSanitizer build that catches the same heap and stack errors
- Isolating a C module that calls a network or filesystem function by wrapping it with CMocka `__wrap_` mocks
- Wiring CTest into a CMake build so `cmake --build build && ctest` gives a single pass/fail result in CI

---

## Unity — Minimal Unit Testing

Unity is a single-file C test framework — no dependencies.

```c
/* tests/test_queue.c */
#include "unity.h"
#include "queue.h"

void setUp(void)    { /* called before each test */ }
void tearDown(void) {
```

</details>
