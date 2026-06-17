---
name: SRombauts__SQLiteCpp__skill
source: https://github.com/SRombauts/SQLiteCpp/blob/d66a92a53dc4c333e8491584a8ca452dc058c977/.claude/skills/sqlitecpp-build-cmake/SKILL.md
repo: SRombauts/SQLiteCpp
kind: skill
stars: 2744
last_pushed: 2026-05-25T16:37:03Z
license: mit
score: 7
domains: [cpp, build-systems, database]
tags: [cmake, sqlite, build-instructions]
curated: 2026-06-16
curated_by: config-scout
---

# SRombauts/SQLiteCpp — skill

**Why it's worth keeping:** It explicitly maps complex CMake options to their functions and includes crucial setup steps like submodule initialization, which prevents agent errors during environment preparation.

**Summary:** Provides comprehensive CMake build instructions, configuration flags, and testing commands for the SQLiteCpp library.

**Source credibility:** High; the repository is well-starred (2.7k+) and actively maintained.

**Recency:** Very current; last pushed 1 month ago.

**Source:** [SRombauts/SQLiteCpp/.claude/skills/sqlitecpp-build-cmake/SKILL.md](https://github.com/SRombauts/SQLiteCpp/blob/d66a92a53dc4c333e8491584a8ca452dc058c977/.claude/skills/sqlitecpp-build-cmake/SKILL.md) · 2744★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sqlitecpp-build-cmake
description: Build SQLiteCpp with CMake. Use for CMake builds, tests, options, or build scripts.
---

# SQLiteCpp CMake Build

## Quick builds
- Windows (VS 2022):
  - `mkdir build`
  - `cd build`
  - `cmake -G "Visual Studio 17 2022" -DSQLITECPP_BUILD_TESTS=ON -DSQLITECPP_BUILD_EXAMPLES=ON ..`
  - `cmake --build . --config Release`
- Unix/macOS:
  - `mkdir build && cd build`
  - `cmake -DCMAKE_BUILD_TYPE=Debug -DSQLITECPP_BUILD_TESTS=ON -DSQLITECPP_BUILD_EXAMPLES=ON ..`
  - `cmake --build .`

## Build scripts
- `build.bat` (Windows) enables shared libs, tests, examples, and runs `ctest`.
- `build.sh` (Unix) enables ASAN, shared libs, tests, examples, and runs `ctest`.

## Common options
- `SQLITECPP_BUILD_TESTS` (OFF): build unit tests.
- `SQLITECPP_BUILD_EXAMPLES` (OFF): build examples.
- `BUILD_SHARED_LIBS` (OFF): build shared libs (DLLs).
- `SQLITECPP_INTERNAL_SQLITE` (ON): use bundled sqlite3 source.
- `SQLITE_ENABLE_COLUMN_METADATA` (ON): enable `getColumnOriginName()`.
- `SQLITECPP_RUN_CPPLINT` (ON): run cpplint target.
- `SQLITECPP_RUN_CPPCHECK` (ON): run cppcheck target.
- `SQLITECPP_RUN_DOXYGEN` (OFF): generate docs.
- `SQLITECPP_USE_ASAN`
```

</details>
