---
name: motiondivision__motion__skill
source: https://github.com/motiondivision/motion/blob/0c6ba08c8eb0e91bfb632f97d30efe901c46d9ca/.agents/skills/fix/SKILL.md
repo: motiondivision/motion
kind: skill
stars: 32347
last_pushed: 2026-06-12T09:22:29Z
license: mit
score: 9
domains: [web-frontend, software-engineering]
tags: [tdd, plan-driven, github-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# motiondivision/motion — skill

**Why it's worth keeping:** It utilizes a 'Plan vs. Executor' separation of concerns, mandates a failing test before implementation, and includes explicit stop conditions to prevent hallucinated fixes or scope creep.

**Summary:** A high-discipline execution skill that transforms plans or issues into verified PRs using a strict TDD and multi-environment verification workflow.

**Source credibility:** High; part of the professional Motion/Framer Motion repository ecosystem.

**Recency:** Current; incorporates modern tech requirements like React 18/19 and Vite recipes.

**Source:** [motiondivision/motion/.agents/skills/fix/SKILL.md](https://github.com/motiondivision/motion/blob/0c6ba08c8eb0e91bfb632f97d30efe901c46d9ca/.agents/skills/fix/SKILL.md) · 32347★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: fix
description: Take a GitHub issue, an open PR, or a plan file from plans/ and drive it to a merge-ready PR — reproduce with a failing test first, implement the fix (bugs) or feature (plans), verify against the repo's gates, and open or update the PR. Use when asked to fix an issue, implement or execute a plan, finish or land an open PR, or work through plans/issues/.
metadata:
  author: mattgperry
  version: "1.0.0"
---

# Fix

You are the **executor**. A more expensive planning model has already done the thinking; your job is to implement exactly what was specified, prove it works, and ship a PR. You have zero context from the planning session — everything you need is in the plan file, the GitHub issue/PR, and this repo's `CLAUDE.md`. Read all three before writing any code.

## Resolving the input

The argument can be:

1. **A plan file path** (e.g. `plans/issues/pr-3724.md` or `plans/001-animate-layout-public-api.md`) — read it in full. Plans are the primary input for this skill.
2. **A plan number** (e.g. `008`) — find the matching file in `plans/` or `plans/issues/`.
3. **A GitHub issue number** (e.g. `#3741`) — run `gh issue view <number>` first. Check whether a p
```

</details>
