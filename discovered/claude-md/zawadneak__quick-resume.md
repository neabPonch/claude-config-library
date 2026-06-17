---
name: zawadneak__quick-resume
source: https://github.com/zawadneak/quick-resume/blob/4c2e94bd4389428b0544ae5829e59f967944c9d1/Claude.md
repo: zawadneak/quick-resume
kind: claude-md
stars: 0
last_pushed: 2026-03-01T14:18:15Z
license: unknown
score: 9
domains: [cli-tools, systems-programming, windows-dev, rust]
tags: [low-level, memory-management, win32]
curated: 2026-06-15
curated_by: config-scout
---

# zawadneak/quick-resume — claude-md

**Why it's worth keeping:** Excellent use of 'Key Design Decisions' to explain logic/tradeoffs and a detailed 'Workflow' section that provides algorithmic steps. The inclusion of 'Known Limitations' is top-tier as it prevents the AI from attempting impossible or out-of-scope tasks.

**Summary:** A high-density technical blueprint for a systems-level Rust project involving Windows API and memory manipulation.

**Source credibility:** Low social proof (0 stars), but the documentation depth indicates high technical sophistication in systems programming.

**Recency:** Highly current; provides the exact level of low-level context required for modern agentic coding.

**Source:** [zawadneak/quick-resume/Claude.md](https://github.com/zawadneak/quick-resume/blob/4c2e94bd4389428b0544ae5829e59f967944c9d1/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Quick Resume

Xbox-style Quick Resume for Windows — snapshot a running process's full state (memory + threads) to disk and restore it later from a cold launch.

## Project Overview

A Rust CLI tool that can freeze a running Windows process, dump its entire virtual memory and thread register contexts to a compressed file, and later restore that exact state into a freshly spawned process. The primary use case is games (tested with Mini Metro / Unity titles), enabling instant resume without the game's normal startup sequence.

## Architecture

```
src/
├── main.rs              # CLI entry point, orchestrates all commands
├── process/             # Attach to and inspect live processes
│   ├── attach.rs        # Find process by name via Toolhelp32, open with PROCESS_ALL_ACCESS
│   ├── info.rs          # Enumerate memory regions, threads, and loaded modules
│   └── suspend.rs       # RAII SuspendGuard using NtSuspendProcess/NtResumeProcess
├── snapshot/            # Capture process state
│   ├── memory.rs        # Walk VirtualQueryEx, ReadProcessMemory for all committed regions
│   ├── threads.rs       # GetThreadContext (CONTEXT_ALL) for every thread
│   └── writer.rs        # Seriali
```

</details>
