---
name: deviceplug__btleplug
source: https://github.com/deviceplug/btleplug/blob/ee381ac34fd8600cc0faae1b8e71470db84135cf/CLAUDE.md
repo: deviceplug/btleplug
kind: claude-md
stars: 1136
last_pushed: 2026-05-25T05:36:21Z
license: other
score: 8
domains: [systems-programming, rust, cross-platform]
tags: [rust, hardware-abstraction, architecture-rules]
curated: 2026-06-14
curated_by: config-scout
---

# deviceplug/btleplug — claude-md

**Why it's worth keeping:** The 'Boundaries' section is highly effective at preventing illegal imports in conditionally compiled modules; the distinction between unit and hardware-dependent integration tests is crucial.

**Summary:** Provides technical stack details and essential architectural constraints for a complex cross-platform Rust library.

**Source credibility:** High credibility with 1k+ stars and recent activity.

**Recency:** Extremely current, referencing modern Rust edition 2024 standards.

**Source:** [deviceplug/btleplug/CLAUDE.md](https://github.com/deviceplug/btleplug/blob/ee381ac34fd8600cc0faae1b8e71470db84135cf/CLAUDE.md) · 1136★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# btleplug

Last verified: 2026-03-08

## Tech Stack

- Language: Rust (edition 2024)
- Platforms: Windows (WinRT), macOS/iOS (CoreBluetooth), Linux (BlueZ), Android (JNI)
- Async runtime: Tokio
- Testing: `cargo test`, integration tests require BLE hardware/virtual peripheral

## Commands

- `cargo build` -- Build for host platform
- `cargo test` -- Run unit tests
- `cargo test --test '*' -- --ignored` -- Run integration tests (requires test peripheral)
- `scripts/run-jni-tests.sh` -- Compile Java sources and run JNI host tests on host JVM
- `scripts/run-integration-tests.sh` -- Run BLE integration tests (requires test peripheral)
- `scripts/run-integration-tests-android.sh` -- Run Android integration tests
- `scripts/build-java.sh` -- Build Java/Android components

## Project Structure

- `src/api/` -- Public BLE API traits (Manager, Central, Peripheral)
- `src/bluez/` -- Linux BlueZ backend
- `src/corebluetooth/` -- macOS/iOS CoreBluetooth backend
- `src/droidplug/` -- Android JNI backend
- `src/winrtble/` -- Windows WinRT backend
- `src/common/` -- Shared utilities (non-Linux platforms)
- `src/platform/` -- Platform-specific type exports
- `tests/` -- Integration test suite (se
```

</details>
