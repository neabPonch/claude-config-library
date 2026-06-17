---
name: NVMau__ai-qc-seminar__demo-skill
source: https://github.com/NVMau/ai-qc-seminar/blob/5bedc79c7682aabc6817af881e70bbbfda30a6f5/docs/demo-skill.md
repo: NVMau/ai-qc-seminar
kind: skill
stars: 0
last_pushed: 2026-05-30T01:38:14Z
license: unknown
score: 8
domains: [qa-automation, web-frontend, agents-ai, mcp]
tags: [smoke-test, playwright, orchestration]
curated: 2026-06-16
curated_by: config-scout
---

# NVMau/ai-qc-seminar — skill

**Why it's worth keeping:** The 'Spec (oracle)' pattern provides high-quality grounding for LLM assertions, and the workflow demonstrates effective multi-tool orchestration by closing the loop from bug detection to issue reporting.

**Summary:** A structured QA smoke test playbook that integrates Playwright browser automation with an issue-tracking MCP. It uses a clear 'Spec' table to act as a ground-truth oracle for the agent.

**Source credibility:** Low; it is a teaching/demo file from a seminar rather than a production tool.

**Recency:** Current; demonstrates modern MCP-driven agentic workflows.

**Source:** [NVMau/ai-qc-seminar/docs/demo-skill.md](https://github.com/NVMau/ai-qc-seminar/blob/5bedc79c7682aabc6817af881e70bbbfda30a6f5/docs/demo-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill: `qc-tasks-smoke-test`

A sample skill (playbook) the agent follows during the seminar's demo section.
Goal: run a smoke test against `/demo-app/` and surface anything that violates the spec.

> This file is shown on the slide for illustration. In a real project, the skill
> usually lives in `.agents/skills/qc-tasks-smoke-test.md` and the agent loads it
> when it receives a matching task.

---

## When to use this skill

Every time a new build of the `qc-tasks` app is deployed to staging, run this
skill to verify regressions on the core flows: **Login · Create · Cancel-delete · Filter**.

## Required tools

- `playwright-mcp` — to drive the browser.
- (Optional) `backlog-mcp` — to file issues for the bugs found.

## Spec (oracle for assertions)

| Action | Expected |
| --- | --- |
| Sign in with `qc@example.com` / `qc123` | Lands on the dashboard, header contains `"QC User"` |
| Create a valid task | Toast == `"Task created"` |
| Open delete modal → click **Cancel** | Row count is unchanged |
| Tick "Only show high priority" | Every visible row has priority badge == `"High"` |

## Steps

```yaml
- name: Setup
  steps:
    - navigate: "{{baseUrl}}/demo-app/#reset"
    - wait
```

</details>
