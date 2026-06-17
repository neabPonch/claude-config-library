---
name: TelegramMessenger__Telegram-iOS__claude
source: https://github.com/TelegramMessenger/Telegram-iOS/blob/6e370e06d147b091b07903071cb1b8a22152492d/submodules/TgVoipWebrtc/CLAUDE.md
repo: TelegramMessenger/Telegram-iOS
kind: claude-md
stars: 8609
last_pushed: 2026-06-09T14:27:05Z
license: unknown
score: 9
domains: [networking, c++, voice-over-ip, cross-platform]
tags: [bazel, webrtc, sctp, macOS, Linux]
curated: 2026-06-15
curated_by: config-scout
---

# TelegramMessenger/Telegram-iOS — claude-md

**Why it's worth keeping:** It documents complex architectural 'gotchas' (like the custom SCTP timer tuning) that prevent an AI from accidentally undoing critical bug fixes. It also provides specific, high-value test commands for verifying complex interoperability scenarios.

**Summary:** Provides platform-specific build instructions for macOS/Linux and deep technical documentation of critical SCTP signaling logic and cross-version compatibility architecture.

**Source credibility:** High; comes from the Telegram-iOS repository which is a major, highly-active open-source project.

**Recency:** Current; includes recent updates regarding macOS arm64 support and modern toolchain compatibility.

**Source:** [TelegramMessenger/Telegram-iOS/submodules/TgVoipWebrtc/CLAUDE.md](https://github.com/TelegramMessenger/Telegram-iOS/blob/6e370e06d147b091b07903071cb1b8a22152492d/submodules/TgVoipWebrtc/CLAUDE.md) · 8609★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# tgcalls Library

The tgcalls VoIP library source. See the root `CLAUDE.md` for build instructions and the project overview.

## macOS Build Support

This repo has been patched to support native macOS arm64 builds (`darwin_arm64` CPU) in addition to the original iOS targets. Changes made:
- `third-party/webrtc/BUILD` — added `@platforms//os:linux` to `arch_specific_cflags` select (fixes macOS getting Linux flags via `//conditions:default`); moved `cocoa_threading.mm` from `cc_library` to `webrtc_platform_helpers` `objc_library` (Bazel 8 rejects `.mm` in `cc_library`); replaced UIKit with AppKit for macOS
- `third-party/openh264/BUILD` — added `//conditions:default` to `select()` statements
- `third-party/webrtc/absl/absl/base/attributes.h` — disabled `ABSL_ATTRIBUTE_LIFETIME_BOUND` (newer Xcode clang rejects it on void-returning functions)
- 8 third-party BUILD files + 8 build shell scripts — added `darwin_arm64 -> macos_arm64` architecture support (opus, libvpx, ffmpeg, dav1d, mozjpeg, webp, libjxl, td)

## Linux Build Support

The repo supports native Linux arm64 and x86_64 builds. Key changes from the iOS/macOS-only baseline:
- `.bazelrc` — Apple toolchain settings under `build
```

</details>
