---
name: swoole__swoole-src
source: https://github.com/swoole/swoole-src/blob/31b469470fe4297321c0beb41475f54cf3bd9623/CLAUDE.md
repo: swoole/swoole-src
kind: claude-md
stars: 18887
last_pushed: 2026-06-08T09:45:18Z
license: apache-2.0
score: 9
domains: [backend, systems-programming, php, cpp]
tags: [low-level, high-performance, multi-language]
curated: 2026-06-15
curated_by: config-scout
---

# swoole/swoole-src — claude-md

**Why it's worth keeping:** The explicit distinction between the core C++ layer and the PHP extension layer, including specific CMake vs. phpize workflows, is a highly transferable pattern for complex multi-language projects. The inclusion of CI filter tags and platform-specific caveats provides critical context for debugging cross-platform issues.

**Summary:** This config provides a masterclass in explaining high-level architecture alongside granular build/test commands for a dual-layer (C++/PHP) project. It maps source directories directly to functional subsystems to prevent LLM confusion.

**Source credibility:** Extremely high; Swoole is a premier industry-standard concurrency engine with massive community adoption.

**Recency:** Current; the repo is actively maintained and includes modern features like io_uring support.

**Source:** [swoole/swoole-src/CLAUDE.md](https://github.com/swoole/swoole-src/blob/31b469470fe4297321c0beb41475f54cf3bd9623/CLAUDE.md) · 18887★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build & Test Commands

### Traditional PHP Extension Build (for production use)
```bash
phpize && ./configure [flags] && make -j$(nproc) && make install
```
Common configure flags: `--enable-sockets`, `--enable-mysqlnd`, `--enable-swoole-curl`, `--enable-cares`, `--enable-swoole-pgsql`, `--with-openssl-dir=DIR`, `--enable-swoole-thread`, `--enable-iouring`, `--enable-uring-socket`

### Developer Build (with ASAN + warnings)
```bash
phpize && ./configure --enable-swoole-dev --enable-debug-log --enable-sockets --enable-mysqlnd --enable-swoole-curl
```

### CMake Build (for core lib development without full PHP build)
```bash
mkdir -p build && cd build && cmake .. && make -j$(nproc)
```
This produces `lib/libswoole.so` (core library) and `core-tests` (Google Test binary for C++ tests).

Optional CMake flags: `-DCODE_COVERAGE=ON`, `-Denable_asan=ON`, `-Denable_thread=ON`, `-Dphp_dir=PATH`, `-Dopenssl_dir=PATH`

### Running Tests

**PHP tests** (phpt format, run from repo root):
```bash
# Run all tests
php run-tests.php tests/

# Run a single test
php run-tests.php tes
```

</details>
