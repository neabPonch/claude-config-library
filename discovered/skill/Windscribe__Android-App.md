---
name: Windscribe__Android-App
source: https://github.com/Windscribe/Android-App/blob/5b34e62cca562eb745c107f03f65bcfdbd9ec9b7/SKILL.md
repo: Windscribe/Android-App
kind: skill
stars: 318
last_pushed: 2026-05-31T20:11:31Z
license: gpl-2.0
score: 9
domains: [mobile-android, mobile-development]
tags: [android, jetpack-compose, hilt, workflow]
curated: 2026-06-14
curated_by: config-scout
---

# Windscribe/Android-App — skill

**Why it's worth keeping:** It avoids single-file instructions in favor of 'Step 1 to Step N' sequences that detail how changes must propagate across routes, navigation graphs, and dependency injection layers to maintain architectural integrity.

**Summary:** A highly structured technical playbook that guides an AI agent through multi-file development workflows within a production Android codebase.

**Source credibility:** Extremely high; it is derived from the official source of a large-scale, production-grade Android application.

**Recency:** 

**Source:** [Windscribe/Android-App/SKILL.md](https://github.com/Windscribe/Android-App/blob/5b34e62cca562eb745c107f03f65bcfdbd9ec9b7/SKILL.md) · 318★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Windscribe Android App — AI Agent Skill

You are an AI agent working with the Windscribe Android app codebase. This skill defines HOW to perform common development, debugging, and maintenance tasks.

For architecture reference (WHAT the system is), see [AGENTS.md](AGENTS.md).
For human-friendly overview, see [README.md](README.md).

---

## Prerequisites

Before starting any work session:

```bash
# 1. Verify Android environment
echo $ANDROID_HOME
./gradlew --version

# 2. Pull latest changes (avoid conflicts)
git pull --rebase

# 3. Check current branch
git branch --show-current

# 4. Clean build if switching branches or after schema changes
./gradlew clean
```

---

## Development Workflows

### Adding a New Screen (Mobile — Jetpack Compose)

**Step 1: Define Screen Route**

```kotlin
// mobile/src/main/java/com/windscribe/mobile/nav/Screen.kt
sealed class Screen(val route: String) {
    // Existing screens...
    object NewFeature: Screen("new_feature")
}
```

**Step 2: Add to Navigation Graph**

```kotlin
// mobile/src/main/java/com/windscribe/mobile/nav/NavigationStack.kt
private fun NavGraphBuilder.addNavigationScreens() {
    // Existing routes...

    composable(
```

</details>
