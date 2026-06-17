---
name: Snapchat__Valdi__skill
source: https://github.com/Snapchat/Valdi/blob/dac3ece5ae1659338fdd7eb2f1110c1c0f5dc408/ai-skills/skills/valdi-migrate/skill.md
repo: Snapchat/Valdi
kind: skill
stars: 16379
last_pushed: 2026-06-13T00:24:54Z
license: other
score: 9
domains: [mobile-ui, cross-platform-frameworks]
tags: [migration, mapping, negative-constraints, ui-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# Snapchat/Valdi — skill

**Why it's worth keeping:** Uses high-density 'negative constraints' to prevent framework hallucinations and provides structured lookup tables for component/lifecycle equivalence.

**Summary:** A highly specialized migration skill providing strict architectural guardrails and semantic mapping between legacy frameworks (React/Flutter/Compose) and Valdi.

**Source credibility:** High; sourced from a significant official Snapchat repository with active maintenance.

**Recency:** Extremely current, reflecting the latest development status of the source framework.

**Source:** [Snapchat/Valdi/ai-skills/skills/valdi-migrate/skill.md](https://github.com/Snapchat/Valdi/blob/dac3ece5ae1659338fdd7eb2f1110c1c0f5dc408/ai-skills/skills/valdi-migrate/skill.md) · 16379★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Valdi Migration Assistant

Guidance for migrating code from Flutter, React, or Jetpack Compose to Valdi.

## When to use

Use this skill when converting Flutter widgets, React components, or Compose `@Composable` functions to Valdi components, or when translating framework-specific patterns (hooks, widgets, Navigator, setState, remember, LaunchedEffect, Modifier, Provider, styled-components, FlatList, LazyColumn, etc.) to Valdi equivalents.

## Critical: Never suggest these patterns

```typescript
// ❌ React hooks — DO NOT EXIST in Valdi
useState / useEffect / useContext / useMemo / useCallback / useRef

// ❌ Compose APIs — DO NOT EXIST in Valdi
@Composable annotation
remember { mutableStateOf() } / remember { }
derivedStateOf / collectAsState / LaunchedEffect / DisposableEffect
Modifier chain (Modifier.padding().background().clickable())
CompositionLocalProvider / LocalXxx.current

// ❌ Functional components — DO NOT EXIST
const MyComp = () => <view />;
function MyComp(props) { return <view />; }

// ❌ Wrong naming
this.props          // → this.viewModel
onMount/onUnmount   // → onCreate/onDestroy
markNeedsRender()   // → this.setState({})
scheduleRender()    // → deprecated, us
```

</details>
