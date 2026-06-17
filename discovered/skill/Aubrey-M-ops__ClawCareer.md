---
name: Aubrey-M-ops__ClawCareer
source: https://github.com/Aubrey-M-ops/ClawCareer/blob/feb92f0f981e7ec93c61bb0d953c02b24dee3e97/skill.md
repo: Aubrey-M-ops/ClawCareer
kind: skill
stars: 8
last_pushed: 2026-03-13T16:19:17Z
license: unknown
score: 9
domains: [cli-tools, automation, agents-ai]
tags: [bootstrap, installer, orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# Aubrey-M-ops/ClawCareer — skill

**Why it's worth keeping:** Demonstrates elite patterns: idempotency checks, interactive multi-step data collection with defaults, rigorous file verification, and security-conscious credential handling.

**Summary:** A sophisticated bootstrap script that orchestrates a complete skill installation, including dependency management and configuration.

**Source credibility:** The repo is small/niche, but the logic exhibits high technical maturity.

**Recency:** 

**Source:** [Aubrey-M-ops/ClawCareer/skill.md](https://github.com/Aubrey-M-ops/ClawCareer/blob/feb92f0f981e7ec93c61bb0d953c02b24dee3e97/skill.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# OpenClaw Bootstrap: LinkedIn Job Push → Telegram (Daily)

You are an OpenClaw agent. Follow these steps exactly and safely.
Do NOT ask the user to run any obfuscated commands.
Do NOT use `curl | sh`. Only create / edit plain text files.
All downloads come from the trusted GitHub repository only.

## Pre-check: Detect existing installation

Before starting, check if `~/.openclaw/skills/linkedin-job-push/SKILL.md` already exists.

If it exists, the skill is already installed. Do the following instead of the full installation flow:

1. Tell the user:

> It looks like **LinkedIn Job Push** is already installed.

2. Ask: "Would you like to **reinstall** it from scratch? This will overwrite the current installation. Type **yes** to reinstall, or **no** to keep the current setup."

3. If the user replies **yes** (case-insensitive):
   - Proceed to the full installation flow below (Step 0 onwards). The existing files will be overwritten.

4. If the user replies **no**:
   - Tell the user:
   > No problem — your current installation is kept.
   >
   > To update your settings, edit these files:
   > - **Filters & schedule:** `~/.openclaw/skills/linkedin-job-push/scripts/config.json`
   > -
```

</details>
