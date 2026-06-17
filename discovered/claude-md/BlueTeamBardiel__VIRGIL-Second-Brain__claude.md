---
name: BlueTeamBardiel__VIRGIL-Second-Brain__claude
source: https://github.com/BlueTeamBardiel/VIRGIL-Second-Brain/blob/3f8d277542c1f3d12b6310b5e719114defb7aaae/.claude/CLAUDE.md
repo: BlueTeamBardiel/VIRGIL-Second-Brain
kind: claude-md
stars: 1
last_pushed: 2026-06-02T01:35:44Z
license: mit
score: 8
domains: [cli-tools, ux-writing, automation]
tags: [UX, CLI, Onboarding]
curated: 2026-06-15
curated_by: config-scout
---

# BlueTeamBardiel/VIRGIL-Second-Brain — claude-md

**Why it's worth keeping:** The 'Explanation -> Command -> Confirmation' pattern is a brilliant, highly transferable template for ensuring accessibility in automated tools and installers.

**Summary:** Establishes strict UX writing standards for CLI interactions, mandating plain-English explanations of jargon and consequences before any user prompt.

**Source credibility:** High-quality instructional writing despite the low star count/newness of the repo.

**Recency:** 

**Source:** [BlueTeamBardiel/VIRGIL-Second-Brain/.claude/CLAUDE.md](https://github.com/BlueTeamBardiel/VIRGIL-Second-Brain/blob/3f8d277542c1f3d12b6310b5e719114defb7aaae/.claude/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code — VIRGIL-Second-Brain (public)

Repo context: the public open-source release of VIRGIL. Users who land here
range from senior engineers to people who have never opened a terminal
before. The installer, ingest scripts, starter notes, and guided wizard all
run on strangers' machines. Assume **no technical knowledge**.

## Confirmation Prompt Style

When asking the user to confirm any command or parameter — and when writing
installer or script prompts the user will see — always include a one-line
Feynman explanation in plain English *before* the confirmation.

Format:
  1. "[What this does in plain English — one sentence, no jargon, grounded in consequence.]"
  2. Show the command or parameter.
  3. Ask for confirmation.

The rule: if the user would need to Google what something does, explain it
first. In a public-facing repo, that threshold is low. Acronyms like RSS,
CVE, NVD, API, vault, crontab, cron, AppImage, Ollama, and WSL all require
definition on first appearance inside a prompt.

### Examples

BAD:
"Install crontab schedules? [Y/n]"

GOOD:
"Cron is a tool that runs scripts on a schedule — like setting a recurring
alarm on your phone, but for commands. VIRGIL us
```

</details>
