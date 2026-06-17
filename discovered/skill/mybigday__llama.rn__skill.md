---
name: mybigday__llama.rn__skill
source: https://github.com/mybigday/llama.rn/blob/4f915f5e5630eaf045c55c65cee16f967eb748d2/.agents/skills/upgrade-react-native/SKILL.md
repo: mybigday/llama.rn
kind: skill
stars: 972
last_pushed: 2026-06-13T10:53:18Z
license: mit
score: 8
domains: [mobile-dev, automation]
tags: [react-native, migration, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# mybigday/llama.rn — skill

**Why it's worth keeping:** Demonstrates a robust migration workflow including remote data retrieval via shell commands and mandatory build-based validation to ensure success.

**Summary:** Automates React Native version upgrades by fetching official diffs from rn-diff-purge and applying them across dependencies, config files, and native code.

**Source credibility:** High; the source repository is a popular React Native binding with significant stars and recent activity.

**Recency:** Current; follows modern agentic patterns of tool verification and automated testing.

**Source:** [mybigday/llama.rn/.agents/skills/upgrade-react-native/SKILL.md](https://github.com/mybigday/llama.rn/blob/4f915f5e5630eaf045c55c65cee16f967eb748d2/.agents/skills/upgrade-react-native/SKILL.md) · 972★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: upgrade-react-native
description: Upgrade React Native version in example/ directory using rn-diff-purge methodology. Use when the user wants to upgrade react-native, migrate to a new RN version, or update React Native dependencies in the example app. Handles diff retrieval, systematic file changes, dependency updates, and conflict resolution.
---

# Upgrade React Native

## CRITICAL: File Editing Rules

- **ALWAYS use Edit/Write tools** to make changes - never just report what should be changed
- **VERIFY changes were saved** by reading the file after editing
- **Actually apply all changes** - do not just list them in a summary

## Workflow

### 1. Detect Current Version

Read `example/package.json` to identify the current react-native version.

### 2. Fetch Upgrade Diff

```bash
curl -s "https://raw.githubusercontent.com/react-native-community/rn-diff-purge/diffs/diffs/{currentVersion}..{toVersion}.diff" | awk '/^GIT binary patch$/,/^diff --git/ {if (/^diff --git/) print; next} 1'
```

For binary files (e.g., gradle-wrapper.jar):
```
https://raw.githubusercontent.com/react-native-community/rn-diff-purge/release/{version}/RnDiffApp/android/gradle/wrapper/gradle-wrapper.j
```

</details>
