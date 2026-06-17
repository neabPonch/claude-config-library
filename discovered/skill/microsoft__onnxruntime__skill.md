---
name: microsoft__onnxruntime__skill
source: https://github.com/microsoft/onnxruntime/blob/bf7e27a44ee1310fa248430e463ea09f3051a565/.agents/skills/ort-build/SKILL.md
repo: microsoft/onnxruntime
kind: skill
stars: 20822
last_pushed: 2026-06-15T01:38:37Z
license: mit
score: 9
domains: [ml-ops, cli-tools, cpp]
tags: [build-system, onnxruntime, cmake]
curated: 2026-06-15
curated_by: config-scout
---

# microsoft/onnxruntime — skill

**Why it's worth keeping:** The 'Agent tips' section provides critical operational intelligence, such as directing output to files to avoid buffer overflows and handling shell-specific redirection issues.

**Summary:** A specialized skill file for building ONNX Runtime that distinguishes between build phases to optimize execution time.

**Source credibility:** High; sourced from a massive, highly-starred Microsoft repository used globally for ML inference.

**Recency:** Very current; addresses specific agentic workflows like polling long-running builds and environment activation.

**Source:** [microsoft/onnxruntime/.agents/skills/ort-build/SKILL.md](https://github.com/microsoft/onnxruntime/blob/bf7e27a44ee1310fa248430e463ea09f3051a565/.agents/skills/ort-build/SKILL.md) · 20822★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ort-build
description: Build ONNX Runtime from source. Use this skill when asked to build, compile, or generate CMake files for ONNX Runtime.
---

# Building ONNX Runtime

The build scripts `build.sh` (Linux/macOS) and `build.bat` (Windows) delegate to `tools/ci_build/build.py`.

## Build phases

Three phases, controlled by flags:

- `--update` — generate CMake build files
- `--build` — compile (add `--parallel` to speed this up)
- `--test` — run tests

For native builds, if none are specified (and `--skip_tests` is not passed), **all three run by default**. For cross-compiled builds, the default is `--update` + `--build` only.

### When to use `--update`

You need `--update` when:
- First build in a new build directory
- New source files are added (some CMake targets use glob patterns, others use explicit file lists — re-run to pick up new files either way)
- CMake configuration changes (new flags, updated CMakeLists.txt)

You do **not** need `--update` when only modifying existing `.cc`/`.h` files — just use `--build`. Skipping it saves time.

## Examples

```bash
# Full build (update + build + test)
./build.sh --config Release --parallel
.\build.bat --config Release --
```

</details>
