---
name: m-sec-org__BreachWeave__skill
source: https://github.com/m-sec-org/BreachWeave/blob/ceac953dc501fe98f7ddbec2c1eeb0fe2993aff3/packages/core/src/config/skills/builtin/payloads-everything/SKILL.md
repo: m-sec-org/BreachWeave
kind: skill
stars: 369
last_pushed: 2026-05-06T12:29:40Z
license: apache-2.0
score: 8
domains: [security, cli-tools, knowledge-navigation]
tags: [pentesting, payloads, hierarchical-search]
curated: 2026-06-17
curated_by: config-scout
---

# m-sec-org/BreachWeave — skill

**Why it's worth keeping:** The 'README-first' drill-down methodology and specific command patterns (using find, sed, and rg with scope limits) are highly transferable to any large documentation repository.

**Summary:** Provides a structured, hierarchical navigation strategy for exploring massive local knowledge bases (like security payloads) without exhausting context windows.

**Source credibility:** Strong; part of a specialized security agent project with significant community interest.

**Recency:** Current; utilizes modern CLI tools like ripgrep (rg) standard in Claude Code environments.

**Source:** [m-sec-org/BreachWeave/packages/core/src/config/skills/builtin/payloads-everything/SKILL.md](https://github.com/m-sec-org/BreachWeave/blob/ceac953dc501fe98f7ddbec2c1eeb0fe2993aff3/packages/core/src/config/skills/builtin/payloads-everything/SKILL.md) · 369★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: payloads-all-the-things
description: Browse the bundled PayloadsAllTheThings corpus for CTF and web security payloads, bypasses, fuzz strings, exploit ideas, and methodology notes. Use when Agent needs to locate payloads by vulnerability category during CTFs, pentests, or challenge solving, then drill into the relevant README.md and markdown files under references/ instead of loading the whole corpus at once.
---

# PayloadsAllTheThings Local Navigator

把 `references/` 当作本地只读 payload 知识库。

按下面的顺序工作，不要一次性读取整个语料库：

1. 先看一级目录，按漏洞类型缩小范围。
2. 进入目标目录后先读该目录的 `README.md`，它通常会概述这个类目的 payload、利用技巧、绕过思路、工具和实验环境。
3. 再查看同级的具体 `*.md`、`Intruder/`、`Images/`、`Configuration*`、`CVE*` 或其他子目录。
4. 只在当前类目内使用 `rg -n` 搜关键词，避免全仓库大范围搜索。
5. 输出 payload 或技巧时，带上来源路径，便于继续深入。

优先使用这些命令：

```bash
find references -maxdepth 1 -mindepth 1 -type d -exec basename {} \; | sort
sed -n '1,200p' 'references/SQL Injection/README.md'
find 'references/SQL Injection' -maxdepth 1 \( -type f -o -type d \) | sort
rg -n 'union|time based|auth bypass' 'references/SQL Injection'
sed -n '1,200p' 'references/Server Side Request Forgery/README.md'
rg -n 'gopher|metadata|redirect|localhost' 'references/Server Side Request Forger
```

</details>
