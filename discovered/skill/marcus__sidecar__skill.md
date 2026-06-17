---
name: marcus__sidecar__skill
source: https://github.com/marcus/sidecar/blob/ca6814d35c82687a10bf07b1b206d68f2b43a5b8/.claude/skills/profile-memory/SKILL.md
repo: marcus/sidecar
kind: skill
stars: 1026
last_pushed: 2026-06-09T03:30:32Z
license: mit
score: 9
domains: [systems-programming, go-backend, cli-tools]
tags: [profiling, memory-leak, pprof, debugging, go]
curated: 2026-06-15
curated_by: config-scout
---

# marcus/sidecar — skill

**Why it's worth keeping:** Provides actionable triage tables, specific 'red flag' thresholds (e.g., thread counts, VM regions), and high-value snapshot comparison workflows.

**Summary:** A comprehensive debugging playbook for profiling Go memory, CPU, and file descriptor usage using system-level tools and pprof.

**Source credibility:** High; 1k+ stars and extremely active maintenance/recent pushes.

**Recency:** Current; reflects modern Go runtime debugging and macOS/Linux system tool patterns.

**Source:** [marcus/sidecar/.claude/skills/profile-memory/SKILL.md](https://github.com/marcus/sidecar/blob/ca6814d35c82687a10bf07b1b206d68f2b43a5b8/.claude/skills/profile-memory/SKILL.md) · 1026★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: profile-memory
description: >
  Profile memory usage in sidecar using Go pprof, system tools, and heap analysis.
  Covers identifying memory leaks, goroutine leaks, file descriptor accumulation,
  and CPU profiling. Use when investigating memory issues, profiling performance,
  debugging memory leaks, or diagnosing unresponsive plugins.
disable-model-invocation: true
---

# Memory Profiling for Sidecar

## Quick Triage

| Symptom | Tool | Action |
|---------|------|--------|
| High RSS / memory growth | vmmap, pprof heap | Check system memory, then heap profile |
| Too many open files | lsof | Check FD count and breakdown |
| High CPU | pprof cpu, ps | Capture CPU profile |
| Goroutine leak | pprof goroutines | Check goroutine count and stacks |
| Plugin unresponsive | lsof + goroutines | Check SQLite locks, blocked goroutines |

```
Triage flow: Is RSS high? -> Check FD count -> Check vmmap -> Check heap profile
```

## System-Level Profiling (No pprof Required)

### Find the Process

```bash
pgrep -f sidecar
ps aux | grep sidecar
```

### Basic Stats

```bash
# RSS, VSZ, CPU%, thread count
ps -o pid,rss,vsz,%cpu,nlwp -p <PID>

# Human-readable RSS
ps -o pid,rss -p <PID>
```

</details>
