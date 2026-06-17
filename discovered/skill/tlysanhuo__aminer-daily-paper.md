---
name: tlysanhuo__aminer-daily-paper
source: https://github.com/tlysanhuo/aminer-daily-paper/blob/2bcf5dcb1161a85904b06ba9c5cca0dcaaf1533d/SKILL.md
repo: tlysanhuo/aminer-daily-paper
kind: skill
stars: 483
last_pushed: 2026-06-15T12:19:52Z
license: mit
score: 8
domains: [agents-ai, cli-tools, data-pipeline]
tags: [research, recommendation, workflow-automation]
curated: 2026-06-16
curated_by: config-scout
---

# tlysanhuo/aminer-daily-paper — skill

**Why it's worth keeping:** The 'Contract' section is an excellent template for defining how an agent should interpret specific return codes (like NO_REPLY) to handle side-effect heavy actions without unnecessary chatter.

**Summary:** A specialized skill for a research paper recommendation pipeline that integrates AMiner and arXiv with Feishu card dispatching.

**Source credibility:** Strong; the repository has significant stars and high recent activity/maintenance.

**Recency:** Current; uses highly effective agency patterns for tool output interpretation.

**Source:** [tlysanhuo/aminer-daily-paper/SKILL.md](https://github.com/tlysanhuo/aminer-daily-paper/blob/2bcf5dcb1161a85904b06ba9c5cca0dcaaf1533d/SKILL.md) · 483★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aminer-rec5
description: "OpenClaw personalized paper recommendation skill. When the user invokes /aminer-rec5 or /skill aminer-rec5 in Feishu, immediately run the local pipeline under {baseDir}/scripts/, accept aminer_user_id, scholar hints, seed paper titles, papers_file, or free-form topic text, build a unified ResearchProfile, retrieve papers, enrich with AMiner, dispatch Feishu cards, and return NO_REPLY."
homepage: https://github.com/tlysanhuo/aminer-rec
user-invocable: true
disable-model-invocation: false
metadata: { "openclaw": { "emoji": "📚", "requires": { "bins": ["python3"] } } }
---

# aminer-rec5

Use this skill only for explicit `/aminer-rec5` or `/skill aminer-rec5` requests.

## Contract

- Every explicit invocation is a new run.
- Do not answer with status-only text.
- Do not search, install, or repair skills.
- After running `handle_trigger.py`, check `final_response` in the JSON output:
  - `NO_REPLY` → Feishu cards were dispatched successfully. Return exactly `NO_REPLY`.
  - `TEXT` → No Feishu target available. Present the `reply_text` value directly to the user.
  - Any error → Report the `reply_text` or error detail to the user.

## Inputs

- `aminer
```

</details>
