---
name: software-mansion__react-native-audio-api__skill
source: https://github.com/software-mansion/react-native-audio-api/blob/f29c31b542abd04c9f9388daa94db16316a8707f/.claude/skills/flow/SKILL.md
repo: software-mansion/react-native-audio-api
kind: skill
stars: 787
last_pushed: 2026-06-15T13:17:25Z
license: mit
score: 9
domains: [react-native, mobile-development, high-performance-audio]
tags: [workflow, cross-language, cpp-js-bridge]
curated: 2026-06-16
curated_by: config-scout
---

# software-mansion/react-native-audio-api — skill

**Why it's worth keeping:** It provides precise cross-language orchestration instructions and strict architectural constraints—like avoiding allocations in the audio thread—that prevent common performance pitfalls.

**Summary:** A high-fidelity development workflow for implementing features across TypeScript, JSI (HostObjects), and C++ within a high-performance audio engine.

**Source credibility:** High; maintained by Software Mansion, leaders in React Native infrastructure.

**Recency:** Very current, aligning with modern JSI and TurboModule development patterns.

**Source:** [software-mansion/react-native-audio-api/.claude/skills/flow/SKILL.md](https://github.com/software-mansion/react-native-audio-api/blob/f29c31b542abd04c9f9388daa94db16316a8707f/.claude/skills/flow/SKILL.md) · 787★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: flow
description: >
  End-to-end process for shipping a feature or bug fix in react-native-audio-api. Covers all required deliverables in order: Web Audio API spec review, TypeScript interface and types, C++ AudioNode implementation, HostObject wiring, TypeScript class, TurboModule spec (when needed), C++ tests (Google Test), JS tests (Jest), documentation (audiodocs MDX), and post-work checks. Also covers the bug-fix flow: MRE first, C++ test when applicable, root-cause analysis, post-mortem. Use this skill at the start of any feature implementation or bug fix. Trigger phrases: "implement a feature", "add a node", "fix a bug", "what steps", "where do I start", "PR checklist", "how to write tests".
---

# Skill: Feature Implementation Flow

## Quick Reference

**Feature checklist (all 9 steps required for a PR):**
1. Read spec → define exactly what you're building
2. TypeScript interface + option types (`src/interfaces/`, `src/types/`)
3. C++ AudioNode (`core/<category>/MyNode.h/.cpp`) — see `audio-nodes` skill
4. HostObject (`HostObjects/MyNodeHostObject.h/.cpp`) — see `host-objects` skill
5. TypeScript class (`src/core/MyNode.ts`)
6. TurboModule spec entry — **only** if
```

</details>
