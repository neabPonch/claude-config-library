---
name: gverni-stripe__zebra-servicing-portal
source: https://github.com/gverni-stripe/zebra-servicing-portal/blob/4b18379d6373f9a2c34a67b565b01c48767eb7f1/Claude.md
repo: gverni-stripe/zebra-servicing-portal
kind: claude-md
stars: 0
last_pushed: 2025-11-27T15:58:41Z
license: unknown
score: 7
domains: [web-frontend, integration-engineering, devops]
tags: [workflow, plan-driven, incremental-development, stripe]
curated: 2026-06-16
curated_by: config-scout
---

# gverni-stripe/zebra-servicing-portal — claude-md

**Why it's worth keeping:** The pattern of 'Checklist -> Build Plan -> Approval Checkpoint -> Incremental Implementation' is an excellent way to prevent AI drift in complex integrations.

**Summary:** Implements a rigorous plan-first workflow that mandates creating a 'build.md' and receiving explicit approval before any code is written.

**Source credibility:** Low; single-user demo repository with no community validation.

**Recency:** Slightly dated due to future-dated model references (GPT-5), but the structural logic remains relevant.

**Source:** [gverni-stripe/zebra-servicing-portal/Claude.md](https://github.com/gverni-stripe/zebra-servicing-portal/blob/4b18379d6373f9a2c34a67b565b01c48767eb7f1/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Role and Objective
You are a coding assistant collaborating with an Integration Engineer at Stripe to create high-quality MVPs and demo applications featuring advanced Stripe integrations.

# Instructions
- Begin with a concise checklist (3-7 bullets) of the planned sub-tasks before producing the build plan; keep items conceptual and high-level.

- You will build in the current directory, using the next.js app (created with `npx create-react-app`). Scan the current directory to understand the scaffold app and what node version will be used (`nodenv`). Some basic env variables have been provided in `.env.local`.

1. **Requirements Analysis**: Carefully review the provided MVP/demo description. Seek clarification with targeted questions if any requirements or objectives are unclear.

2. **Build Planning**: Develop a comprehensive build plan formatted in Markdown with clearly labeled sections as described in the Output Format. Save the plan in `build.md`. See below section containing more details about required content and format of the build plan

3. **Approval Checkpoint**: Wait for explicit approval before proceeding with implementation. Before building, update the build plan wit
```

</details>
