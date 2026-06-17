---
name: bbatchelder__tap
source: https://github.com/bbatchelder/tap/blob/1b5bd2ce0625568602b84cc736940972b18cfc09/skill.md
repo: bbatchelder/tap
kind: skill
stars: 1
last_pushed: 2026-01-19T02:05:11Z
license: mit
score: 7
domains: [cli-tools, devops, agents-ai]
tags: [process-management, logging, debugging]
curated: 2026-06-14
curated_by: config-scout
---

# bbatchelder/tap — skill

**Why it's worth keeping:** It defines specific debugging workflows—such as using `--grep` or `--since`—that prevent agents from drowning in massive log outputs.

**Summary:** A guide for `tap`, a process supervisor that provides agents with structured ways to observe logs, search errors, and manage service lifecycles.

**Source credibility:** Low-star utility tool; likely a specialized developer productivity script.

**Recency:** Recent (5 months ago) and highly relevant to current agentic process management needs.

**Source:** [bbatchelder/tap/skill.md](https://github.com/bbatchelder/tap/blob/1b5bd2ce0625568602b84cc736940972b18cfc09/skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# tap - Process Supervisor for LLM Agents

You are using `tap`, a process supervisor with queryable logs. This guide helps you use tap effectively.

## Quick Reference

```bash
tap ls                                    # List all services
tap observe <svc> --last 50        # View last 50 log lines
tap observe <svc> --grep "error"   # Search logs for "error"
tap restart <svc>                  # Restart a service
tap status <svc>                   # Get detailed status
```

## When to Check Logs

- **After starting a server**: Verify it started successfully
- **When requests fail**: Check for errors in the service logs
- **After code changes**: Confirm hot reload worked (or restart if needed)
- **Debugging issues**: Search logs with `--grep`

## Common Patterns

### Check if a service is running
```bash
tap ls
```
Look at the STATE column. "running" means healthy.

### View recent errors
```bash
tap observe website --last 100 --grep "error" --regex
```

### Check logs from the last 5 minutes
```bash
tap observe website --since 5m
```

### View only stderr (errors/warnings)
```bash
tap observe website --stream stderr --last 50
```

## When to Restart Services

Not all services hot-rel
```

</details>
