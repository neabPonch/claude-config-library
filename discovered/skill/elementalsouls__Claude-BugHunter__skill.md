---
name: elementalsouls__Claude-BugHunter__skill
source: https://github.com/elementalsouls/Claude-BugHunter/blob/780caf7ed5b88276e837a1ddd0fb19ee6a0246aa/skills/hunt-misc/SKILL.md
repo: elementalsouls/Claude-BugHunter
kind: skill
stars: 2448
last_pushed: 2026-06-16T07:18:32Z
license: other
score: 9
domains: [security, red-teaming, backend-api]
tags: [bug-bounty, vulnerability-research, penetration-testing]
curated: 2026-06-16
curated_by: config-scout
---

# elementalsouls/Claude-BugHunter — skill

**Why it's worth keeping:** It includes high-signal grep patterns for source reconnaissance and a practical 'Marker Discipline' to ensure high-confidence vulnerability reporting via body-diffing.

**Summary:** A specialized skill for hunting miscellaneous vulnerabilities like broken access control, session management flaws, and information disclosure in enterprise systems.

**Source credibility:** Very high; the repository has significant social proof with 2.4k stars and active maintenance.

**Recency:** Highly current, focusing on modern SaaS, OAuth/SAML flows, and API security standards.

**Source:** [elementalsouls/Claude-BugHunter/skills/hunt-misc/SKILL.md](https://github.com/elementalsouls/Claude-BugHunter/blob/780caf7ed5b88276e837a1ddd0fb19ee6a0246aa/skills/hunt-misc/SKILL.md) · 2448★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: hunt-misc
description: Hunting skill for misc vulnerabilities. Built from 225 public bug bounty reports. Use when hunting misc on any target.
sources: github, hackerone_public
report_count: 225
---

## Crown Jewel Targets

**Why this vuln class pays:**
MISC vulnerabilities span access control failures, information disclosure, session/auth logic bugs, and misconfiguration — the categories that consistently produce the highest payouts because they map directly to business impact: data exposure, account takeover, privilege escalation, and infrastructure compromise.

**Highest-value targets:**
- **SaaS platforms with role hierarchies** (Shopify, GitHub, GitLab) — any boundary between owner/admin/staff/guest is a privilege escalation surface
- **Identity/auth flows** — invitation links, password reset, SAML SSO, OAuth token scopes
- **Multi-tenant systems** — one tenant touching another tenant's data
- **Internal APIs** — LFS endpoints, pre-receive hooks, internal GraphQL/REST that assume caller is trusted
- **Domain/DNS management features** — transfer controls, subdomain delegation
- **Token/credential management** — PAT scopes, deploy keys, API tokens stored in config field
```

</details>
