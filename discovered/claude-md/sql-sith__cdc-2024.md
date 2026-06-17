---
name: sql-sith__cdc-2024
source: https://github.com/sql-sith/cdc-2024/blob/50aa639b16e153ecc7dbf07757bf5a717948eb18/CLAUDE.md
repo: sql-sith/cdc-2024
kind: claude-md
stars: 3
last_pushed: 2026-04-20T15:01:59Z
license: mit
score: 8
domains: [cli-tools, security, education]
tags: [cryptography, python, shell-scripting, educational]
curated: 2026-06-15
curated_by: config-scout
---

# sql-sith/cdc-2024 — claude-md

**Why it's worth keeping:** Excellent 'Running Code' section with specific command examples and platform-specific dependency warnings; includes a high-level architecture overview that explains file variations.

**Summary:** Provides detailed execution instructions for various cryptographic and shell scripting exercises, including dependency nuances. It clarifies the intent behind multiple file variants to assist in understanding progression.

**Source credibility:** A niche educational repository for a cyber defense competition; highly structured due to its instructional nature.

**Recency:** Current; explicitly references Claude Code and modern Python environments.

**Source:** [sql-sith/cdc-2024/CLAUDE.md](https://github.com/sql-sith/cdc-2024/blob/50aa639b16e153ecc7dbf07757bf5a717948eb18/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Educational repository for the Cedar Rapids Area Homeschools IT Club's Cyber Defense competition (2023-2024 season). Contains cryptography implementations, shell scripting exercises, and meeting/homework documentation.

## Running Code

There is no build system — all scripts run directly.

### Diffie-Hellman (Python)

```bash
cd src/diffie_hellman

# Install dependencies (first time)
python -m pip install -r requirements.txt

# Interactive version (user supplies p, g, private keys)
python diffie_hellman.py

# Automated version with 2048-bit RFC 3526 primes (requires gmpy2)
python diffie_hellman_gmpy.py

# Refactored variants follow the same pattern
python diffie_hellman_refactored.py
python diffie_hellman_refactored_gmpy.py

# Object-oriented variant of the gmpy2 script
python diffie_hellman_gmpy_oo.py
```

`gmpy2>=2.2` is resolved from PyPI; pre-built wheels are available there for CPython 3.10–3.14 on Windows AMD64 and Linux x86_64. On platforms without a published wheel, pip will fall back to a source build, which requires the GMP, MPFR, and M
```

</details>
