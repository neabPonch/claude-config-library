---
name: chohra-med__expo_boilerplate__claude-skill
source: https://github.com/chohra-med/expo_boilerplate/blob/9ea04cd5bc715d7010e7098298a4e829105277c1/CLAUDE_SKILL.md
repo: chohra-med/expo_boilerplate
kind: skill
stars: 25
last_pushed: 2026-04-23T08:52:23Z
license: mit
score: 9
domains: [mobile-development, react-native, ai-agents]
tags: [expo, redux-toolkit, scaffolding, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# chohra-med/expo_boilerplate — skill

**Why it's worth keeping:** The 'command + checklist' pattern is elite; it ensures that after code generation, the user is prompted for required manual registrations like adding reducers to the store. The use of specific architectural constraints (e.g., forcing Restyle over StyleSheet) makes the skill highly predictable and professional.

**Summary:** Provides a command-driven DSL (`/mobilelauncher`) for high-speed, architecturally-compliant scaffolding in an Expo/React Native project. It automates feature creation while enforcing strict rules on styling, state management, and type safety.

**Source credibility:** High-quality specialized boilerplate with recent activity.

**Recency:** Extremely current, updated within the last 2 months.

**Source:** [chohra-med/expo_boilerplate/CLAUDE_SKILL.md](https://github.com/chohra-med/expo_boilerplate/blob/9ea04cd5bc715d7010e7098298a4e829105277c1/CLAUDE_SKILL.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE_SKILL.md — MobileLauncher LT

This project ships with a Claude Code skill that generates boilerplate-consistent code for this repo.

The skill file lives at: `.claude/skills/mobilelauncher/skill.md`

---

## How to use

From inside this project, run:

```
/mobilelauncher <command>
```

---

## Commands

| Command | What it does |
|---|---|
| `/mobilelauncher orient` | Read the project and output a concise orientation: versions, features, reducers, rules summary |
| `/mobilelauncher feature <name>` | Scaffold a complete new feature with all files (types, slice, selectors, RTK Query endpoints, hooks, screens, barrel exports) |
| `/mobilelauncher screen <feature> <name>` | Add a new screen to an existing feature, typed and wired for navigation |
| `/mobilelauncher component <name>` | Generate a shared Restyle UI component in `src/ui/components/` |
| `/mobilelauncher hook <name>` | Generate a custom hook (feature-scoped or shared) |
| `/mobilelauncher slice <feature>` | Generate a Redux slice + createSelector selectors for an existing feature |
| `/mobilelauncher endpoint <feature> <name>` | Generate an RTK Query endpoint injection for an existing feature |
| `/mobilelauncher
```

</details>
