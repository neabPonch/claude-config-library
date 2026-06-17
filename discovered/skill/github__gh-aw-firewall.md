---
name: github__gh-aw-firewall
source: https://github.com/github/gh-aw-firewall/blob/e0c118bc360c3bfaec2ef8ad62735c0992131084/skill.md
repo: github/gh-aw-firewall
kind: skill
stars: 93
last_pushed: 2026-06-14T19:51:24Z
license: mit
score: 9
domains: [security, agents-ai, cli-tools]
tags: [network-isolation, sandboxing, egress-control]
curated: 2026-06-15
curated_by: config-scout
---

# github/gh-aw-firewall — skill

**Why it's worth keeping:** The skill demonstrates a highly effective pattern for wrapping arbitrary processes in security boundaries; it covers complex edge cases like SSL inspection and local service access.

**Summary:** Provides specialized instructions for using the AWF CLI to execute commands within a network-isolated environment with domain whitelisting.

**Source credibility:** High; comes from an official GitHub repository (github/gh-aw-firewall) with recent activity.

**Recency:** Very current, directly addressing modern agentic security concerns.

**Source:** [github/gh-aw-firewall/skill.md](https://github.com/github/gh-aw-firewall/blob/e0c118bc360c3bfaec2ef8ad62735c0992131084/skill.md) · 93★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: awf-skill
description: Use the AWF (Agentic Workflow Firewall) to run commands with network isolation and domain whitelisting. Provides L7 HTTP/HTTPS egress control for AI agents.
allowed-tools: Bash(sudo:*), Bash(awf:*), Bash(docker:*), Read
user-invocable: false
---

# AWF (Agentic Workflow Firewall) Usage Skill

Use this skill when you need to run commands with network isolation, restrict network access to approved domains, or execute AI agents in a sandboxed environment with controlled network access.

## What is AWF?

AWF is a network firewall for agentic workflows that provides:

- **L7 Domain Whitelisting**: Control HTTP/HTTPS traffic at the application layer
- **Host-Level Enforcement**: Uses iptables DOCKER-USER chain to enforce firewall on ALL containers
- **Chroot Mode**: Optional transparent access to host binaries (Python, Node.js, Go) while maintaining network isolation

## When to Use AWF

Use AWF when:
- Running AI agents (Copilot CLI, Claude, etc.) that need network access but should be restricted
- Testing code that makes network requests in a controlled environment
- Enforcing network security policies for automated workflows
- Running untrusted command
```

</details>
