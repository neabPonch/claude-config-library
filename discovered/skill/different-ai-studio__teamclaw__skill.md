---
name: different-ai-studio__teamclaw__skill
source: https://github.com/different-ai-studio/teamclaw/blob/cc145f70d4ffa86626901191b50b8427549ba5e1/.claude/skills/sentry-monitor/SKILL.md
repo: different-ai-studio/teamclaw
kind: skill
stars: 229
last_pushed: 2026-05-16T15:18:49Z
license: mit
score: 8
domains: [observability, devops, automation, cli-tools]
tags: [sentry, monitoring, root-cause-analysis]
curated: 2026-06-15
curated_by: config-scout
---

# different-ai-studio/teamclaw — skill

**Why it's worth keeping:** Demonstrates a sophisticated 'observability-to-codebase' loop where the agent uses stack traces to navigate and interpret actual files. It also provides clear instructions for parallelizing sub-tasks using subagents.

**Summary:** Automates Sentry issue monitoring by fetching error details, performing local root cause analysis via source code inspection, and posting structured reports to WeCom.

**Source credibility:** High; 229 stars on GitHub indicates this is a vetted toolset from an active development studio.

**Recency:** Current; utilizes modern agentic orchestration patterns like parallel execution and multi-tool integration.

**Source:** [different-ai-studio/teamclaw/.claude/skills/sentry-monitor/SKILL.md](https://github.com/different-ai-studio/teamclaw/blob/cc145f70d4ffa86626901191b50b8427549ba5e1/.claude/skills/sentry-monitor/SKILL.md) · 229★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sentry-monitor
description: Use when the user wants to check Sentry issues, run a Sentry daily report, or monitor error trends. Triggers on "sentry 监控", "sentry 日报", "查看 sentry", "sentry report", "sentry monitor".
---

# Sentry Monitor — Daily Issue Report

Scan both TeamClaw Sentry projects for unresolved fatal/high issues, analyze root causes, and push a summary report to WeCom.

## Projects

| Project | Sentry Slug | Platform |
|---------|-------------|----------|
| Rust backend | `ucar-inc/teamclaw` | Rust |
| React frontend | `ucar-inc/teamclaw-react` | JavaScript React |

## Execution Steps

### 1. Scan Issues

Run these two commands in parallel:

```bash
sentry issue list ucar-inc/teamclaw --query "is:unresolved" --json --fields shortId,title,priority,level,status --limit 20
```

```bash
sentry issue list ucar-inc/teamclaw-react --query "is:unresolved" --json --fields shortId,title,priority,level,status --limit 20
```

Filter results: keep only issues where `level` is `fatal` OR `priority` is `high`.

If no issues match, skip to step 4 with "全部正常" message.

### 2. Analyze Root Causes (Local)

For each filtered issue (max 10 total), perform local root cause analysis
```

</details>
