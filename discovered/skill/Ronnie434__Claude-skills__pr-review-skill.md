---
name: Ronnie434__Claude-skills__pr-review-skill
source: https://github.com/Ronnie434/Claude-skills/blob/fe8b397d17ddf46f087c091a3ac3ebb71582634a/pr-review-skill.md
repo: Ronnie434/Claude-skills
kind: skill
stars: 0
last_pushed: 2026-02-26T22:06:07Z
license: unknown
score: 8
domains: [software-engineering, security, devops]
tags: [code-review, pr-review, qa]
curated: 2026-06-16
curated_by: config-scout
---

# Ronnie434/Claude-skills — skill

**Why it's worth keeping:** The use of weighted review phases (Phase 2) and highly granular, language-specific checklists provides deep technical coverage. The standardized output format ensures the agent provides actionable, professional feedback rather than generic praise.

**Summary:** A highly structured framework for systematic pull request reviews that prioritizes agent effort toward high-risk areas like security and correctness.

**Source credibility:** Low social proof due to zero stars, but the high technical density suggests expert authorship.

**Recency:** Current and highly applicable to modern agentic coding workflows.

**Source:** [Ronnie434/Claude-skills/pr-review-skill.md](https://github.com/Ronnie434/Claude-skills/blob/fe8b397d17ddf46f087c091a3ac3ebb71582634a/pr-review-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pr-review
description: Expert-level pull request code review for AI agentic development. Triggers when reviewing PRs, diffs, changesets, merge requests, or code changes. Performs comprehensive analysis covering correctness, security vulnerabilities, performance, maintainability, testing, and adherence to best practices. Use for GitHub PRs, GitLab MRs, Bitbucket PRs, or any diff-based code review workflow. Supports all major languages including TypeScript, JavaScript, Python, Go, Rust, Java, and more.
---

# PR Review Skill

Expert-level code review for pull requests and changesets.

## Review Workflow

### Phase 1: Context Gathering

Before reviewing, gather essential context:

1. **PR Metadata**: Title, description, linked issues, labels
2. **Changed Files**: List all modified, added, deleted files
3. **Diff Size**: Assess scope (small <100 lines, medium 100-500, large >500)
4. **PR Type**: Feature, bugfix, refactor, dependency update, config change

### Phase 2: Systematic Review

Review in this order, spending proportional effort:

```
1. Critical Path (40% effort)
   └── Security → Data handling → Auth/authz → Input validation

2. Correctness (30% effort)
   └── Logic
```

</details>
