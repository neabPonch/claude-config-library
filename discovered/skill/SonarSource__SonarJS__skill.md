---
name: SonarSource__SonarJS__skill
source: https://github.com/SonarSource/SonarJS/blob/4574b48999813fa92063fb7432787b7a6b530963/.claude/skills/ruling/SKILL.md
repo: SonarSource/SonarJS
kind: skill
stars: 1242
last_pushed: 2026-06-14T22:48:19Z
license: other
score: 7
domains: [cli-tools, testing, static-analysis]
tags: [integration-testing, debugging, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# SonarSource/SonarJS — skill

**Why it's worth keeping:** Demonstrates the effective use of 'disable-model-invocation' for long-running tasks and provides high-leverage debugging instructions (environment variables/concurrency control) that an agent can utilize.

**Summary:** Provides a technical manual for running, syncing, and debugging complex integration tests used to verify static analysis rules.

**Source credibility:** Extremely high; SonarSource is a leading industry standard for static code analysis.

**Recency:** Current; the repository shows very recent activity.

**Source:** [SonarSource/SonarJS/.claude/skills/ruling/SKILL.md](https://github.com/SonarSource/SonarJS/blob/4574b48999813fa92063fb7432787b7a6b530963/.claude/skills/ruling/SKILL.md) · 1242★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ruling
description: Run ruling integration tests and update expected results for SonarJS rules. Use when running ruling tests or syncing expected ruling output.
disable-model-invocation: true
---

## Overview

Ruling tests analyze large third-party codebases (JS/TS and CSS) and compare issues against expected output. Run them when adding or modifying rules to verify real-world behavior.

> **Warning:** Running ruling tests removes `node_modules` from the project root. Run `npm ci` afterward.

## Running Ruling

```bash
# Prerequisites: init submodules, install dependencies, build JS/TS, then rebuild the jar
git submodule update --init --recursive
npm install
npm run bbf
mvn install -DskipTests

# Run ruling (JS/TS and CSS)
npm run ruling

# Sync actual → expected (after reviewing output)
npm run ruling-sync

# Debug differences
sh tools/ruling-debug-script.sh
```

Results:

- Actual: `packages/ruling/actual/`
- Expected: `its/ruling/src/test/expected/`

## Java Ruling (Old Way)

```bash
cd its/ruling
mvn verify -Dtest=RulingTest -Dmaven.test.redirectTestOutputToFile=false
```

Copy actual to expected:

```bash
cp -R target/actual/ src/test/expected/
```

Review diff:

```
```

</details>
