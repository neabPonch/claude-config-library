---
name: BasedHardware__omi__skill
source: https://github.com/BasedHardware/omi/blob/f05687ae92f54d0ec124a6801520d43fc3412552/app/e2e/SKILL.md
repo: BasedHardware/omi
kind: skill
stars: 12786
last_pushed: 2026-06-15T02:35:16Z
license: mit
score: 9
domains: [mobile-app, flutter, automation]
tags: [ui-exploration, navigation-map, testing]
curated: 2026-06-15
curated_by: config-scout
---

# BasedHardware/omi — skill

**Why it's worth keeping:** The hierarchical 'Screen Map' provides excellent architectural context, and the command table includes critical warnings about widget tree instability that prevent common agent error loops.

**Summary:** Provides an agent with a structured way to explore and interact with a live Flutter mobile app via a specialized CLI.

**Source credibility:** High-star, active repository (12k+ stars) focused on AI-human interaction.

**Recency:** Current; utilizes modern Flutter/Android debugging protocols.

**Source:** [BasedHardware/omi/app/e2e/SKILL.md](https://github.com/BasedHardware/omi/blob/f05687ae92f54d0ec124a6801520d43fc3412552/app/e2e/SKILL.md) · 12786★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: mobile-app-flows
description: "Understand and explore the Omi Flutter mobile app's UI flows, navigation patterns, and widget architecture. Use when developing features, fixing bugs, or verifying changes in app/lib/ Dart files. Provides agent-flutter commands to explore the live app, understand how screens connect, and verify your work."
allowed-tools: Bash, Read, Glob, Grep
---

# Omi Mobile App — Flows & Exploration

This skill teaches you the Omi Flutter mobile app's navigation structure, screen architecture, and widget patterns. Use it when developing features (to understand how the app works), fixing bugs (to navigate to the affected screen), or verifying changes (to confirm your code works in the live app).

## How to Explore the App

You can interact with the running app via `agent-flutter` — a CLI that taps widgets, reads the widget tree, and captures screenshots through Flutter's Marionette debug protocol.

### Setup
```bash
# 1. Emulator must be running
adb devices                          # should show emulator-5554
# If not: sg kvm -c "$ANDROID_HOME/emulator/emulator -avd omi-dev -no-window -gpu swiftshader_indirect -no-audio -no-boot-anim &"

# 2. Set system l
```

</details>
