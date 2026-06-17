---
name: daymade__claude-code-skills__skill
source: https://github.com/daymade/claude-code-skills/blob/dde45c2105516aa703667ea8d21dd85cd3b6ec1e/cli-demo-generator/SKILL.md
repo: daymade/claude-code-skills
kind: skill
stars: 1187
last_pushed: 2026-06-14T10:01:47Z
license: mit
score: 9
domains: [cli-tools, documentation]
tags: [vhs, demo-generation, automation]
curated: 2026-06-16
curated_by: config-scout
---

# daymade/claude-code-skills — skill

**Why it's worth keeping:** Includes highly specific expert techniques like base64 encoding to bypass VHS parser limitations and the 'Hide/clear/Show' pattern to prevent setup leakage.

**Summary:** Provides a professional workflow for generating high-quality, animated CLI demos using VHS with support for automated generation and self-cleaning environments.

**Source credibility:** High; repository is well-starred and shows recent, active maintenance.

**Recency:** Current; integrates modern terminal recording workflows.

**Source:** [daymade/claude-code-skills/cli-demo-generator/SKILL.md](https://github.com/daymade/claude-code-skills/blob/dde45c2105516aa703667ea8d21dd85cd3b6ec1e/cli-demo-generator/SKILL.md) · 1187★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cli-demo-generator
description: Generates professional animated CLI demos as GIFs using VHS terminal recordings. Handles tape file creation, self-bootstrapping demos with hidden setup, output noise filtering, post-processing speed-up, and frame-level verification. Use when users want to create terminal demos, record CLI workflows as GIFs, generate animated documentation, build demo tapes for README files, or need to showcase any command-line tool visually. Also triggers on "record terminal", "VHS tape", "demo GIF", "animate my CLI", or any request to visually demonstrate shell commands.
---

# CLI Demo Generator

Create professional animated CLI demos. Four approaches, from fully automated to pixel-precise manual control.

## Quick Start

**Simplest path** — give commands, get GIF:

```bash
python3 ${CLAUDE_SKILL_DIR}/scripts/auto_generate_demo.py \
  -c "npm install my-package" \
  -c "npm run build" \
  -o demo.gif
```

**Self-bootstrapping demo** — for repeatable recordings that clean their own state:

```bash
python3 ${CLAUDE_SKILL_DIR}/scripts/auto_generate_demo.py \
  -c "npm install my-package" \
  -c "npm run build" \
  -o demo.gif \
  --bootstrap "npm uninstall m
```

</details>
