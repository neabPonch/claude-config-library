---
name: google__skills__skill
source: https://github.com/google/skills/blob/a9462f422a7d56a62d7fe7904a0baca1fb0f8146/skills/cloud/google-cloud-networking-observability/SKILL.md
repo: google/skills
kind: skill
stars: 13681
last_pushed: 2026-06-13T19:49:32Z
license: apache-2.0
score: 9
domains: [cloud-infrastructure, networking, observability, google-cloud]
tags: [gcp, troubleshooting, sql-generation, observability]
curated: 2026-06-15
curated_by: config-scout
---

# google/skills — skill

**Why it's worth keeping:** The 'Boundaries' section uses brilliant negative constraints to prevent common agent failures like 'discrepancy loops' or unnecessary verification cycles. Its schema verification procedure for SQL generation is also a high-quality, transferable pattern.

**Summary:** A highly specialized skill file for diagnosing Google Cloud networking issues via logs, metrics, and BigQuery. It emphasizes rapid conclusion-finding and prevents agent looping during multi-tool investigations.

**Source credibility:** Very high; authoritative Google-maintained repository with significant community validation and recent activity.

**Recency:** Extremely current; incorporates modern MCP-first workflows and advanced agentic reasoning patterns.

**Source:** [google/skills/skills/cloud/google-cloud-networking-observability/SKILL.md](https://github.com/google/skills/blob/a9462f422a7d56a62d7fe7904a0baca1fb0f8146/skills/cloud/google-cloud-networking-observability/SKILL.md) · 13681★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: google-cloud-networking-observability
description: >-
  Investigates Google Cloud networking issues by analyzing logs, metrics, and diagnostics. Use when investigating VPC Flow Logs (including cost estimation), NAT, firewall, or threat logs, querying latency and throughput metrics, or running Connectivity Tests for path diagnostics. Don't use for generic VM management or non-observability tasks.
---

# Google Cloud Networking Observability Expert

## 🛑 Core Directive: Results First

1.  **Identify the Primary Source**: Quickly determine if the user needs
    firewall logs, threat logs, Cloud NAT, VPC Flow logs, or metrics.
2.  **Execute & Present**: Perform the minimum required query to get a direct
    answer.
3.  **Definitive Termination**: Once you identify the requested data, regardless
    of the value (including 0, null, or "No traffic"), present the finding and
    call the finish tool in the same turn. Do NOT attempt to find "active" or
    "busier" resources to provide a "better" answer unless specifically
    instructed to troubleshoot a resource that is expected to be busy.

## Log & Telemetry Overview

-   **Threat Logs**: Specialized logs from Cloud Firewall
```

</details>
