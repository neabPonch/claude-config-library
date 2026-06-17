---
name: slowmist__slowmist-agent-security__report-skill
source: https://github.com/slowmist/slowmist-agent-security/blob/0718ece96b8acb121466874d111fe80d41971a57/templates/report-skill.md
repo: slowmist/slowmist-agent-security
kind: skill
stars: 467
last_pushed: 2026-04-17T02:12:58Z
license: mit
score: 8
domains: [security, agents-ai, governance]
tags: [audit-template, mcp-security, risk-assessment]
curated: 2026-06-15
curated_by: config-scout
---

# slowmist/slowmist-agent-security — skill

**Why it's worth keeping:** It mandates extreme specificity in permission mapping (e.g., specific file paths instead of broad categories) and forces scrutiny of 'human-in-the-loop' and data boundary behaviors.

**Summary:** A highly structured security audit template for vetting MCP skills and AI agents before integration.

**Source credibility:** High; authored by SlowMist, a recognized security firm, with significant community interest shown via star count.

**Recency:** Very current; updated within the last few months to reflect modern agentic risks.

**Source:** [slowmist/slowmist-agent-security/templates/report-skill.md](https://github.com/slowmist/slowmist-agent-security/blob/0718ece96b8acb121466874d111fe80d41971a57/templates/report-skill.md) · 467★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill / MCP Security Assessment Report Template

Use this template when reporting the results of a skill-mcp.md review.

---

```
════════════════════════════════════
  SKILL / MCP SECURITY ASSESSMENT
────────────────────────────────────
  Name:         [skill-name]
  Version:      [x.y.z]
  Source:       [clawhub / github / npm / url]
  Author:       [name or organization]
  Trust Tier:   [1-5] — [description]
  Published:    [date]
  Last Updated: [date]
────────────────────────────────────
  FILES SCANNED
  Total: [n]  |  Executable: [n]  |  Docs: [n]
  High-risk files: [list or "None"]
────────────────────────────────────
  RED FLAGS
  [None]
  — or —
  • [flag-1]: [description] (Severity: 🔴/🟡)
  • [flag-2]: [description] (Severity: 🔴/🟡)
────────────────────────────────────
  PERMISSIONS REQUIRED
  Read:     [files/directories or "None"]
  Write:    [files/directories or "None"]
  Network:  [domains/endpoints or "None"]
  System:   [commands or "None"]
  Env Vars: [variable names or "None"]
────────────────────────────────────
  ARCHITECTURE
  Credential handling:  [description]
  Human-in-the-loop:    [Yes/No — detail]
  Auto-update:          [Yes/No — detail]
  Data boundar
```

</details>
