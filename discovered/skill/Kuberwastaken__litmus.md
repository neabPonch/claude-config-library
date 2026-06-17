---
name: Kuberwastaken__litmus
source: https://github.com/Kuberwastaken/litmus/blob/225f0c2b86b48b608fdee07095f71047a8ada6c1/SKILL.md
repo: Kuberwastaken/litmus
kind: skill
stars: 70
last_pushed: 2026-03-28T18:15:42Z
license: mit
score: 9
domains: [ml-research, autonomous-agents, orchestration]
tags: [git-worktrees, knowledge-distillation, parallel-agents]
curated: 2026-06-14
curated_by: config-scout
---

# Kuberwastaken/litmus — skill

**Why it's worth keeping:** Uses git worktrees for efficient cross-agent code sharing/inspection; implements a high-level orchestration pattern (Director/Synthesizer) to turn raw experiment logs into reusable, persistent skills.

**Summary:** An autonomous ML research framework that uses Git worktrees to manage parallel agent experiments and a 'Skills Library' for knowledge distillation.

**Source credibility:** Established niche tool with 70 stars and recent activity.

**Recency:** Highly current; leverages advanced subagent spawning and session management patterns.

**Source:** [Kuberwastaken/litmus/SKILL.md](https://github.com/Kuberwastaken/litmus/blob/225f0c2b86b48b608fdee07095f71047a8ada6c1/SKILL.md) · 70★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: litmus
version: 1.1.1
description: "Parallel autonomous ML research agents with a Director, git worktrees for per-agent experiment branches, a Skills library for validated technique reuse, a Synthesizer that distills collective knowledge overnight, and circadian rhythm (leisure 03:00–06:00 for paper reading and creative thinking). Uses OpenClaw sessions_spawn, cron, and steer natively. Use when: (1) start or run ML research agents overnight, (2) check agent status or experiment results, (3) view leaderboard or morning digest, (4) steer or stop agents, (5) ask what agents discovered or are exploring, (6) set up Litmus for the first time. NOT for: general coding, non-ML tasks, or machines without a GPU."
homepage: https://github.com/kuberwastaken/litmus
source: https://github.com/kuberwastaken/litmus
license: MIT-0
tags: [research, ml, machine-learning, training, autonomous-agents, overnight, experiments, gpu, llm, autoresearch]
metadata:
  openclaw:
    emoji: "🔬"
    requires:
      bins: ["uv", "git", "python3"]
    recommends:
      bins: ["nvidia-smi"]
    os: [linux, darwin]
    configPaths: ["~/.litmus/"]
    optional:
      env: ["CLAWRXIV_API_KEY"]
---

# Litmus —
```

</details>
