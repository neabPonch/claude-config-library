---
name: naraesk__krunner-translator
source: https://github.com/naraesk/krunner-translator/blob/afe1978108dbb1ea2c05c08d33832a045ffd41d6/CLAUDE.md
repo: naraesk/krunner-translator
kind: claude-md
stars: 110
last_pushed: 2026-05-10T09:46:37Z
license: gpl-3.0
score: 9
domains: [desktop-integration, c++, qt]
tags: [kde, plasma-6, kf6, cmake]
curated: 2026-06-15
curated_by: config-scout
---

# naraesk/krunner-translator — claude-md

**Why it's worth keeping:** The 'KF6/Qt6 Conventions' section is exceptional; it preemptively solves common pitfalls regarding macros, string handling, and JSON metadata requirements specific to the framework.

**Summary:** Provides a comprehensive project map and deep architectural detail for a KDE Plasma 6 plugin.

**Source credibility:** High-quality specialized project with decent social proof (110 stars) and modern maintenance.

**Recency:** Very current, targeting latest Plasma 6/KF6 standards.

**Source:** [naraesk/krunner-translator/CLAUDE.md](https://github.com/naraesk/krunner-translator/blob/afe1978108dbb1ea2c05c08d33832a045ffd41d6/CLAUDE.md) · 110★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# KRunner Translator Plugin

## Project Overview
A KRunner plugin for KDE Plasma 6 that translates text using multiple translation engines. Users type a language code (or source-target pair) followed by text in KRunner to get translations.

**Query syntax:** `<lang> text` or `<source>-<target> text` (e.g., `de hello` or `en-fr hello`)

## Build System
- **Framework:** KDE Frameworks 6 (KF6), Qt 6, ECM 6.0+
- **Build:** `mkdir build && cd build && cmake .. && make`
- **Test:** `cd build && ctest` or run `./bin/translator_test`
- **Install:** `cd build && sudo make install`
- Plugins install to `kf6/krunner/` and `kf6/krunner/kcms/` namespaces via `kcoreaddons_add_plugin`

## Architecture

### Three build targets
1. **krunner_translator** - the main runner plugin (.so)
2. **kcm_krunner_translator** - KCM config module for runner settings
3. **translator_test** - test executable

### Translation engines
- **GoogleTranslate** and **Bing** - command-line engines using `trans` (translate-shell) via `TranslateShellProcess`
- **Baidu** and **Youdao** - network API engines using `QNetworkAccessManager` with async HTTP requests
- All engines implement `CommandLineEngine` interface (despite t
```

</details>
