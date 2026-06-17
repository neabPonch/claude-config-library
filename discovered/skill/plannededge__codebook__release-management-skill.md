---
name: plannededge__codebook__release-management-skill
source: https://github.com/plannededge/codebook/blob/034a9c6ffaa45e9f2df98f412819f58b45929df7/.claude/skills/release-management.skill.md
repo: plannededge/codebook
kind: skill
stars: 1
last_pushed: 2026-01-31T06:03:19Z
license: mit
score: 8
domains: [devops, delivery, cli-tools]
tags: [release-management, git-workflow, procedural-skills]
curated: 2026-06-16
curated_by: config-scout
---

# plannededge/codebook — skill

**Why it's worth keeping:** Utilizes semantic cross-referencing (@skill/@ref) to create a navigable knowledge graph and provides explicit shell command templates for predictable tool execution.

**Summary:** A highly structured procedural manual for managing software releases, including specific git commands and GitHub release workflows.

**Source credibility:** Low social proof (1 star), but the documentation structure is professional-grade.

**Recency:** Current; aligns perfectly with modern CLI-driven agentic workflows.

**Source:** [plannededge/codebook/.claude/skills/release-management.skill.md](https://github.com/plannededge/codebook/blob/034a9c6ffaa45e9f2df98f412819f58b45929df7/.claude/skills/release-management.skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
document_name: "release-management.skill.md"
location: ".claude/skills/release-management.skill.md"
codebook_id: "CB-SKILL-RELEASE-001"
version: "1.0.0"
date_created: "2026-01-04"
date_last_edited: "2026-01-04"
document_type: "skill"
purpose: "Procedures for planning and executing releases"
skill_metadata:
  category: "delivery"
  complexity: "intermediate"
  estimated_time: "30-60 min per release"
  prerequisites:
    - "Approved PRs ready"
    - "Version determined"
category: "skills"
status: "active"
tags:
  - "skill"
  - "release"
  - "delivery"
ai_parser_instructions: |
  This skill defines procedures for release management.
  Section markers: === SECTION ===
  Procedure markers: === PROCEDURE: NAME ===
---

# Release Management Skill

=== PURPOSE ===

This skill provides procedures for planning and executing releases. Used by the Delivery Lead for all release-related work.

---

=== USED BY ===

| Agent | Purpose |
|-------|---------|
| @agent(delivery-lead) @ref(CB-AGENT-DELIVERY-001) | Primary skill for releases |

---

=== PREREQUISITES ===

Before using this skill:
- [ ] All PRs for release are merged
- [ ] Tests passing on main branch
- [ ] Version number determined
```

</details>
