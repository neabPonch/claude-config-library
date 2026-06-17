---
name: ryoppippi__zigcv
source: https://github.com/ryoppippi/zigcv/blob/1d8a3dee507ecee7fd3f73cab4bc4f5c9fcf35b4/CLAUDE.md
repo: ryoppippi/zigcv
kind: claude-md
stars: 162
last_pushed: 2026-06-05T16:59:37Z
license: mit
score: 9
domains: [systems-programming, computer-vision]
tags: [zig, opencv, bindings]
curated: 2026-06-15
curated_by: config-scout
---

# ryoppippi/zigcv — claude-md

**Why it's worth keeping:** Uses explicit 'Key Patterns' with code examples to enforce idiomatic code generation and provides clear setup steps for ML model dependencies.

**Summary:** Provides build/test commands, project architecture, and specific coding patterns for Zig-OpenCV bindings.

**Source credibility:** High-quality repository with active maintenance and significant star count for a niche binding library.

**Recency:** Very current; addresses specific Zig versioning and modern development workflows like devenv.

**Source:** [ryoppippi/zigcv/CLAUDE.md](https://github.com/ryoppippi/zigcv/blob/1d8a3dee507ecee7fd3f73cab4bc4f5c9fcf35b4/CLAUDE.md) · 162★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ZIGCV is a Zig language binding library for OpenCV 4. It provides Zig developers with access to computer vision functionality through idiomatic Zig APIs while wrapping the GoCV C++ interface.

## Essential Commands

### Building
```bash
# Build the library
zig build

# Build all examples
zig build examples

# Build and run a specific example
zig build showimage
zig build facedetect
```

### Testing
```bash
# Run all tests
zig build test

# Download required ML models for tests (required before running tests)
devenv shell -- download-models
```

### Development with devenv
```bash
# Enter devenv shell
devenv shell

# Build using devenv (inside the shell)
build

# Run tests (inside the shell)
test
```

## Architecture

The codebase follows a modular structure mirroring OpenCV's organization:

1. **Core Bindings** (`src/c_api.zig`): Direct C bindings to the GoCV wrapper
2. **Module Files** (`src/*.zig`): Each OpenCV module has a corresponding Zig file that wraps C APIs with idiomatic Zig interfaces
3. **Main Export** (`src/main.zig`): Central entry
```

</details>
