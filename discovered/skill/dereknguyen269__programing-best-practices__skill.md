---
name: dereknguyen269__programing-best-practices__skill
source: https://github.com/dereknguyen269/programing-best-practices/blob/ed6f347670079444d4cf88ae344843ff757a1068/skills/best-practices/SKILL.md
repo: dereknguyen269/programing-best-practices
kind: skill
stars: 661
last_pushed: 2026-02-18T09:59:46Z
license: unlicense
score: 8
domains: [cli-tools, knowledge-retrieval, software-engineering]
tags: [search-workflow, best-practices, structured-retrieval]
curated: 2026-06-16
curated_by: config-scout
---

# dereknguyen269/programing-best-practices — skill

**Why it's worth keeping:** It implements a highly specific 'Analyze -> Search (with flags) -> Read' workflow that ensures agents prioritize high-authority data over general training knowledge. The use of command-line arguments like --recommend and --domain provides granular control over information retrieval depth.

**Summary:** A structured tool-use protocol that leverages a custom search script to navigate a curated knowledge base of industry programming standards.

**Source credibility:** High; the source repository is well-regarded with 661 stars.

**Recency:** Current; utilizes modern CLI patterns suitable for agentic tool execution.

**Source:** [dereknguyen269/programing-best-practices/skills/best-practices/SKILL.md](https://github.com/dereknguyen269/programing-best-practices/blob/ed6f347670079444d4cf88ae344843ff757a1068/skills/best-practices/SKILL.md) · 661★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
inclusion: auto
---

# best-practices

Searchable knowledge base of 152+ programming best practices across 30+ languages and frameworks. BM25-powered search over curated resources from industry leaders (Google, Airbnb, Uber, Mozilla, Shopify, OWASP).

## Prerequisites

Python 3 must be installed:

```bash
python3 --version
```

## How to Use This Workflow

When user asks about coding standards, best practices, style guides, code review, architecture, security, or performance for any language/framework, follow this workflow:

### Step 1: Analyze User Requirements

Extract from user request:
- **Language/Framework**: Python, JavaScript, Go, React, Rails, etc.
- **Topic**: style guide, design patterns, performance, security, clean code, etc.
- **Depth**: quick reference vs. deep dive

### Step 2: Search Best Practices (REQUIRED)

**Always start with `--recommend`** to get comprehensive results (resources + deep content):

```bash
python3 skills/best-practices/scripts/search.py "<language> <topic>" --recommend
```

**Examples:**
```bash
python3 skills/best-practices/scripts/search.py "python style guide" --recommend
python3 skills/best-practices/scripts/search.py "javascript clean
```

</details>
