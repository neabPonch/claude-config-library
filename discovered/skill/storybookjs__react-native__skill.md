---
name: storybookjs__react-native__skill
source: https://github.com/storybookjs/react-native/blob/1f966228449dd54041dee54f3e3d83991b56fcbd/skills/setup-react-native-storybook/SKILL.md
repo: storybookjs/react-native
kind: skill
stars: 1295
last_pushed: 2026-06-14T20:54:29Z
license: mit
score: 9
domains: [mobile-development, react-native, testing-tools]
tags: [storybook, react-native, expo, setup-guide]
curated: 2026-06-16
curated_by: config-scout
---

# storybookjs/react-native — skill

**Why it's worth keeping:** Includes explicit filesystem-based logic to determine the correct setup flow and provides precise code snippets for bundler configuration and entrypoint adjustments.

**Summary:** Provides a structured decision tree and implementation steps for adding Storybook to various React Native configurations including Expo, Expo Router, and Re.Pack.

**Source credibility:** High; sourced from the official Storybook React Native repository which is actively maintained.

**Recency:** Very current, covering modern patterns like Expo Router and modern bundlers.

**Source:** [storybookjs/react-native/skills/setup-react-native-storybook/SKILL.md](https://github.com/storybookjs/react-native/blob/1f966228449dd54041dee54f3e3d83991b56fcbd/skills/setup-react-native-storybook/SKILL.md) · 1295★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: setup-react-native-storybook
description: Set up Storybook for React Native in Expo, React Native CLI, or Re.Pack projects. Use when adding Storybook to a project, configuring metro.config.js with withStorybook, creating .rnstorybook configuration files, setting up Storybook routes in Expo Router, configuring getStorybookUI, or adding the StorybookPlugin to a Re.Pack rspack/webpack config. Covers Expo, Expo Router, plain React Native CLI, and Re.Pack setups.
---

# React Native Storybook Setup

Add `@storybook/react-native` v10 to a React Native project.

**Important:** Detect the project's package manager (look for `yarn.lock`, `pnpm-lock.yaml`, or `bun.lockb`) and use it for all install/run commands instead of `npm`. The examples below use `npm` but substitute accordingly (e.g. `yarn add` instead of `npm install`, `yarn storybook` instead of `npm run storybook`). For Expo projects, use `npx expo install` (or `bunx expo install`, etc.) to install dependencies so Expo can resolve compatible versions.

For the init command, use `<pm> create storybook` with the flags shown below. Only npm needs `--` before the flags. Never use `npx`/`bunx` etc for this.

Four setup flows ba
```

</details>
