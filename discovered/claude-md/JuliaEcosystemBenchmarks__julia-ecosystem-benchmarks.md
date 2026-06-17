---
name: JuliaEcosystemBenchmarks__julia-ecosystem-benchmarks
source: https://github.com/JuliaEcosystemBenchmarks/julia-ecosystem-benchmarks/blob/90b34924d914c8b2e5bbb28de593d5ed737facce/CLAUDE.md
repo: JuliaEcosystemBenchmarks/julia-ecosystem-benchmarks
kind: claude-md
stars: 1
last_pushed: 2026-06-15T16:02:11Z
license: unknown
score: 7
domains: [benchmarking, cli-tools, data-science]
tags: [julia, performance-testing, automation]
curated: 2026-06-15
curated_by: config-scout
---

# JuliaEcosystemBenchmarks/julia-ecosystem-benchmarks — claude-md

**Why it's worth keeping:** It explicitly maps out a multi-step operational workflow and provides exact command patterns needed to execute scripts within specific project environments.

**Summary:** Provides comprehensive execution context for Julia benchmarking, including environment variables, version management via juliaup, and data processing workflows.

**Source credibility:** High; represents a specialized, well-maintained technical benchmarking repository.

**Recency:** Current; reflects up-to-date toolchain usage (juliaup).

**Source:** [JuliaEcosystemBenchmarks/julia-ecosystem-benchmarks/CLAUDE.md](https://github.com/JuliaEcosystemBenchmarks/julia-ecosystem-benchmarks/blob/90b34924d914c8b2e5bbb28de593d5ed737facce/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Julia Ecosystem Benchmarks - Claude Context

## Repository Overview
This repository contains bash scripts for benchmarking various features of the Julia language ecosystem across different Julia versions and registry states. The benchmarks are designed to measure Time-To-First-X (TTFX) performance metrics.

## Key Scripts
- `run_all.sh`: Main orchestration script that runs benchmarks across multiple Julia versions
- `run_julia_ttfx_snippets.sh`: Runs TTFX benchmarks using the Julia-TTFX-Snippets repository
- `run_all_between_dates.sh`: Runs benchmarks for specific date ranges
- `timetravel_setup.sh`: Sets up registry time-travel functionality
- `hostdescription.sh`: Captures host system information

## Environment Variables
- `JEB_JULIA_VERSION`: Julia version being tested
- `JEB_REGISTRY_START_DATE` / `JEB_REGISTRY_END_DATE`: Registry date range
- `JEB_REGISTRY_DATE`: Specific registry date
- `JEB_HOSTNAME`: Host system identifier
- `JULIA_DEPOT_PATH`: Set to `$PWD/depot`
- `JULIA_PKG_PRECOMPILE_AUTO=0`: Disables automatic precompilation
- `JULIA_CI=true`: Enables CI mode
- `JULIA_NUM_THREADS=4`: Sets thread count

## Log Storage
- Benchmark results are stored in the `jeb_logs`
```

</details>
