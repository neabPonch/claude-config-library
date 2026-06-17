---
name: windmill-labs__windmill__skill
source: https://github.com/windmill-labs/windmill/blob/dd7d8c2d47f49fd8c3984b1edad527ecc3670198/system_prompts/auto-generated/skills/write-script-deno/SKILL.md
repo: windmill-labs/windmill
kind: skill
stars: 16775
last_pushed: 2026-06-15T09:02:15Z
license: other
score: 9
domains: [cli-tools, backend-api, devops]
tags: [deno, typescript, windmill, workflow-engine]
curated: 2026-06-15
curated_by: config-scout
---

# windmill-labs/windmill — skill

**Why it's worth keeping:** The 'Preview vs Run' heuristic provides excellent intent-based logic to prevent accidental deployments. Embedding the full `windmill-client` API ensures the agent doesn't hallucinate or default to unreliable `fetch` calls.

**Summary:** Provides highly specific CLI workflows and SDK documentation for writing, testing, and deploying Deno/TypeScript scripts on the Windmill platform.

**Source credibility:** High; Windmill is a major, highly-starred (16k+) developer platform with active maintenance.

**Recency:** Current; includes modern Deno/npm import patterns and specific workflow instructions for agentic execution.

**Source:** [windmill-labs/windmill/system_prompts/auto-generated/skills/write-script-deno/SKILL.md](https://github.com/windmill-labs/windmill/blob/dd7d8c2d47f49fd8c3984b1edad527ecc3670198/system_prompts/auto-generated/skills/write-script-deno/SKILL.md) · 16775★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: write-script-deno
description: MUST use when writing Deno/TypeScript scripts.
---

## CLI Commands

Place scripts in a folder.

After writing, tell the user which command fits what they want to do:

- `wmill script preview <script_path>` — **default when iterating on a local script.** Runs the local file without deploying.
- `wmill script run <path>` — runs the script **already deployed** in the workspace. Use only when the user explicitly wants to test the deployed version, not local edits.
- `wmill generate-metadata` — generate `.script.yaml` and `.lock` files for the script you modified.
- `wmill sync push` — deploy local changes to the workspace. Only suggest/run this when the user explicitly asks to deploy/publish/push — not when they say "run", "try", or "test".

### Preview vs run — choose by intent, not habit

If the user says "run the script", "try it", "test it", "does it work" while there are **local edits to the script file**, use `script preview`. Do NOT push the script to then `script run` it — pushing is a deploy, and deploying just to test overwrites the workspace version with untested changes.

Only use `script run` when:
- The user explicitly says "run t
```

</details>
