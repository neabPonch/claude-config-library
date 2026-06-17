---
name: datahub-project__datahub__claude
source: https://github.com/datahub-project/datahub/blob/5c9761ece924e21f3241fbf89cdad70d80a9cffa/datahub-web-react/CLAUDE.md
repo: datahub-project/datahub
kind: claude-md
stars: 12098
last_pushed: 2026-06-16T07:28:30Z
license: apache-2.0
score: 9
domains: [web-frontend, react-typescript]
tags: [architectural-patterns, style-guide, component-hierarchy, cli-commands]
curated: 2026-06-16
curated_by: config-scout
---

# datahub-project/datahub — claude-md

**Why it's worth keeping:** It provides high-signal rules for when to extract hooks or components and distinguishes between 'general' vs 'domain-specific' assets. The command section uses exact CLI/Gradle signatures which is critical for agentic tool-use.

**Summary:** A comprehensive technical handbook covering architectural patterns, component abstraction logic, and specific development commands.

**Source credibility:** High; DataHub is a major, highly-starred open-source project with active maintenance.

**Recency:** Current; reflects modern React/TypeScript standards and recent activity.

**Source:** [datahub-project/datahub/datahub-web-react/CLAUDE.md](https://github.com/datahub-project/datahub/blob/5c9761ece924e21f3241fbf89cdad70d80a9cffa/datahub-web-react/CLAUDE.md) · 12098★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this directory.
It also contains our style guide, which can be consumed by engineers.

## Style Guide

### File Structure

- What should our top-level folders be?
    - `app`: components that implement the entire application
        - Based on nav page
        - Each new high-level page gets a new top-level folder
        - Nested pages are within the same top-level folder
    - `graphql`: graphql files and generated types
    - `images`: all custom images
    - `conf` / `fonts` / `providers` / `utils`: do we need these?
    - When do we create a new one?
- What to put in `index.ts(x)`?
    - Do not create these files
- Where to put tests?
    - In `__tests__/` in the same directory as the file
    - Named `OriginalFile.test.ts(x)`
- Where to put utils?
    - For utils used in a single file: `SourceFile.utils.ts`
    - For utils used in a folder: `folderName/folderName.utils.ts`
- Where to put hooks?
    - For helper hooks used in a single file: `SourceFile.hooks.ts(x)`
    - For standalone, reusable hooks: `hookName.ts(x)`
    - Try not to write hooks that generate JSX, but sometimes
```

</details>
