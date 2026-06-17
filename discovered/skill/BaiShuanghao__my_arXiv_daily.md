---
name: BaiShuanghao__my_arXiv_daily
source: https://github.com/BaiShuanghao/my_arXiv_daily/blob/e82cd303d8a9b5855781108be0d3b6f21263162c/skill.md
repo: BaiShuanghao/my_arXiv_daily
kind: skill
stars: 188
last_pushed: 2026-06-15T13:53:20Z
license: apache-2.0
score: 9
domains: [agents-ai, cli-tools, prompt-engineering]
tags: [meta-skill, optimization, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# BaiShuanghao/my_arXiv_daily — skill

**Why it's worth keeping:** Introduces advanced techniques like 'Progressive Disclosure' for managing context limits and provides tactical advice on preventing skill 'undertriggering' by using pushy descriptions.

**Summary:** A meta-skill designed to guide users through the end-to-end lifecycle of creating, testing, and optimizing Claude Code skills.

**Source credibility:** High-quality content; while the repo name is generic, the technical depth suggests an expert understanding of agentic workflows.

**Recency:** Highly current; specifically tailored to the Claude Code/MCP ecosystem and modern context management needs.

**Source:** [BaiShuanghao/my_arXiv_daily/skill.md](https://github.com/BaiShuanghao/my_arXiv_daily/blob/e82cd303d8a9b5855781108be0d3b6f21263162c/skill.md) · 188★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: skill-creator
description: Create new skills, modify and improve existing skills, and measure skill performance. Use when users want to create a skill from scratch, edit, or optimize an existing skill, run evals to test a skill, benchmark skill performance with variance analysis, or optimize a skill's description for better triggering accuracy.
---

# Skill Creator

A skill for creating new skills and iteratively improving them.

At a high level, the process of creating a skill goes like this:

- Decide what you want the skill to do and roughly how it should do it
- Write a draft of the skill
- Create a few test prompts and run claude-with-access-to-the-skill on them
- Help the user evaluate the results both qualitatively and quantitatively
  - While the runs happen in the background, draft some quantitative evals if there aren't any (if there are some, you can either use as is or modify if you feel something needs to change about them). Then explain them to the user (or if they already existed, explain the ones that already exist)
  - Use the `eval-viewer/generate_review.py` script to show the user the results for them to look at, and also let them look at the quantitati
```

</details>
