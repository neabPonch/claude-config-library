---
name: TerminalSkills__skills__skill
source: https://github.com/TerminalSkills/skills/blob/77fa0150aa0921f892420d3ec2a9204e3124b71e/skills/amass/SKILL.md
repo: TerminalSkills/skills
kind: skill
stars: 74
last_pushed: 2026-06-11T19:37:07Z
license: apache-2.0
score: 9
domains: [security, cli-tools, network-mapping]
tags: [dns, reconnaissance, owasp, amass]
curated: 2026-06-16
curated_by: config-scout
---

# TerminalSkills/skills — skill

**Why it's worth keeping:** Includes a practical Python script for parsing JSON output and a complete API configuration template, which allows an agent to move beyond execution into data analysis.

**Summary:** A comprehensive technical runbook for OWASP Amass that covers the entire lifecycle from installation to advanced data processing.

**Source credibility:** High-quality documentation from a recently updated repository with active maintenance.

**Recency:** Highly relevant as it focuses on standard CLI tool workflows compatible with modern AI agents.

**Source:** [TerminalSkills/skills/skills/amass/SKILL.md](https://github.com/TerminalSkills/skills/blob/77fa0150aa0921f892420d3ec2a9204e3124b71e/skills/amass/SKILL.md) · 74★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: amass
description: >-
  OWASP Amass for in-depth DNS enumeration, subdomain discovery, and network mapping with active
  and passive modes. Use when: comprehensive subdomain enumeration, ASN and IP range mapping, attack
  surface discovery, building full network topology of a target organization.
license: Apache-2.0
compatibility: "Go 1.18+ (binary) or Docker"
metadata:
  author: terminal-skills
  version: "1.0.0"
  category: research
  tags: [amass, dns, subdomain, attack-surface, network-mapping]
  use-cases:
    - "Enumerate all subdomains for a target domain using passive sources"
    - "Map ASN, IP ranges, and CIDR blocks for an organization"
    - "Discover shadow IT and forgotten subdomains before a pentest"
    - "Build a visual network graph of target infrastructure"
  agents: [claude-code, openai-codex, gemini-cli, cursor]
---

# OWASP Amass

## Overview

OWASP Amass performs network mapping of attack surfaces and external asset discovery using open source information gathering and active reconnaissance techniques. It supports dozens of passive data sources (certificate transparency, DNS datasets, APIs) and active techniques (brute force, DNS zone transfers). Am
```

</details>
