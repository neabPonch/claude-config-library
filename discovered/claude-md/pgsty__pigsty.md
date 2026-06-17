---
name: pgsty__pigsty
source: https://github.com/pgsty/pigsty/blob/67959cfa1780352f57860f1eb730f6e2068f6fc3/CLAUDE.md
repo: pgsty/pigsty
kind: claude-md
stars: 5166
last_pushed: 2026-05-11T08:42:45Z
license: apache-2.0
score: 9
domains: [database-ops, infrastructure, devops, security]
tags: [postgresql, ansible, safety-first, dba]
curated: 2026-06-14
curated_by: config-scout
---

# pgsty/pigsty — claude-md

**Why it's worth keeping:** It uses a tiered permission model (Always Allowed vs. Requires Confirmation vs. Forbidden) and enforces specific verification rituals like asking the user to type exact names before destructive actions.

**Summary:** Defines strict operational guardrails and safety protocols for managing production PostgreSQL clusters via Ansible and the 'pig' CLI.

**Source credibility:** Highly credible; high-star enterprise-grade PostgreSQL distribution with recent activity.

**Recency:** Very current; perfectly tailored for modern agentic workflows requiring safety guardrails.

**Source:** [pgsty/pigsty/CLAUDE.md](https://github.com/pgsty/pigsty/blob/67959cfa1780352f57860f1eb730f6e2068f6fc3/CLAUDE.md) · 5166★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Pigsty Production Environment - Claude Code Guide

Pigsty v4.3.0 | PostgreSQL RDS/DBaaS | Apache-2.0
- EN Docs: https://pigsty.io/docs
- CN Docs: https://pigsty.cc/docs
- Expert Support: https://pigsty.io/price (rh@vonng.com)

---

## Important Files

**`pigsty.yml`**, source of truth of this deployment, always read it to understand current environment.
Sometimes the real state may drift from the config file, especially after manual changes / failover. trust by verify.

**`files/pki/ca/ca.key`** - highly sensitive CA private key. Keep it safe, never share it, don't lose it.

If `pig` cli is available, you can use it to perform operation command with caution. https://pigsty.io/docs/pig


---

## Standard Operating Procedures

### Before Any Change

1. **Identify scope:** Which cluster? Which nodes?
2. **Check current state:** `pig pg list`, system status
3. **Verify backup:** `pig pb info` - is backup recent?
4. **Dry run first:** Add `--check` to playbook

### For Dangerous Operations

1. **Confirm with user** - even in YOLO mode
2. **Verify backup exists and is recent**
3. **Ask user to type exact target name**
4. **Execute with explicit `-l` limit flag**

### Incident Response
```

</details>
