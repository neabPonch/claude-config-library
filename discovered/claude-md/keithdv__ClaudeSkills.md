---
name: keithdv__ClaudeSkills
source: https://github.com/keithdv/ClaudeSkills/blob/b691bd90d6ea919fe5dd101a674853af1689081d/CLAUDE.md
repo: keithdv/ClaudeSkills
kind: claude-md
stars: 0
last_pushed: 2026-06-01T02:25:10Z
license: unknown
score: 9
domains: [backend, devops, testing, agents-ai]
tags: [agent-orchestration, build-optimization, tdd, dotnet]
curated: 2026-06-14
curated_by: config-scout
---

# keithdv/ClaudeSkills — claude-md

**Why it's worth keeping:** The protocol for redirecting large outputs to log files to prevent truncation is a brilliant, highly practical trick. It also includes strong guardrails against 'gutting' tests or working around bugs to maintain code integrity.

**Summary:** A highly opinionated instruction set that focuses on agent-orchestration boundaries and technical protocols for build/test reliability.

**Source credibility:** Low star count, but the extreme specificity regarding build logs and agent behavior suggests high-level engineering expertise.

**Recency:** Very current; addresses modern agentic workflow challenges like output truncation and subagent management.

**Source:** [keithdv/ClaudeSkills/CLAUDE.md](https://github.com/keithdv/ClaudeSkills/blob/b691bd90d6ea919fe5dd101a674853af1689081d/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---

## Core Rules

- **STOP and ask** when you hit an obstacle - don't push through with workarounds
- **STOP and ask** before reverting, undoing, or changing direction
- **STOP and ask** before modifying out-of-scope tests
- **STOP and ask** before using reflection
- **STOP and ask** when a required agent (e.g., `crm-architect`) is not available as a Task subagent — do NOT substitute a general-purpose agent or work around it
- **NEVER take over for an agent.** If an agent appears stuck, slow, or unresponsive — STOP and ask for direction. Do NOT kill the agent and do the work yourself. Do NOT read source files "to take over." The orchestrator never modifies source code. Always wait for the user, even if they are away.

---

## ALWAYS Capture Build and Test Output to a File

**Builds and tests produce large output that gets truncated when piped through `tail`, `grep`, or the harness's task-output buffer.** Re-running a build or test because you couldn't find the failure in truncated output is the single most expensive mistake you can make — it wastes minutes per cycle and trains the user to distrust you.

**The rule:**

```bash
dotnet build > /tmp/build.log 2>&1
dotnet test --no-bu
```

</details>
