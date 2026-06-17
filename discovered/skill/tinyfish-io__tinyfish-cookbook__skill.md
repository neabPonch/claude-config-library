---
name: tinyfish-io__tinyfish-cookbook__skill
source: https://github.com/tinyfish-io/tinyfish-cookbook/blob/768ea6d9743b468630522717ecd1f3bdfcf9d8e2/plugins/tinyfish/skills/tunneling/SKILL.md
repo: tinyfish-io/tinyfish-cookbook
kind: skill
stars: 2039
last_pushed: 2026-06-13T00:51:25Z
license: mit
score: 8
domains: [cli-tools, web-development, agents-ai]
tags: [ssh, tunneling, webhooks, local-dev]
curated: 2026-06-15
curated_by: config-scout
---

# tinyfish-io/tinyfish-cookbook — skill

**Why it's worth keeping:** It includes specific 'Usage Guidelines' that instruct the agent on persona-driven behavior (asking for ports, running in background). It also provides a pre-flight check and keep-alive parameters to ensure connection stability.

**Summary:** Enables an agent to expose local development servers to the internet via SSH tunneling. This allows remote agents to access webhooks or local UI services.

**Source credibility:** High; high star count and active maintenance from a specialized web agent project.

**Recency:** Current; addresses the fundamental 'local-access' hurdle prevalent in modern AI coding workflows.

**Source:** [tinyfish-io/tinyfish-cookbook/plugins/tinyfish/skills/tunneling/SKILL.md](https://github.com/tinyfish-io/tinyfish-cookbook/blob/768ea6d9743b468630522717ecd1f3bdfcf9d8e2/plugins/tinyfish/skills/tunneling/SKILL.md) · 2039★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tunneling
description: Expose local ports to the internet as public HTTPS URLs using tinyfi.sh SSH tunnels. Use when you need to expose a locally running app, test webhooks, or give TinyFish access to a site that is only hosted locally — tunnel it first, then point TinyFish to the tunneled URL. No signup, no API key, no installation beyond SSH.
---

# TinyFish Tunneling (tinyfi.sh)

Create instant public HTTPS URLs for locally running apps via SSH tunneling. Free, no account, no installation beyond SSH.

## Pre-flight Check (REQUIRED)

```bash
which ssh && echo "SSH available" || echo "SSH not found — install OpenSSH first"
```

If SSH is not available, stop and tell the user to install OpenSSH.

---

## Quick Start

**Warning:** This exposes your local service to the public internet. Do not tunnel admin panels, debug endpoints, or services that expose secrets or credentials.

```bash
ssh -o StrictHostKeyChecking=accept-new -R 80:localhost:<PORT> tinyfi.sh
```

Replace `<PORT>` with the port your app is running on. The command prints a public `https://<random>.tinyfi.sh` URL.

> **Note:** `StrictHostKeyChecking=accept-new` automatically trusts the tinyfi.sh host key on fi
```

</details>
