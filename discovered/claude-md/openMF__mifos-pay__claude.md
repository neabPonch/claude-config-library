---
name: openMF__mifos-pay__claude
source: https://github.com/openMF/mifos-pay/blob/a518db714fe18119d5521cc80b98ec417954193d/fastlane/CLAUDE.md
repo: openMF/mifos-pay
kind: claude-md
stars: 333
last_pushed: 2026-06-13T13:50:20Z
license: mpl-2.0
score: 9
domains: [mobile-dev, devops, automation]
tags: [fastlane, android, ios, deployment]
curated: 2026-06-15
curated_by: config-scout
---

# openMF/mifos-pay — claude-md

**Why it's worth keeping:** It documents known bugs and missing validations (e.g., the Firebase 'groups' parameter bug), preventing AI agents from attempting broken or unreliable workflows.

**Summary:** A highly detailed technical reference for mobile deployment automation using Fastlane across Android and iOS.

**Source credibility:** High-quality, specific documentation for a specialized financial platform repository.

**Recency:** Extremely current/future-dated (Feb 2026).

**Source:** [openMF/mifos-pay/fastlane/CLAUDE.md](https://github.com/openMF/mifos-pay/blob/a518db714fe18119d5521cc80b98ec417954193d/fastlane/CLAUDE.md) · 333★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Fastlane - Deployment Automation

**Last Updated:** 2026-02-13
**Total Lanes:** 12 (7 Android + 5 iOS)
**Configuration:** `fastlane-config/project_config.rb`

[← Back to Main](../CLAUDE.md)

---

## Table of Contents

1. [Overview](#overview)
2. [Android Lanes](#android-lanes)
3. [iOS Lanes](#ios-lanes)
4. [Configuration](#configuration)
5. [Common Tasks](#common-tasks)
6. [Troubleshooting](#troubleshooting)

---

## Overview

Fastlane automates iOS and Android deployment to Firebase, TestFlight, App Store, and Play Store.

**Key Concepts:**
- **Lanes:** Automated deployment workflows
- **Match:** iOS code signing certificate management (uses Git repository)
- **Plugins:** `firebase_app_distribution`, `increment_build_number`
- **Configuration:** Single source of truth in `fastlane-config/project_config.rb`

**Architecture:**
```
GitHub Actions
    ↓
Custom Actions (inflate secrets, call Fastlane)
    ↓
Fastlane Lanes (build, sign, upload)
    ↓
Firebase / Play Store / TestFlight / App Store
```

---

## Android Lanes

### Lane 1: `assembleDebugApks`

**Purpose:** Build debug APKs (no signing)

**Usage:**
```bash
bundle exec fastlane android assembleDebugApks
```

**What it does:
```

</details>
