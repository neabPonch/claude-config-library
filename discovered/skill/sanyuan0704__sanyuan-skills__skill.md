---
name: sanyuan0704__sanyuan-skills__skill
source: https://github.com/sanyuan0704/sanyuan-skills/blob/08b6572ef108f22d4e8a3ecf9182a4bbef097744/skills/sigma/SKILL.md
repo: sanyuan0704/sanyuan-skills
kind: skill
stars: 3643
last_pushed: 2026-05-11T07:21:45Z
license: mit
score: 9
domains: [education, learning-systems]
tags: [tutor, mastery-learning, socratic, stateful-agent]
curated: 2026-06-15
curated_by: config-scout
---

# sanyuan0704/sanyuan-skills — skill

**Why it's worth keeping:** It utilizes the file system to create sophisticated long-term memory (cross-topic profiles) and structured short-term state. The workflow demonstrates advanced agentic patterns: diagnosis, roadmap generation, and strict mastery gating.

**Summary:** A stateful Socratic tutor implementing Bloom’s mastery learning through persistent local file storage for learner profiles and session progress.

**Source credibility:** High; 3600+ stars indicates a widely used and proven skill set.

**Recency:** Current; utilizes modern Claude Code capabilities like AskUserQuestion and structured file-system workflows.

**Source:** [sanyuan0704/sanyuan-skills/skills/sigma/SKILL.md](https://github.com/sanyuan0704/sanyuan-skills/blob/08b6572ef108f22d4e8a3ecf9182a4bbef097744/skills/sigma/SKILL.md) · 3643★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sigma
description: "Personalized 1-on-1 AI tutor using Bloom's 2-Sigma mastery learning. Guides users through any topic with Socratic questioning, adaptive pacing, and rich visual output (HTML dashboards, Excalidraw concept maps, generated images). Use when user wants to learn something, study a topic, understand a concept, requests tutoring, says 'teach me', 'I want to learn', 'explain X to me step by step', 'help me understand', or invokes /sigma. Triggers on: learn, study, teach, tutor, understand, master, explain step by step."
---

# Sigma Tutor

Personalized 1-on-1 mastery tutor. Bloom's 2-Sigma method: diagnose, question, advance only on mastery.

## Usage

```bash
/sigma Python decorators
/sigma 量子力学 --level beginner
/sigma React hooks --level intermediate --lang zh
/sigma linear algebra --resume    # Resume previous session
```

## Arguments

| Argument | Description |
|----------|-------------|
| `<topic>` | Subject to learn (required, or prompted) |
| `--level <level>` | Starting level: beginner, intermediate, advanced (default: diagnose) |
| `--lang <code>` | Language override (default: follow user's input language) |
| `--resume` | Resume previous session fro
```

</details>
