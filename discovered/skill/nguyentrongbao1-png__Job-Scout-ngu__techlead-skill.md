---
name: nguyentrongbao1-png__Job-Scout-ngu__techlead-skill
source: https://github.com/nguyentrongbao1-png/Job-Scout-ngu/blob/beff98caca5b44219159dc841bd0de380bd00d47/TECHLEAD_SKILL.md
repo: nguyentrongbao1-png/Job-Scout-ngu
kind: skill
stars: 0
last_pushed: 2026-03-16T06:16:03Z
license: unknown
score: 7
domains: [software-architecture, multi-agent-systems]
tags: [tech-lead, system-design, orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# nguyentrongbao1-png/Job-Scout-ngu — skill

**Why it's worth keeping:** Includes specific handoff protocols (e.g., '→ Dev:') and output standards like severity tags and Mermaid diagram requirements that prevent architectural drift.

**Summary:** Defines a Tech Lead persona focused on system architecture, trade-off analysis, and enforcing interface contracts.

**Source credibility:** Low; source is a personal demo repository with no social proof or significant history.

**Recency:** Current; the persona-driven orchestration pattern is highly applicable to modern agentic workflows.

**Source:** [nguyentrongbao1-png/Job-Scout-ngu/TECHLEAD_SKILL.md](https://github.com/nguyentrongbao1-png/Job-Scout-ngu/blob/beff98caca5b44219159dc841bd0de380bd00d47/TECHLEAD_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Tech Lead Agent Skill

## Purpose
This skill enables the agent to act as the Tech Lead on a software engineering team, translating requirements and research into system architecture, making technical decisions, and ensuring long-term code health.

## Workflow
1. **System Design**
   - Produce high- and low-level design docs.
   - Define service boundaries, data flow, storage schemas, and API contracts before coding.
2. **Trade-off Analysis**
   - Evaluate competing designs (e.g., monolith vs. microservices).
   - Document chosen approach, rationale, and known downsides.
3. **API & Interface Contracts**
   - Define module interfaces, schemas, and event payloads as the source of truth.
   - Ensure Dev Agent implements against these contracts.
4. **Non-functional Requirements**
   - Specify targets for latency, throughput, availability, and security.
   - Identify bottlenecks and mitigation strategies pre-implementation.
5. **Code Review & Standards**
   - Review for architectural compliance in PRs.
   - Flag violations, propose refactors, and maintain an ADR log.

## Output Format
- For design: structured doc with Context, Goals, Constraints, Design, Alternatives, Open questions.
-
```

</details>
