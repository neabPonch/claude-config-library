---
name: digego__extempore
source: https://github.com/digego/extempore/blob/8ff862c87ba9a2157cc6b6ba17c7dee009bd94f5/CLAUDE.md
repo: digego/extempore
kind: claude-md
stars: 1461
last_pushed: 2026-06-10T11:36:28Z
license: unknown
score: 9
domains: [systems-programming, cli-tools]
tags: [cmake, llvm, c++, scheme]
curated: 2026-06-15
curated_by: config-scout
---

# digego/extempore — claude-md

**Why it's worth keeping:** Includes highly specific details like exact `ctest` labels, internal LLVM header paths, and nuanced CLI flag combinations (e.g., `--batch` vs `--noaudio`) that prevent environment errors.

**Summary:** A high-density technical guide covering complex build/test workflows, LLVM dependency management, and execution modes.

**Source credibility:** Highly credible; a popular specialized project with 1400+ stars and active maintenance.

**Recency:** Current; utilizes modern C++20 and recent LLVM versions.

**Source:** [digego/extempore/CLAUDE.md](https://github.com/digego/extempore/blob/8ff862c87ba9a2157cc6b6ba17c7dee009bd94f5/CLAUDE.md) · 1461★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Extempore

Live coding environment for music, audio, and graphics. Scheme interpreter with
xtlang---a statically-typed lisp that compiles to LLVM IR at runtime.

## Build

```bash
mkdir build && cd build
cmake ..
cmake --build . -j$(nproc)
```

Key options: `-DASSETS=ON` (download multimedia assets), `-DBUILD_TESTS=ON`
(default).

### LLVM dependency

LLVM is fetched and built automatically via CMake's `FetchContent`. The version
is pinned in `CMakeLists.txt` (currently 22.x). On first build, CMake downloads
the LLVM source tarball and builds only the required components (OrcJIT, target
codegen, AsmParser, Passes, MCDisassembler, IRPrinter).

After configuration, LLVM sources and build artifacts are in:

- `build/_deps/llvm-src/` --- LLVM source tree
- `build/_deps/llvm-build/` --- LLVM build outputs (libraries, generated
  headers)

The LLVM headers used by extempore come from two locations:

- `build/_deps/llvm-src/llvm/include/` --- static headers from source
- `build/_deps/llvm-build/include/` --- generated headers (e.g. `llvm/Config/`)

The first LLVM build takes significant time (~10-30 min depending on hardware).
Subsequent builds reuse the cached LLVM artifacts. The GitHu
```

</details>
