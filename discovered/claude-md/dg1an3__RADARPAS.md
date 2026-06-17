---
name: dg1an3__RADARPAS
source: https://github.com/dg1an3/RADARPAS/blob/5ac0df791e90501651dd2c51667ae70e0267dd5a/CLAUDE.md
repo: dg1an3/RADARPAS
kind: claude-md
stars: 1
last_pushed: 2026-04-27T22:56:08Z
license: unknown
score: 8
domains: [legacy-systems, low-level]
tags: [historical-archive, knowledge-base, embedded]
curated: 2026-06-15
curated_by: config-scout
---

# dg1an3/RADARPAS — claude-md

**Why it's worth keeping:** It utilizes a semantic knowledge base (Prolog/RDF) pattern to help the agent navigate complex file relationships and provides critical hardware constraints for legacy code debugging.

**Summary:** Defines a multi-layered historical archive where directories represent software families and subdirectories represent chronological snapshots.

**Source credibility:** Highly specific personal/historical archive with deep domain expertise.

**Recency:** Current; reflects recent repository activity.

**Source:** [dg1an3/RADARPAS/CLAUDE.md](https://github.com/dg1an3/RADARPAS/blob/5ac0df791e90501651dd2c51667ae70e0267dd5a/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

Historical software archive (1984–2024) preserved as a synthetic git repository built from dated snapshots. The main project is **RADARPAS** — a radar terminal for the Ellason E300/E250 system, written by Derek G. Lane starting at age 15. The repo also contains EEVORG (cellular automata), SSM (spreadsheet engine), theWheel (spreading activation networks), and several other sub-projects.

Each top-level directory is a software family. Each dated subdirectory is a snapshot.

## Build Commands

```bash
# FreePascal build (compiles radar/radar.pas → radarpas executable)
make                # build
make run            # build and run
make clean          # remove .o, .ppu, radarpas

# Docker build (no local FPC required)
./build.sh          # automated: builds image + compiles
# Or manually:
docker build -t radarpas-fpc:latest .
docker run --rm -v "$(pwd):/build" radarpas-fpc:latest make
```

The modern `radar/radar.pas` is a FreePascal-compatible stub — it compiles but stubs out hardware (EGA, RS-232, interrupts). The historical originals (e.g., `radar/19
```

</details>
