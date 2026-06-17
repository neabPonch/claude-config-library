---
name: wmacevoy__spider-cipher
source: https://github.com/wmacevoy/spider-cipher/blob/11db68562357af6f8b36f620afd6269341c3e417/CLAUDE.md
repo: wmacevoy/spider-cipher
kind: claude-md
stars: 0
last_pushed: 2026-06-14T05:00:13Z
license: mit
score: 9
domains: [security, cli-tools, cryptography]
tags: [build-instructions, security-constraints, system-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# wmacevoy/spider-cipher — claude-md

**Why it's worth keeping:** The 'Architecture' section uses proactive constraints (warning against 'obvious' optimizations to preserve constant-time properties) and provides specific resource requirements for long-running tests. It also establishes a domain-specific lexicon to ensure AI consistency.

**Summary:** Provides exhaustive build/test instructions for multi-language implementations and explains a complex cryptographic state machine. It includes vital security warnings regarding side-channel resistance.

**Source credibility:** High-density technical documentation characteristic of a specialized security/math project, despite low GitHub star counts.

**Recency:** 

**Source:** [wmacevoy/spider-cipher/CLAUDE.md](https://github.com/wmacevoy/spider-cipher/blob/11db68562357af6f8b36f620afd6269341c3e417/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

The Spider Cipher is a manual encryption scheme operated with a 40-card deck (values 0–39, mod-40 "base40" arithmetic). This repo holds several implementations of the cipher (C reference, minimal C core, C++ headers, Verilog hardware RNG, JS browser demo), tooling for the physical artifacts (card SVGs, 3D-printed dice), and the academic papers describing it.

## Build & test

### Reference C implementation (root `Makefile`, `src/`, `include/`)

**Requires sibling repos checked out next to this repo**: `../facts`, `../utf8`, `../cio` (github.com/wmacevoy/{facts,utf8,cio}). The Makefile includes their headers and compiles their sources directly; CI (`.github/workflows/c-cpp.yml`) checks them out the same way.

```sh
make all          # builds bin/spider_cipher (CLI) and bin/spider_cipher_facts (tests)
make check        # runs facts tests against expected/ and round-trips encrypt/decrypt in all 3 formats
make expected     # regenerates expected/ outputs (only when output changes are intentional)
```

Tests use the `facts` framework (test registry in `sr
```

</details>
