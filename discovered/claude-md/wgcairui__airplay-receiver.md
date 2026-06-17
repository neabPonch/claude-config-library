---
name: wgcairui__airplay-receiver
source: https://github.com/wgcairui/airplay-receiver/blob/33e047866871a186d3829e57a53438eac4d9343f/CLAUDE.md
repo: wgcairui/airplay-receiver
kind: claude-md
stars: 0
last_pushed: 2025-08-23T08:40:29Z
license: mit
score: 7
domains: [mobile-dev, flutter, android]
tags: [architecture-mapping, technical-specs, build-commands]
curated: 2026-06-17
curated_by: config-scout
---

# wgcairui/airplay-receiver — claude-md

**Why it's worth keeping:** It includes a clear directory hierarchy linking services to core logic and critical technical specifications (resolutions/protocols) that prevent AI hallucination during development.

**Summary:** A highly structured project guide that maps complex service layers and provides specific command-line workflows.

**Source credibility:** 

**Recency:** Current; follows modern Flutter/Android development patterns.

**Source:** [wgcairui/airplay-receiver/CLAUDE.md](https://github.com/wgcairui/airplay-receiver/blob/33e047866871a186d3829e57a53438eac4d9343f/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - PadCast AirPlay Receiver

This file provides guidance to Claude Code (claude.ai/code) when working with the PadCast AirPlay receiver project.

## Commands

### Build
```bash
cd padcast
flutter build apk --release  # Release APK (49.6MB)
flutter build apk --debug    # Debug APK
```

### Test
```bash
cd padcast
flutter test                 # Run Dart unit tests
flutter analyze             # Code analysis (currently clean)
```

### Lint
```bash
cd padcast
flutter analyze             # Static analysis
dart fix --apply            # Auto-fix issues
```

### Development
```bash
cd padcast
flutter run                 # Hot reload development
flutter clean               # Clean build cache
flutter pub get             # Update dependencies
```

## Architecture

### Project Structure
PadCast是一个专为OPPO Pad 4 Pro开发的AirPlay接收器应用，采用Flutter + 原生Android插件架构。

```
padcast/
├── lib/                    # Flutter Dart代码
│   ├── main.dart          # 应用入口
│   ├── controllers/       # MVC控制器层
│   │   └── airplay_controller.dart
│   ├── services/          # 核心服务层
│   │   ├── airplay_service.dart        # 主AirPlay服务
│   │   ├── mdns_service.dart          # mDNS设备发现
│   │   ├── rtsp_service.dart
```

</details>
