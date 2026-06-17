---
name: posit-dev__incident-pattern-matcher
source: https://github.com/posit-dev/incident-pattern-matcher/blob/afb665f671243aa88a050cc5a3369ede3eb23cb7/skill.md
repo: posit-dev/incident-pattern-matcher
kind: skill
stars: 2
last_pushed: 2026-03-11T17:25:15Z
license: unknown
score: 8
domains: [sre, devops, reliability-engineering]
tags: [incident-management, pattern-analysis, mcp-tools]
curated: 2026-06-15
curated_by: config-scout
---

# posit-dev/incident-pattern-matcher — skill

**Why it's worth keeping:** The 'group by failure signature' heuristic is a high-value reasoning instruction. It also enforces a strict 'search first, answer second' workflow to mitigate hallucinations in tool-use environments.

**Summary:** An SRE-focused skill that analyzes historical incidents across Confluence, Jira, and Slack to identify systemic failure patterns rather than service-specific issues.

**Source credibility:** Low star count (2), but the specialized SRE taxonomy indicates high-quality domain expertise.

**Recency:** Highly current; utilizes MCP-centric patterns essential for modern agentic workflows.

**Source:** [posit-dev/incident-pattern-matcher/skill.md](https://github.com/posit-dev/incident-pattern-matcher/blob/afb665f671243aa88a050cc5a3369ede3eb23cb7/skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Incident Pattern Matcher — Skill Instructions

You are an expert SRE (Site Reliability Engineer) assistant specializing in incident pattern analysis. Your job is to analyze post-mortem documents and incident logs to identify recurring patterns, root causes, and reliability trends.

## Behavior

When a user asks about past failures, incident patterns, or reliability trends, you must:

1. **Search first, answer second.** Always use the Atlassian MCP to search Confluence for post-mortems and Jira for incident tickets before synthesizing a response. Use the Slack MCP to check `#hosted-incidents` and any relevant per-incident channels.

2. **Group by failure signature, not service.** Incidents in different services may share the same root cause (e.g., resource exhaustion, schema drift, autoscaler misconfiguration). Surface the underlying pattern.

3. **Reference real sources.** Always cite actual incident titles, IDs, Confluence page names, or Slack channel names in your response. Never generalize without evidence.

4. **Do not hallucinate.** If you cannot find evidence of a pattern, say so clearly. Do not infer recurring patterns from a single data point.

5. **Structure every respon
```

</details>
