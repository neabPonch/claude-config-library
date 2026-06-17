---
name: control-theory__gonzo__skill
source: https://github.com/control-theory/gonzo/blob/ce151a927dba2dfa6fa90583fa0b9c5ffde565e6/skills/gonzo/SKILL.md
repo: control-theory/gonzo
kind: skill
stars: 2683
last_pushed: 2026-06-09T00:00:54Z
license: mit
score: 9
domains: [cli-tools, devops, observability]
tags: [logs, automation, environment-detection, troubleshooting]
curated: 2026-06-15
curated_by: config-scout
---

# control-theory/gonzo — skill

**Why it's worth keeping:** The two-pass detection logic (project vs. user-level credentials) and the explicit instruction to avoid executing TUI commands in a non-interactive shell are exceptional edge-case mitigations.

**Summary:** A high-precision workflow for an agent to detect deployment environments and configure real-time log analysis pipelines using Gonzo.

**Source credibility:** High; source repository is well-starred, active, and provides highly specific integration guides.

**Recency:** Current; specifically accounts for modern 'claude-code' AI provider integrations.

**Source:** [control-theory/gonzo/skills/gonzo/SKILL.md](https://github.com/control-theory/gonzo/blob/ce151a927dba2dfa6fa90583fa0b9c5ffde565e6/skills/gonzo/SKILL.md) · 2683★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: gonzo
description: >
  Set up and use Gonzo, the open-source terminal log analysis tool. Use when
  the user wants to tail, watch, stream, or analyze logs. Detects deployment
  platforms, generates pipe commands, and configures AI analysis.
---

# Gonzo — Terminal Log Analysis Skill

Gonzo is an open-source TUI for real-time log tailing, filtering, and AI-powered
analysis in the terminal — patterns, heatmaps, anomaly detection, and more.
It works with any log source that can pipe to stdout. No account required —
fully open source.

**Repo:** https://github.com/control-theory/gonzo
**Docs:** https://docs.controltheory.com

---

## Quick start

When the user says "tail my logs", "watch my logs", or wants to see logs:

1. Detect platform → 2. Install Gonzo if needed → 3. Configure AI →
4. Generate command → 5. Run it.

---

## Setup flow

### 1. Detect deployment platform(s) — two passes

Detection has two layers. **Always run both passes and combine results
before deciding.** A common failure is detecting only project files and
missing platforms configured at the user level (AWS credentials,
kubeconfig).

#### Pass 1: Project-level signal files

Scan from cwd, walking up to
```

</details>
