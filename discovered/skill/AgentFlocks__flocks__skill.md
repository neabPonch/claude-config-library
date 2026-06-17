---
name: AgentFlocks__flocks__skill
source: https://github.com/AgentFlocks/flocks/blob/dd82bac26e557296dfeef3b790faf3f898609a34/.flocks/flockshub/plugins/skills/Anthropic-Cybersecurity-Skills/exploiting-deeplink-vulnerabilities/SKILL.md
repo: AgentFlocks/flocks
kind: skill
stars: 371
last_pushed: 2026-06-15T03:42:39Z
license: apache-2.0
score: 9
domains: [cybersecurity, mobile-security, penetration-testing]
tags: [android, ios, deep-links, owasp-mobile]
curated: 2026-06-15
curated_by: config-scout
---

# AgentFlocks/flocks — skill

**Why it's worth keeping:** Includes highly actionable shell commands (adb, plutil, grep) and follows a logical reconnaissance-to-exploitation sequence typical of professional security audits.

**Summary:** Provides a structured penetration testing workflow for discovering and exploiting mobile deep link vulnerabilities on Android and iOS.

**Source credibility:** The repository shows high engagement with 371 stars and active maintenance for specialized SecOps workflows.

**Recency:** 

**Source:** [AgentFlocks/flocks/.flocks/flockshub/plugins/skills/Anthropic-Cybersecurity-Skills/exploiting-deeplink-vulnerabilities/SKILL.md](https://github.com/AgentFlocks/flocks/blob/dd82bac26e557296dfeef3b790faf3f898609a34/.flocks/flockshub/plugins/skills/Anthropic-Cybersecurity-Skills/exploiting-deeplink-vulnerabilities/SKILL.md) · 371★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: exploiting-deeplink-vulnerabilities
description: 'Tests and exploits deep link (URL scheme and App Link) vulnerabilities in Android and iOS mobile applications
  to identify unauthorized access, data injection, intent hijacking, and redirect manipulation. Use when assessing mobile
  app attack surface through custom URI schemes, Android App Links, iOS Universal Links, or intent-based navigation. Activates
  for requests involving deep link security testing, URL scheme exploitation, mobile intent abuse, or link hijacking.

  '
domain: cybersecurity
subdomain: mobile-security
author: mahipal
tags:
- mobile-security
- android
- ios
- deep-links
- owasp-mobile
- penetration-testing
version: 1.0.0
license: Apache-2.0
nist_csf:
- PR.PS-01
- PR.AA-05
- ID.RA-01
- DE.CM-09
---
# Exploiting Deep Link Vulnerabilities

## When to Use

Use this skill when:
- Assessing mobile app deep link handling for injection and redirect vulnerabilities
- Testing Android intent filters and iOS URL scheme handlers for unauthorized access
- Evaluating App Links (Android) and Universal Links (iOS) verification
- Testing for link hijacking via competing app registrations

**Do not use** without author
```

</details>
