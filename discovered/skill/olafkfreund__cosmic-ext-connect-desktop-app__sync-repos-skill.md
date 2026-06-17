---
name: olafkfreund__cosmic-ext-connect-desktop-app__sync-repos-skill
source: https://github.com/olafkfreund/cosmic-ext-connect-desktop-app/blob/71b8c2ac8f5c003b8cfbeec0f19ad373856c7af6/tools/sync-repos-skill.md
repo: olafkfreund/cosmic-ext-connect-desktop-app
kind: skill
stars: 9
last_pushed: 2026-06-05T15:20:39Z
license: other
score: 9
domains: [multi-repo, cross-language, system-design]
tags: [sync, rust, kotlin, protocol]
curated: 2026-06-16
curated_by: config-scout
---

# olafkfreund/cosmic-ext-connect-desktop-app — skill

**Why it's worth keeping:** It provides highly transferable language-specific translation patterns (e.g., Rust Enums to Kotlin Sealed Classes) and a structured, high-safety multi-phase execution loop.

**Summary:** An interactive multi-repo synchronization workflow that detects protocol changes in one repository and generates corresponding code for others.

**Source credibility:** Low star count suggests a niche tool, but the technical depth of the logic is high.

**Recency:** Current; demonstrates advanced agentic patterns like human-in-the-loop review and dependency analysis.

**Source:** [olafkfreund/cosmic-ext-connect-desktop-app/tools/sync-repos-skill.md](https://github.com/olafkfreund/cosmic-ext-connect-desktop-app/blob/71b8c2ac8f5c003b8cfbeec0f19ad373856c7af6/tools/sync-repos-skill.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Sync Repos Skill - Interactive Multi-Repository Sync with Claude

## Overview

This skill enables Claude to assist with syncing changes between:
- `cosmic-connect-desktop-app` (Rust - source)
- `cosmic-ext-connect-core` (Rust - shared library)
- `cosmic-connect-android` (Kotlin - mobile client)

**Key Features:**
- Claude analyzes changes and identifies what needs syncing
- Interactive review and confirmation for each change
- Claude generates appropriate code for Rust and Kotlin
- Preserves language-specific idioms and patterns
- Verifies compatibility and suggests improvements

## Usage

```
/sync-repos [--since COMMIT]
```

## Workflow

### 1. Analysis Phase (Automated)
Claude will:
- Analyze recent commits in desktop-app
- Identify changes that affect protocol, errors, constants
- Check for breaking changes
- Categorize by target repository (core vs android)

### 2. Review Phase (Interactive)
Claude will present findings and ask:
- "I found protocol version change - shall I sync to both core and android?"
- "New packet type detected - update android only?"
- "Error type modified - how should we translate to Kotlin?"

### 3. Generation Phase (AI-Assisted)
For each approved cha
```

</details>
