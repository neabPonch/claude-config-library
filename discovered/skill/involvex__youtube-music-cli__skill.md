---
name: involvex__youtube-music-cli__skill
source: https://github.com/involvex/youtube-music-cli/blob/35314a328ace7ae9c4b5370dabe829efde3d4e88/.agents/skills/node-to-bun/SKILL.md
repo: involvex/youtube-music-cli
kind: skill
stars: 330
last_pushed: 2026-06-06T16:30:38Z
license: mit
score: 9
domains: [devops, runtime-migration, cli-tools]
tags: [bun, nodejs, migration, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# involvex/youtube-music-cli — skill

**Why it's worth keeping:** The use of a specific reporting template (BUN_MIGRATION_REPORT.md) and hardcoded lists of problematic dependencies provides high-density intelligence for an agent.

**Summary:** A highly structured workflow for migrating Node.js projects to the Bun runtime, covering dependencies, configurations, and testing.

**Source credibility:** High quality; contains detailed technical nuances like tsconfig changes and workspace considerations common in professional migrations.

**Recency:** Very current, targeting Bun 1.0+ and modern TypeScript module resolution standards.

**Source:** [involvex/youtube-music-cli/.agents/skills/node-to-bun/SKILL.md](https://github.com/involvex/youtube-music-cli/blob/35314a328ace7ae9c4b5370dabe829efde3d4e88/.agents/skills/node-to-bun/SKILL.md) · 330★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: node-to-bun
description: Migrate Node.js projects to Bun with compatibility analysis. Use when converting existing npm/pnpm/yarn projects to Bun or auditing dependencies for Bun compatibility.
compatibility: Requires Bun 1.0+
allowed-tools: ["Bash", "Read", "Grep", "Write"]
metadata:
  author: daleseo
  category: bun-runtime
  tags: [bun, migration, nodejs, node-to-bun, compatibility, dependencies]
---

# Node.js to Bun Migration

You are assisting with migrating an existing Node.js project to Bun. This involves analyzing dependencies, updating configurations, and ensuring compatibility.

## Migration Workflow

### 1. Pre-Migration Analysis

**Check if Bun is installed:**
```bash
bun --version
```

**Analyze current project:**
```bash
# Check Node.js version
node --version

# Check package manager
ls -la | grep -E "package-lock.json|yarn.lock|pnpm-lock.yaml"
```

Read `package.json` to understand the project structure.

### 2. Dependency Compatibility Check

**Read and analyze all dependencies** from `package.json`:

```bash
cat package.json
```

**Check for known incompatible native modules:**

Common problematic packages (check against current dependencies):

- `bcrypt`
```

</details>
