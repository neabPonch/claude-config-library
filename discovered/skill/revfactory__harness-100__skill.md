---
name: revfactory__harness-100__skill
source: https://github.com/revfactory/harness-100/blob/8e8d35c6a19166614d1af1df85512266d51121ae/en/20-cicd-pipeline/.claude/skills/cicd-pipeline/skill.md
repo: revfactory/harness-100
kind: skill
stars: 972
last_pushed: 2026-03-22T22:42:10Z
license: apache-2.0
score: 9
domains: [devops, cicd, agents-ai, security]
tags: [pipeline-automation, multi-agent, orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# revfactory/harness-100 — skill

**Why it's worth keeping:** It implements 'Mode by Task Scale' to optimize agent deployment based on request complexity and uses a structured '_workspace/' directory pattern for robust state handoff between specialized agents.

**Summary:** A sophisticated multi-agent orchestration framework for end-to-end CI/CD pipeline lifecycle management.

**Source credibility:** High; the repository has significant social proof with 972 stars and professional-grade documentation.

**Recency:** Current; the multi-agent orchestration patterns are highly applicable to modern Claude Code workflows.

**Source:** [revfactory/harness-100/en/20-cicd-pipeline/.claude/skills/cicd-pipeline/skill.md](https://github.com/revfactory/harness-100/blob/8e8d35c6a19166614d1af1df85512266d51121ae/en/20-cicd-pipeline/.claude/skills/cicd-pipeline/skill.md) · 972★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cicd-pipeline
description: "Full pipeline for CI/CD pipeline design, build, monitoring, and optimization. An agent team collaborates to perform stage design, YAML configuration generation, security scan integration, and monitoring/alert design. Use this skill for any CI/CD task including 'create a CI/CD pipeline', 'GitHub Actions', 'GitLab CI', 'Jenkins pipeline', 'deployment automation', 'build pipeline', 'DevOps pipeline', 'auto deploy', 'CI setup', 'CD setup', etc. Also supports optimization and security hardening for existing pipelines. Note: actual infrastructure provisioning (AWS/GCP resource creation), server configuration, and cluster management are outside the scope of this skill."
---

# CI/CD Pipeline — Pipeline Design, Build, Monitoring, and Optimization

An agent team collaborates to perform CI/CD pipeline design, configuration generation, security integration, and monitoring in a single pass.

## Execution Mode

**Agent Team** — 5 members communicate directly via SendMessage and cross-validate each other's work.

## Agent Composition

| Agent | File | Role | Type |
|-------|------|------|------|
| pipeline-designer | `.claude/agents/pipeline-designer.md` | S
```

</details>
