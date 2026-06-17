---
name: PatchyVideo__Touhou-Vote
source: https://github.com/PatchyVideo/Touhou-Vote/blob/5069ec640b54dc413148a61275b4fefaaa0c5bc8/CLAUDE.md
repo: PatchyVideo/Touhou-Vote
kind: claude-md
stars: 32
last_pushed: 2026-06-10T15:25:20Z
license: gpl-3.0
score: 8
domains: [agents-ai, cli-tools, devops]
tags: [skill-routing, orchestration, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# PatchyVideo/Touhou-Vote — claude-md

**Why it's worth keeping:** The 'Skill routing' pattern is a highly transferable technique for transforming an AI from a generic assistant into a structured orchestrator of complex, multi-step organizational tasks.

**Summary:** Implements an intent-mapping system that routes user requests to specialized 'skills' with predefined workflows and quality gates.

**Source credibility:** The content demonstrates high-level agentic orchestration patterns used in advanced developer toolchains.

**Recency:** Current; reflects modern 'agent-as-an-orchestrator' paradigms for AI coding tools.

**Source:** [PatchyVideo/Touhou-Vote/CLAUDE.md](https://github.com/PatchyVideo/Touhou-Vote/blob/5069ec640b54dc413148a61275b4fefaaa0c5bc8/CLAUDE.md) · 32★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## gstack (REQUIRED — global install)

**Before doing ANY work, verify gstack is installed:**

```bash
test -d ~/.claude/skills/gstack/bin && echo "GSTACK_OK" || echo "GSTACK_MISSING"
```

If GSTACK_MISSING: STOP. Do not proceed. Tell the user:

> gstack is required for all AI-assisted work in this repo.
> Install it:
> ```bash
> git clone --depth 1 https://github.com/garrytan/gstack.git ~/.claude/skills/gstack
> cd ~/.claude/skills/gstack && ./setup --team
> ```
> Then restart your AI coding tool.

Do not skip skills, ignore gstack errors, or work around missing gstack.

Using gstack skills: After install, skills like /qa, /ship, /review, /investigate,
and /browse are available. Use /browse for all web browsing.
Use ~/.claude/skills/gstack/... for gstack file paths (the global path).

## Skill routing

When the user's request matches an available skill, invoke it via the Skill tool. The
skill has multi-step workflows, checklists, and quality gates that produce better
results than an ad-hoc answer. When in doubt, invoke the skill. A false positive is
cheaper than a false negative.

Key routing rules:
- Product ideas, "is this worth building", brainstorming → invoke /office-hours
-
```

</details>
