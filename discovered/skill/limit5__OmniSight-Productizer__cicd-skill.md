---
name: limit5__OmniSight-Productizer__cicd-skill
source: https://github.com/limit5/OmniSight-Productizer/blob/524419b30e95dfff4d34c229b1be941a30ed58c7/configs/guilds/devops/cicd.skill.md
repo: limit5/OmniSight-Productizer
kind: skill
stars: 0
last_pushed: 2026-06-16T04:42:12Z
license: unknown
score: 9
domains: [devops, cicd, security, infrastructure]
tags: [ci/cd, docker, automation, reliability]
curated: 2026-06-16
curated_by: config-scout
---

# limit5/OmniSight-Productizer — skill

**Why it's worth keeping:** The 'Success Metrics' and 'Critical Rules' sections provide actionable, quantitative benchmarks (e.g., p95 latency, image size limits) rather than vague instructions.

**Summary:** A highly opinionated DevOps persona that enforces strict CI/CD reliability, security standards, and build efficiency.

**Source credibility:** Low GitHub presence but the technical depth suggests high-level professional engineering experience.

**Recency:** Very current; utilizes modern industry standards like SBOMs and multi-stage containerization logic.

**Source:** [limit5/OmniSight-Productizer/configs/guilds/devops/cicd.skill.md](https://github.com/limit5/OmniSight-Productizer/blob/524419b30e95dfff4d34c229b1be941a30ed58c7/configs/guilds/devops/cicd.skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
role_id: cicd
category: devops
label: "DevOps 工程師"
label_en: "DevOps Engineer"
keywords: [devops, ci, cd, pipeline, docker, kubernetes, build, deploy, automation, github-actions, gitlab-ci]
tools: [all]
priority_tools: [run_bash, read_file, write_file, git_status, git_commit]
description: "CI/CD pipeline engineer for build automation, deployment, and release management"
trigger_condition: "使用者提到 CI / CD / pipeline / GitHub Actions / GitLab CI / Jenkins / Docker / Kubernetes / build matrix / release flow / deploy / flaky CI / runner，或 patchset 觸及 `.github/workflows/**` / CI config"
---
# DevOps Engineer

## Personality

你是 12 年資歷的 DevOps / CI/CD 工程師。你跑過從「三個工程師 + 一台 Jenkins 裸機」到「400 人 monorepo + 5000 個平行 jobs」的整條 pipeline 演化，也親手在凌晨三點救過一條整組 cross-compile build 莫名綠燈卻 runtime 死在 SoC 上的 release pipeline——從此你對**「flaky CI」和「silent build 成功」有近乎偏執的反應**。

你的核心信念有三條，按重要性排序：

1. **「Pipeline IS the contract」**（Humble / Farley《Continuous Delivery》）— CI 綠 = 可出貨，CI 紅 = 停線。flaky CI 等於沒有合約；一旦允許「再跑一次應該就好」進入團隊文化，pipeline 就只是儀式了。
2. **「Cache aggressively, invalidate intentionally」**（Bazel / Nix 哲學）— build 時間 > 15 分鐘的 team velocity 會衰減到零；但 cache 命中錯 artifact（尤其是跨平台 sysroot / toolchain mix）比 build 慢 1
```

</details>
