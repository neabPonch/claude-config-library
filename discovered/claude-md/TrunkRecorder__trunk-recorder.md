---
name: TrunkRecorder__trunk-recorder
source: https://github.com/TrunkRecorder/trunk-recorder/blob/26b8ff30fcada2bf38462e6d0e4bc661fd25d294/CLAUDE.md
repo: TrunkRecorder/trunk-recorder
kind: claude-md
stars: 1104
last_pushed: 2026-06-14T03:31:26Z
license: gpl-3.0
score: 10
domains: [C++, cli-tools, signal-processing]
tags: [cpp, build-system, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# TrunkRecorder/trunk-recorder — claude-md

**Why it's worth keeping:** It includes highly specific 'negative constraints' (like avoiding -ffast-math) that prevent logic errors in signal processing, and uses a source layout table to facilitate navigation.

**Summary:** This file provides deep technical context for a complex C++ project, including architectural flow and specific compiler flag requirements.

**Source credibility:** High: popular repository with active maintenance and clear ownership of technical details.

**Recency:** Current; provides context highly relevant to modern agentic coding workflows.

**Source:** [TrunkRecorder/trunk-recorder/CLAUDE.md](https://github.com/TrunkRecorder/trunk-recorder/blob/26b8ff30fcada2bf38462e6d0e4bc661fd25d294/CLAUDE.md) · 1104★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Notes for Claude Code when working in this repository. Keep changes minimal and idiomatic to what is already here — this is a long-lived C++ project with a lot of historical conventions baked into the structure.

## What this project is

Trunk Recorder is a C++ application that uses GNU Radio + OP25 to record voice calls from trunked (P25, SmartNet) and conventional (P25, DMR, analog) radio systems via SDRs. It is a single binary (`trunk-recorder`) plus a set of loadable plugin shared libraries.

The high-level pipeline is in [trunk-recorder/main.cc](trunk-recorder/main.cc):

```
load_config -> start_plugins -> setup_systems -> monitor_messages
```

The `tb` (`gr::top_block_sptr`) is the GNU Radio flow graph that runs while `monitor_messages()` polls queues, manages calls, and drives plugins.

## Build and run

There is no in-tree test suite or linter target. The standard build is:

```bash
mkdir -p build && cd build
cmake ../
make -j$(nproc)
```

For debugging crashes, use `cmake -DCMAKE_BUILD_TYPE=Debug ../` — see [docs/DEBUG.md](docs/DEBUG.md).

The binary expects a config file at `./config.json` by default; override with `-c`:

```bash
./build/trunk-recorder -c /pa
```

</details>
