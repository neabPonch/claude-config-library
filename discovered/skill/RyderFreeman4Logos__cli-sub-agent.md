---
name: RyderFreeman4Logos__cli-sub-agent
source: https://github.com/RyderFreeman4Logos/cli-sub-agent/blob/4c4ce2a7ca2e391341ef8be9b3806a8858754dbc/skill.md
repo: RyderFreeman4Logos/cli-sub-agent
kind: skill
stars: 12
last_pushed: 2026-06-14T23:48:50Z
license: apache-2.0
score: 7
domains: [agents-ai, cli-tools, devops]
tags: [workflow-orchestration, skill-compilation, agent-infrastructure]
curated: 2026-06-15
curated_by: config-scout
---

# RyderFreeman4Logos/cli-sub-agent — skill

**Why it's worth keeping:** Introduces the advanced concept of 'companion skills' and using a compiler (weave) to transform high-level patterns into structured tool configurations.

**Summary:** A technical installation and orchestration guide for a pattern-based skill management framework designed for AI agents.

**Source credibility:** Niche developer project with highly specialized, technical documentation structure.

**Recency:** Very current; aligns with modern AI coding workflows and utilizes modern toolchains like mise.

**Source:** [RyderFreeman4Logos/cli-sub-agent/skill.md](https://github.com/RyderFreeman4Logos/cli-sub-agent/blob/4c4ce2a7ca2e391341ef8be9b3806a8858754dbc/skill.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name = "csa-setup"
version = "0.1.0"
description = "Install CSA, Weave, and coding workflow patterns for AI agent bots"
homepage = "https://github.com/RyderFreeman4Logos/cli-sub-agent"
target = "agent-bots"
---

# CSA Setup

> Installation guide for AI agent bots (openclaw, Moltis, etc.) to set up
> CSA and Weave with optional coding workflow patterns.

## Skill Files

| File | Description |
|------|-------------|
| **skill.md** (this file) | Installation and setup guide |
| **skills/AGENTS.md** | Full skill & pattern catalog |
| **README.md** | Project documentation |

---

## Prerequisites

Before starting, verify these tools are available:

```bash
# Required
git --version          # Git 2.30+
cargo --version        # Rust toolchain (only needed for building from source)

# Optional but recommended
mise --version         # Cross-platform tool version manager
gh --version           # GitHub CLI (for PR workflows)
```

If `mise` is not installed (see [mise.jdx.dev/installing](https://mise.jdx.dev/installing-mise.html) for alternatives):

```bash
# Verify domain before piping to shell
curl https://mise.run | sh
```

If `cargo` is not installed (see [rustup.rs](https://rustup.rs
```

</details>
