---
name: synapticore-io__astro-duck
source: https://github.com/synapticore-io/astro-duck/blob/c66f461e2103b54949082c19641412875300bb76/CLAUDE.md
repo: synapticore-io/astro-duck
kind: claude-md
stars: 1
last_pushed: 2026-05-19T12:22:23Z
license: mit
score: 8
domains: [cli-tools, data-engineering, systems-programming]
tags: [duckdb, cpp, extension-development]
curated: 2026-06-14
curated_by: config-scout
---

# synapticore-io/astro-duck — claude-md

**Why it's worth keeping:** The 'Adding New Functions' procedural workflow is perfect for LLM instruction; the 'Testing Gotchas' preemptively solves common C++/DuckDB integration errors.

**Summary:** Provides clear build/test workflows, architectural structure, and a step-by-step guide for adding new functions. Includes critical environment-specific 'gotchas' regarding extension loading.

**Source credibility:** Low star count, but documentation shows high technical density and clear maintenance patterns.

**Recency:** Current, with activity within the last month.

**Source:** [synapticore-io/astro-duck/CLAUDE.md](https://github.com/synapticore-io/astro-duck/blob/c66f461e2103b54949082c19641412875300bb76/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Astro DuckDB Extension

DuckDB extension for astronomical calculations (coordinate transforms, angular separation, photometry, cosmology).

## Commands

```bash
# Build
make release              # Release build (outputs to build/release/)
make debug                # Debug build
make clean                # Clean build artifacts

# Test
python test_astro.py      # Run Python test suite
```

## Architecture

```
src/
  astro.cpp               # All function implementations (59 functions)
  include/
    astro_extension.hpp   # Extension registration
test/
  sql/astro.test          # SQL test cases
test_astro.py             # Python integration tests
extension-ci-tools/       # DuckDB CI tooling (submodule)
duckdb/                   # DuckDB source (submodule)
```

## Key Files

- `extension_config.cmake` - Extension configuration for DuckDB build system
- `CMakeLists.txt` - CMake configuration
- `.github/workflows/MainDistributionPipeline.yml` - Main CI workflow

## Build Output

Extension binary: `build/release/extension/astro/astro.duckdb_extension`

## Testing Gotchas

- Tests use `duckdb -unsigned` flag to load unsigned extensions
- Extension must be loaded with full absolute pat
```

</details>
