---
name: CyberStrikeus__CyberStrike__skill
source: https://github.com/CyberStrikeus/CyberStrike/blob/0d64b551b4408670fcf603d2b831fbdd2594cc4a/.cyberstrike/skill/CIS_benchmarks/Server_Software/Apache_HTTP_Server/CIS_Apache_HTTP_Server_2.4_Benchmark_v2.3.0/cis-apache24-7.12/SKILL.md
repo: CyberStrikeus/CyberStrike
kind: skill
stars: 326
last_pushed: 2026-06-14T23:36:21Z
license: agpl-3.0
score: 9
domains: [security, devops, linux, web-server]
tags: [cis, apache, tls, hardening]
curated: 2026-06-15
curated_by: config-scout
---

# CyberStrikeus/CyberStrike — skill

**Why it's worth keeping:** It contains ready-to-run shell commands for both auditing (sslscan/openssl) and remediation, which is perfect for agentic tool execution. The structured approach linking 'Audit' directly to 'Remediation' makes it highly actionable.

**Summary:** Provides precise instructions to audit and remediate Apache cipher suites to ensure Forward Secrecy based on CIS benchmarks.

**Source credibility:** High; the repo has significant social proof (326 stars) and very recent activity.

**Recency:** 

**Source:** [CyberStrikeus/CyberStrike/.cyberstrike/skill/CIS_benchmarks/Server_Software/Apache_HTTP_Server/CIS_Apache_HTTP_Server_2.4_Benchmark_v2.3.0/cis-apache24-7.12/SKILL.md](https://github.com/CyberStrikeus/CyberStrike/blob/0d64b551b4408670fcf603d2b831fbdd2594cc4a/.cyberstrike/skill/CIS_benchmarks/Server_Software/Apache_HTTP_Server/CIS_Apache_HTTP_Server_2.4_Benchmark_v2.3.0/cis-apache24-7.12/SKILL.md) · 326★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cis-apache24-7.12
description: "Ensure Only Cipher Suites That Provide Forward Secrecy Are Enabled (Manual)"
category: cis-apache
version: "2.3.0"
author: cyberstrike-official
tags: [cis, apache, linux, ssl, tls, forward-secrecy, ecdhe, dhe, perfect-forward-secrecy]
cis_id: "7.12"
cis_benchmark: "CIS Apache HTTP Server 2.4 Benchmark v2.3.0"
tech_stack: [linux, apache]
cwe_ids: []
chains_with: []
prerequisites: []
severity_boost: {}
---

# Ensure Only Cipher Suites That Provide Forward Secrecy Are Enabled (Manual)

## Profile Applicability

- Level 2

## Description

In cryptography, _forward secrecy_ (FS), which is also known as _perfect forward secrecy_ (PFS), is a feature of specific key exchange protocols that give assurance that your session keys will not be compromised even if the private key of the server is compromised. Protocols such as RSA do not provide the forward secrecy, while the protocols `ECDHE` (Elliptic-Curve Diffie-Hellman Ephemeral) and the `DHE` (Diffie-Hellman Ephemeral) will provide forward secrecy. The `ECDHE` is the stronger protocol and should be preferred, while the `DHE` may be allowed for greater compatibility with older clients. The TLS ciphe
```

</details>
