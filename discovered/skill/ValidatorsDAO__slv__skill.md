---
name: ValidatorsDAO__slv__skill
source: https://github.com/ValidatorsDAO/slv/blob/6fcee0f297853d59b0060f2b6ec5f0c1dca44cf4/oss-skills/slv-smt-disable/SKILL.md
repo: ValidatorsDAO/slv
kind: skill
stars: 86
last_pushed: 2026-06-06T13:02:17Z
license: apache-2.0
score: 8
domains: [devops, systems-ops, performance-tuning]
tags: [linux, grub, kernel, optimization, solana]
curated: 2026-06-15
curated_by: config-scout
---

# ValidatorsDAO/slv — skill

**Why it's worth keeping:** Includes critical verification steps (checking /proc/cmdline) and a clear rollback procedure, which are essential for high-risk system changes.

**Summary:** Provides instructions for disabling SMT via GRUB to optimize single-thread performance for Solana validators.

**Source credibility:** High; comes from a specialized toolkit specifically designed for validator orchestration.

**Recency:** Current; follows standard Linux sysadmin practices used today.

**Source:** [ValidatorsDAO/slv/oss-skills/slv-smt-disable/SKILL.md](https://github.com/ValidatorsDAO/slv/blob/6fcee0f297853d59b0060f2b6ec5f0c1dca44cf4/oss-skills/slv-smt-disable/SKILL.md) · 86★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: slv-smt-disable
description: Disable SMT (Hyper-Threading) by adding `nosmt=force` to GRUB. Required for stable single-thread performance on Solana validators / RPCs. Reboot required.
---

# SLV SMT (Hyper-Threading) Disable Skill

Solana validator / RPC throughput is dominated by single-thread instruction performance, so disabling SMT consistently produces higher and more stable performance. Applied during `slv v init` / `slv r init` as part of the tuning phase.

## How it works

Adds `nosmt=force` to `GRUB_CMDLINE_LINUX_DEFAULT` in `/etc/default/grub` and runs `update-grub`. After reboot, the kernel only schedules on one logical thread per physical core.

## Related ansible playbook

- `ansible/cmn/smt_disable.yml` — appends `nosmt=force` to GRUB and runs `update-grub`
- Idempotency marker: `/var/lib/slv/.smt_disabled`

## Standalone run

```bash
ansible-playbook -i inventory.yml cmn/smt_disable.yml --limit <host>
```

Sets `need_reboot=true` only when GRUB actually changed; the orchestrator reboots when needed.

## Verification

```bash
# on the host
cat /proc/cmdline                      # should contain nosmt=force
lscpu | grep -E 'Thread|Core|Socket'   # Thread(s) p
```

</details>
