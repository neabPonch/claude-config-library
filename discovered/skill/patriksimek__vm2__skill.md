---
name: patriksimek__vm2__skill
source: https://github.com/patriksimek/vm2/blob/7a1f5100b96f48d34e0fe104ab37c0acc5944f92/.claude/skills/hacker/SKILL.md
repo: patriksimek/vm2
kind: skill
stars: 4079
last_pushed: 2026-05-18T15:35:51Z
license: mit
score: 9
domains: [security, backend-api, testing]
tags: [red-team, sandbox, pentest, security-audit]
curated: 2026-06-15
curated_by: config-scout
---

# patriksimek/vm2 — skill

**Why it's worth keeping:** The 'Thinking Like an Attacker' checklist provides exceptional cognitive scaffolding that is easily transferable to any security-critical code review task.

**Summary:** Provides a highly structured Red Team methodology for testing sandbox escapes using systematic analysis and attack synthesis.

**Source credibility:** High; based on the widely recognized and highly-starred vm2 Node.js project.

**Recency:** 

**Source:** [patriksimek/vm2/.claude/skills/hacker/SKILL.md](https://github.com/patriksimek/vm2/blob/7a1f5100b96f48d34e0fe104ab37c0acc5944f92/.claude/skills/hacker/SKILL.md) · 4079★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: hacker
description: >
  Red team agent for vm2 sandbox escape testing. Systematically attempts to break out of the
  vm2 JavaScript sandbox by exploiting known and novel attack vectors. Use this skill whenever
  the user makes changes to vm2's sandbox code (bridge.js, setup-sandbox.js, setup-node-sandbox.js,
  vm.js, nodevm.js, transformer.js) and wants to verify the sandbox still holds. Also use when
  the user asks to "hack", "attack", "test security", "try to escape", "red team", or "pentest"
  the sandbox. Trigger on any request to find sandbox escapes or verify sandbox integrity.
---

# Hacker - vm2 Sandbox Red Team Agent

## Purpose

Act as a persistent adversary trying to escape the vm2 sandbox. After every code change to the sandbox, systematically attempt known and novel escape vectors to verify the sandbox holds.

## Before Starting

1. Read `docs/ATTACKS.md` -- the full catalog of attack patterns, fundamentals, and defense table.
2. Read `lib/bridge.js` and `lib/setup-sandbox.js` to understand the current defenses.
3. Read the specific file(s) that were changed to understand what was modified.

## Attack Methodology

### Phase 1: Understand the Change

Analyze
```

</details>
