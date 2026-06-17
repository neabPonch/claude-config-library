---
name: xalgord__xalgorix__skill
source: https://github.com/xalgord/xalgorix/blob/faa68066dcdb15d0f023949b67bb35571a25302a/internal/tools/skills/data/network-security/detecting-port-scanning-with-fail2ban/SKILL.md
repo: xalgord/xalgorix
kind: skill
stars: 610
last_pushed: 2026-06-13T05:02:44Z
license: mit
score: 9
domains: [security, devops, linux-admin]
tags: [fail2ban, network-security, iptables, intrusion-detection]
curated: 2026-06-15
curated_by: config-scout
---

# xalgord/xalgorix — skill

**Why it's worth keeping:** The 'Detection Gaps & Validation' section is elite; it identifies specific technical failure modes like slow-scan evasion and backend mismatches. The pattern of using custom iptables rules to feed a Fail2ban jail is a highly transferable security architecture template.

**Summary:** Provides a comprehensive workflow for integrating iptables logging with Fail2ban to detect and mitigate port scanning activity.

**Source credibility:** High; the source repo is well-starred and demonstrates specialized cybersecurity domain expertise.

**Recency:** Current; uses modern systemd and iptables integration standards.

**Source:** [xalgord/xalgorix/internal/tools/skills/data/network-security/detecting-port-scanning-with-fail2ban/SKILL.md](https://github.com/xalgord/xalgorix/blob/faa68066dcdb15d0f023949b67bb35571a25302a/internal/tools/skills/data/network-security/detecting-port-scanning-with-fail2ban/SKILL.md) · 610★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: detecting-port-scanning-with-fail2ban
description: 'Configures Fail2ban with custom filters and actions to detect port scanning activity, SSH brute force attempts,
  and network reconnaissance, automatically banning offending IP addresses and alerting security teams to suspicious network
  probing.

  '
domain: cybersecurity
subdomain: network-security
tags:
- network-security
- fail2ban
- port-scanning
- intrusion-prevention
- automated-defense
version: '1.0'
author: mahipal
license: Apache-2.0
nist_csf:
- PR.IR-01
- DE.CM-01
- ID.AM-03
- PR.DS-02
---
# Detecting Port Scanning with Fail2ban

## When to Use

- Automatically blocking IP addresses that perform port scans against internet-facing servers
- Defending SSH, HTTP, FTP, and other services against brute force attacks with automated IP banning
- Creating custom detection filters for organization-specific attack patterns in log files
- Reducing noise from automated scanning bots before traffic reaches IDS/IPS for deeper analysis
- Implementing defense-in-depth by adding host-based automated response to network monitoring

**Do not use** as the sole network security control, for protecting against distributed attacks
```

</details>
