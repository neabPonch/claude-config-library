---
name: RediSearch__RediSearch__skill
source: https://github.com/RediSearch/RediSearch/blob/7ef821158b5b6e93b8f4f85c874980356707cb26/.skills/lint/SKILL.md
repo: RediSearch/RediSearch
kind: skill
stars: 6156
last_pushed: 2026-06-15T17:33:31Z
license: other
score: 8
domains: [systems-programming, cli-tools]
tags: [linting, c, rust, polyglot]
curated: 2026-06-15
curated_by: config-scout
---

# RediSearch/RediSearch — skill

**Why it's worth keeping:** Uses the pattern of providing both verification and auto-fix commands; includes high-value semantic advice like '// SAFETY:' documentation patterns.

**Summary:** Provides a robust polyglot linting workflow covering both C and Rust components with clear check-and-fix instructions.

**Source credibility:** Highly credible; RediSearch is a high-star, actively maintained systems project.

**Recency:** Current; uses modern toolchain commands for Rust and C development.

**Source:** [RediSearch/RediSearch/.skills/lint/SKILL.md](https://github.com/RediSearch/RediSearch/blob/7ef821158b5b6e93b8f4f85c874980356707cb26/.skills/lint/SKILL.md) · 6156★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: lint
description: Check code quality and formatting before committing changes. Use this to verify your changes meet our coding standards.
---

# Lint Skill

Check code quality and formatting before committing changes.

## Usage
Run this skill to check for lint errors and formatting issues.

## Instructions

### C Code

1. Check C/C++ formatting against `.clang-format`:
   ```bash
   clang-format --dry-run -Werror <modified .c and .h files>
   ```

2. If formatting check fails, apply formatting:
   ```bash
   clang-format -i <modified .c and .h files>
   ```

3. Verify the project compiles without warnings-as-errors:
   ```bash
   ./build.sh
   ```
   The CMake build promotes key warnings to errors (`-Werror=incompatible-pointer-types`,
   `-Werror=implicit-function-declaration`). A successful build confirms these pass.

### Rust Code

1. Run the lint check:
   ```bash
   make lint
   ```

2. If clippy reports warnings or errors, fix them before proceeding

3. Check formatting:
   ```bash
   make fmt CHECK=1
   ```

4. If formatting check fails, apply formatting:
   ```bash
   make fmt
   ```

5. If license headers are missing, add them:
   ```bash
   (cd src/redisearch_rs
```

</details>
