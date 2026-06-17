---
name: mukul975__Anthropic-Cybersecurity-Skills__skill
source: https://github.com/mukul975/Anthropic-Cybersecurity-Skills/blob/04450304b12645cb2b974ab96d28c0664758a88d/skills/performing-bandwidth-throttling-attack-simulation/SKILL.md
repo: mukul975/Anthropic-Cybersecurity-Skills
kind: skill
stars: 15937
last_pushed: 2026-06-01T10:15:48Z
license: apache-2.0
score: 9
domains: [security, network-security, devops]
tags: [network, chaos-engineering, security-testing, linux]
curated: 2026-06-16
curated_by: config-scout
---

# mukul975/Anthropic-Cybersecurity-Skills — skill

**Why it's worth keeping:** The 'baseline -> simulate -> verify -> cleanup' workflow is highly transferable for chaos engineering and security audits. It includes specific techniques for simulating both network-layer (tc/netem) and application-layer (Slowloris) degradation.

**Summary:** Simulates network degradation and bandwidth throttling using Linux traffic control (tc) and Python-based connection exhaustion. It provides a complete operational lifecycle including baselining, progressive stress testing, and impact verification.

**Source credibility:** High; the source repository is a well-regarded, large-scale collection of structured cybersecurity skills.

**Recency:** Current; utilizes standard Linux networking tools compatible with modern agentic environments.

**Source:** [mukul975/Anthropic-Cybersecurity-Skills/skills/performing-bandwidth-throttling-attack-simulation/SKILL.md](https://github.com/mukul975/Anthropic-Cybersecurity-Skills/blob/04450304b12645cb2b974ab96d28c0664758a88d/skills/performing-bandwidth-throttling-attack-simulation/SKILL.md) · 15937★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: performing-bandwidth-throttling-attack-simulation
description: 'Simulates bandwidth throttling and network degradation attacks using
  tc, iperf3, and Scapy in authorized environments to test quality-of-service controls,
  application resilience, and network monitoring detection of traffic manipulation
  attacks.

  '
domain: cybersecurity
subdomain: network-security
tags:
- network-security
- bandwidth-throttling
- qos
- traffic-shaping
- network-resilience
version: '1.0'
author: mahipal
license: Apache-2.0
nist_csf:
- PR.IR-01
- DE.CM-01
- ID.AM-03
- PR.DS-02
mitre_attack:
- T1046
- T1040
- T1557
- T1071
---
# Performing Bandwidth Throttling Attack Simulation

## When to Use

- Testing application resilience to degraded network conditions during authorized security assessments
- Validating QoS policies detect and mitigate unauthorized traffic shaping on the network
- Simulating network slowloris-style attacks that degrade bandwidth rather than causing complete outages
- Assessing the impact of bandwidth-based attacks on VoIP, video conferencing, and real-time applications
- Testing network monitoring tools' ability to detect abnormal bandwidth utilization patterns

**Do
```

</details>
