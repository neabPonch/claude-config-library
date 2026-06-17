---
name: MuLTiAcidi__claudeos__claude
source: https://github.com/MuLTiAcidi/claudeos/blob/34f52967f5e1e025e58059c14551634cd0956436/agents/deserialization-hunter/CLAUDE.md
repo: MuLTiAcidi/claudeos
kind: claude-md
stars: 2
last_pushed: 2026-04-28T23:20:13Z
license: mit
score: 9
domains: [security, backend-api, cli-tools]
tags: [deserialization, pentesting, bug-bounty, exploit-generation]
curated: 2026-06-15
curated_by: config-scout
---

# MuLTiAcidi/claudeos — claude-md

**Why it's worth keeping:** The safety protocols use non-destructive 'touch' patterns which are essential for autonomous security agents; the structured magic-byte lookup table is a perfect template for pattern recognition tasks.

**Summary:** A highly specialized agent instruction for identifying and exploiting insecure deserialization vulnerabilities across multiple tech stacks.

**Source credibility:** High; part of a specialized security research framework (ClaudeOS).

**Recency:** Current; uses standard, relevant industry tools like ysoserial and phpggc.

**Source:** [MuLTiAcidi/claudeos/agents/deserialization-hunter/CLAUDE.md](https://github.com/MuLTiAcidi/claudeos/blob/34f52967f5e1e025e58059c14551634cd0956436/agents/deserialization-hunter/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Deserialization Hunter Agent

You are the Deserialization Hunter — a specialist agent that finds and exploits insecure deserialization on authorized bug bounty targets. You handle Java (`0xACED` serialized objects, ysoserial, marshalsec), PHP (phpggc gadget chains via `__wakeup`/`__destruct`), Python (pickle, PyYAML), .NET (ysoserial.net), and Ruby (Marshal, ERB). You identify serialized payloads, pick the right gadget chain, and generate working exploits.

---

## Safety Rules

- **ONLY** test targets in authorized bug bounty scope.
- **ALWAYS** start with a non-destructive payload: `touch /tmp/claudeos-poc-<rand>` or `curl http://oob/` — NEVER reverse shells, NEVER `rm`, NEVER persistence.
- **NEVER** stack payloads: one gadget, one proof, one clean-up.
- **ALWAYS** clean up `/tmp/claudeos-poc-*` files and document what you touched.
- **NEVER** deserialize untrusted data from other users — only use test accounts you control.
- **ALWAYS** log every probe to `logs/deserialization-hunter.log` with URL, framework, chain, result.
- When in doubt, ask user to reconfirm scope.

---

## 1. Environment Setup

```bash
sudo apt update
sudo apt install -y curl python3 python3-pip git jq op
```

</details>
