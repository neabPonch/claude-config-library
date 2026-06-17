---
name: Yeachan-Heo__clawhip
source: https://github.com/Yeachan-Heo/clawhip/blob/ff3ba32dc22a143d53bec40870d3b52b2fa11a2b/SKILL.md
repo: Yeachan-Heo/clawhip
kind: skill
stars: 912
last_pushed: 2026-06-13T15:08:14Z
license: mit
score: 8
domains: [cli-tools, agents-ai, devops]
tags: [daemon, notification-gateway, event-router]
curated: 2026-06-14
curated_by: config-scout
---

# Yeachan-Heo/clawhip — skill

**Why it's worth keeping:** It demonstrates a highly effective 'filesystem-offloaded memory' pattern and provides a structured CLI/config interface for managing event streams outside the LLM window.

**Summary:** A daemon-first notification gateway that routes system events (Git, GitHub, tmux) to Discord channels to prevent AI context pollution.

**Source credibility:** High; 900+ stars and active, recent maintenance suggest a stable and widely used toolset.

**Recency:** Current; utilizes modern developer tooling like 'gh' CLI and advanced tmux integration.

**Source:** [Yeachan-Heo/clawhip/SKILL.md](https://github.com/Yeachan-Heo/clawhip/blob/ff3ba32dc22a143d53bec40870d3b52b2fa11a2b/SKILL.md) · 912★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: clawhip
description: Attach/install/use clawhip as a daemon-first notification gateway runtime for OpenClaw / Clawdbot
---

# clawhip skill attachment surface

## Intent

Use this repo as:
- executable/runtime repo
- daemon process for Discord notification routing
- attachable skill surface for OpenClaw / Clawdbot

## Prerequisites

⭐ If you want to support clawhip, star this repository. The interactive repo-local installer and `clawhip install` can offer an optional post-install GitHub star prompt via authenticated `gh api` access when `gh` is installed and authenticated. Skip it with `--skip-star-prompt` or `CLAWHIP_SKIP_STAR_PROMPT=1`.

```bash
gh api --method PUT /user/starred/Yeachan-Heo/clawhip --silent
```

## Primary install flow

Preferred operator instruction:

```text
@openclaw install https://github.com/Yeachan-Heo/clawhip
```

Expected automation flow:

1. clone repo
2. run `./install.sh`
3. read this `SKILL.md`
4. attach skill
5. scaffold `~/.clawhip/config.toml`
6. start daemon
7. run live verification presets

## Runtime surface

Default daemon URL:

```text
http://127.0.0.1:25294
```

Core commands:

```bash
clawhip
clawhip start
clawhip status
clawhip co
```

</details>
