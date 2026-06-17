---
name: UnitOneAI__SecuritySkills__skill
source: https://github.com/UnitOneAI/SecuritySkills/blob/553177e4156c0c163232e25656be282deaa40bb7/skills/network/firewall-review/SKILL.md
repo: UnitOneAI/SecuritySkills
kind: skill
stars: 16
last_pushed: 2026-06-16T05:58:57Z
license: mit
score: 9
domains: [security, devops, cli-tools]
tags: [firewall, audit, compliance, network-security]
curated: 2026-06-16
curated_by: config-scout
---

# UnitOneAI/SecuritySkills — skill

**Why it's worth keeping:** It includes highly actionable 'Discovery' patterns (Glob/Grep) for IaC and cloud-native configs, and defines a clear logical algorithm for detecting shadowed rules.

**Summary:** An expert security engineering skill that automates firewall rule base audits against NIST and CIS standards. It provides a structured workflow from file discovery to logical analysis of rules.

**Source credibility:** Strong; the repository is specialized in security skills and shows active maintenance.

**Recency:** Current; incorporates modern infrastructure patterns like Terraform and Kubernetes NetworkPolicies.

**Source:** [UnitOneAI/SecuritySkills/skills/network/firewall-review/SKILL.md](https://github.com/UnitOneAI/SecuritySkills/blob/553177e4156c0c163232e25656be282deaa40bb7/skills/network/firewall-review/SKILL.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: firewall-review
description: >
  Performs a structured firewall rule base audit against CIS Controls v8
  (Controls 4.4 and 4.5) and NIST SP 800-41 Rev 1 (Guidelines on Firewalls and
  Firewall Policy). Auto-invoked when reviewing firewall configurations, ACLs,
  or network security policies. Produces a prioritized findings report covering
  overly permissive rules, shadowed rules, logging gaps, and egress filtering
  deficiencies.
tags: [network, firewall, segmentation]
role: [security-engineer]
phase: [operate]
frameworks: [CIS-Controls-v8, NIST-SP-800-41-Rev1]
difficulty: intermediate
time_estimate: "30-60min"
version: "1.0.0"
author: unitoneai
license: MIT
allowed-tools: Read, Grep, Glob
injection-hardened: true
argument-hint: "[target-file-or-directory]"
---

# Firewall Rule Audit

A structured, repeatable process for auditing firewall rule bases against CIS Controls v8 (Control 4.4 -- Implement and Manage a Firewall on Servers, Control 4.5 -- Implement and Manage a Firewall on End-User Devices) and NIST SP 800-41 Rev 1 (Guidelines on Firewalls and Firewall Policy). This skill produces findings with traceable control references, severity ratings, and actionable remed
```

</details>
