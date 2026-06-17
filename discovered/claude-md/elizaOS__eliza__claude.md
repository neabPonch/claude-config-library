---
name: elizaOS__eliza__claude
source: https://github.com/elizaOS/eliza/blob/0250bfb980773163ae408a606fda100dd2f0e895/packages/chip/CLAUDE.md
repo: elizaOS/eliza
kind: claude-md
stars: 18587
last_pushed: 2026-06-14T21:48:59Z
license: mit
score: 9
domains: [hardware-engineering, embedded-systems, semiconductors]
tags: [risc-v, soc, production-grade, verification-driven]
curated: 2026-06-15
curated_by: config-scout
---

# elizaOS/eliza — claude-md

**Why it's worth keeping:** The 'Validation' section provides explicit make targets tied to specific change types, enabling the AI to self-verify its work. The 'Conventions' section uses high-authority language like 'fail closed' and 'no slop' to prevent low-quality or incomplete contributions.

**Summary:** Establishes rigorous, production-grade engineering standards for high-stakes hardware and software co-design. It integrates RTL, firmware, and physical design workflows with strict integrity constraints.

**Source credibility:** High; from the highly-starred, actively maintained ElizaOS repository.

**Recency:** Current; reflects modern high-performance engineering and toolchain management.

**Source:** [elizaOS/eliza/packages/chip/CLAUDE.md](https://github.com/elizaOS/eliza/blob/0250bfb980773163ae408a606fda100dd2f0e895/packages/chip/CLAUDE.md) · 18587★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# packages/chip — Eliza E1 RISC-V AI SoC

Pre-tapeout hardware/software **evidence package** for the Eliza E1 RISC-V AI
SoC scaffold. Treat every change as production-grade engineering work intended
for eventual publication — this directory should read like a publishable
artifact, not a work log. (No `package.json`; driven entirely by `make` and the
`tools/`, `scripts/`, and `external/` toolchain.)

## Native over Docker on Linux x64

The full PD / RTL / sim / formal toolchain is installed and supported
**natively** on Linux x86_64. `tools/env.sh` puts the local binaries first on
`PATH` — Verilator, Icarus, Yosys, SymbiYosys, z3, OpenROAD, OpenLane, magic,
klayout, netgen, QEMU, Renode, KiCad, OpenOCD, sigrok, the RISC-V cross
toolchains — sourced from `external/oss-cad-suite/`, `external/deb-tools/`,
`external/openlane2/.venv/`, and `external/openroad/`. Run flows directly on the
host; native is faster, gives real stack traces, and avoids docker-daemon
babysitting. The `run_openlane.sh` / `run_openroad.sh` wrappers already prefer
the native binary and fall back to Docker only when none is on `PATH`. Docker is
retained only as a documented fallback for macOS reproduction or pinned-
```

</details>
