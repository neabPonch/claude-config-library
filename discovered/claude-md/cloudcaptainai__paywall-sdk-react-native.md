---
name: cloudcaptainai__paywall-sdk-react-native
source: https://github.com/cloudcaptainai/paywall-sdk-react-native/blob/00d45015e72039de288852c49bf0af470612b63b/CLAUDE.md
repo: cloudcaptainai/paywall-sdk-react-native
kind: claude-md
stars: 1
last_pushed: 2026-06-16T05:09:12Z
license: mit
score: 8
domains: [mobile-development, react-native]
tags: [bridge, cross-platform, sdk, safety-constraints]
curated: 2026-06-16
curated_by: config-scout
---

# cloudcaptainai/paywall-sdk-react-native — claude-md

**Why it's worth keeping:** The 'Key architecture rule' maps specific files to the native synchronization process, preventing breaking changes. The 'Key principles' section includes domain-specific semantic rules that prevent jargon confusion.

**Summary:** Provides critical architectural constraints for maintaining a high-stakes React Native bridge across JS, iOS, and Android.

**Source credibility:** Likely a professional engineering team given the SDK complexity and high-quality documentation.

**Recency:** Very current; aligns with modern Expo/React Native development workflows.

**Source:** [cloudcaptainai/paywall-sdk-react-native/CLAUDE.md](https://github.com/cloudcaptainai/paywall-sdk-react-native/blob/00d45015e72039de288852c49bf0af470612b63b/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project overview

React Native SDK for Helium paywalls. Supports bare React Native and Expo 49–51 (Expo 52+ is handled by the separate Expo-modules SDK). Bridges native iOS (Swift, via ObjC `RCT_EXTERN_METHOD` shim) and Android (Kotlin, via `@ReactMethod`) to TypeScript.

## Key principles

- **Never crash the host app.** This SDK is distributed to apps with millions of users. Wrap bridge boundaries and event handlers in try/catch to prevent SDK errors from propagating. For critical flows consider logging and/or surfacing failures to callers rather than silently swallowing them.
- **Avoid using "fallback" in code and comments** unless referring to the Helium fallback paywall flow. This term has a specific meaning in this SDK.

## Key architecture rule

**When modifying the native bridge interface, both iOS and Android native modules MUST be updated** so their signatures stay in sync with the JS call site.

Relevant files for bridge changes:
- `src/index.ts` — public API re-exports
- `src/native-interface.tsx` — JS bridge calls (`NativeModules.HeliumBridge`, `NativeEventEmitter`)
- `src/types.ts`, `src/HeliumExperimentInfo.types.ts` — TypeScript types
- `ios/RCTHeliu
```

</details>
