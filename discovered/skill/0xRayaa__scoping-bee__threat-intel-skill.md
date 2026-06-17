---
name: 0xRayaa__scoping-bee__threat-intel-skill
source: https://github.com/0xRayaa/scoping-bee/blob/138222e148fd6f0d5b7b92b1fee304bbc09417b7/THREAT_INTEL_SKILL.md
repo: 0xRayaa/scoping-bee
kind: skill
stars: 3
last_pushed: 2026-05-04T10:01:50Z
license: mit
score: 9
domains: [security, devsecops, blockchain]
tags: [threat-intel, malware-detection, forensics, audit-safety]
curated: 2026-06-15
curated_by: config-scout
---

# 0xRayaa/scoping-bee — skill

**Why it's worth keeping:** The methodology provides highly specific 'red flag' patterns (e.g., npm lifecycle hooks, DNS/HTTP exfiltration, JS obfuscation) that transform the agent into a specialized security investigator. It also includes a robust two-tier execution strategy using sandboxed Docker or manual LLM analysis.

**Summary:** A professional-grade forensic skill designed to scan untrusted codebases for malware, backdoors, and exfiltration vectors before an auditor interacts with them.

**Source credibility:** Niche tool from a security-focused developer with recent activity.

**Recency:** Highly current; updated within the last month.

**Source:** [0xRayaa/scoping-bee/THREAT_INTEL_SKILL.md](https://github.com/0xRayaa/scoping-bee/blob/138222e148fd6f0d5b7b92b1fee304bbc09417b7/THREAT_INTEL_SKILL.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: threat-intel-scan
description: >-
  Comprehensive threat intelligence scanner for untrusted codebases.
  Detects malware, backdoors, supply chain attacks, phishing kits, obfuscated
  payloads, credential theft, crypto drainers, honeypot contracts, and all
  known classes of malicious code across Solidity, Rust, JavaScript, Python,
  Go, and infrastructure files. Use before any audit engagement to protect
  auditor machines and flag malicious intent.
---

# THREAT INTELLIGENCE SCAN — COMPREHENSIVE SKILL

**`━━━━⬡⬡⬡━━━━ THREAT INTEL METHODOLOGY ━━━━⬡⬡⬡━━━━`**

Deep, multi-phase threat intelligence scanner for **untrusted codebases**.
Run this BEFORE touching, building, testing, or auditing any code from an
external party. Covers **all known malicious code classes** across every
language and framework commonly seen in smart-contract audit engagements.

> **SANDBOX FIRST**: Always run inside an isolated environment (VM, Docker,
> cloud instance). Only move code to your local machine after a CLEAN verdict.

---

## TWO METHODS TO RUN THIS SCAN

### Method A — Isolated Docker scan (preferred)

Runs the full 16-phase scanner inside a container with `--network none` and a
read-on
```

</details>
