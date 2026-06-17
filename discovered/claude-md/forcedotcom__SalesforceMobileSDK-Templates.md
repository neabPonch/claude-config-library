---
name: forcedotcom__SalesforceMobileSDK-Templates
source: https://github.com/forcedotcom/SalesforceMobileSDK-Templates/blob/c1b62a1f72676135a7789a1d95fc5dcc9f6e2001/CLAUDE.md
repo: forcedotcom/SalesforceMobileSDK-Templates
kind: claude-md
stars: 58
last_pushed: 2026-06-12T02:37:08Z
license: bsd-3-clause
score: 8
domains: [mobile-dev, cli-tools, templating]
tags: [ios, android, react-native, sdk, templates]
curated: 2026-06-14
curated_by: config-scout
---

# forcedotcom/SalesforceMobileSDK-Templates — claude-md

**Why it's worth keeping:** Provides specific implementation details for template 'anatomy,' including how dependencies are programmatically managed via custom JS scripts instead of standard package managers alone.

**Summary:** Acts as a technical architectural guide defining the lifecycle and structure of mobile application templates.

**Source credibility:** High; maintained by Salesforce with active recent updates.

**Recency:** Current; includes modern technologies like SwiftUI, Kotlin, and React Native.

**Source:** [forcedotcom/SalesforceMobileSDK-Templates/CLAUDE.md](https://github.com/forcedotcom/SalesforceMobileSDK-Templates/blob/c1b62a1f72676135a7789a1d95fc5dcc9f6e2001/CLAUDE.md) · 58★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Salesforce Mobile SDK Templates

---

## About This Project

The Salesforce Mobile SDK Templates repository is the **template library** for creating Salesforce mobile applications. It contains ready-to-use app templates that serve as starting points for iOS, Android, hybrid (Cordova), and React Native mobile applications.

**Key constraint**: These templates are **consumed by CLI tools** (`forceios`, `forcedroid`, `forcehybrid`, `forcereact`) and the SFDX plugin. Changes here affect every new app created with the Mobile SDK.

## Repository Purpose

This repository provides:

1. **Template Library** - Collection of app templates for all supported platforms and app types
2. **Template Metadata** - `templates.json` defining all available templates
3. **Template Scripts** - `install.js` and `template.js` for dependency management and customization
4. **Testing Infrastructure** - `test_template.sh` for validating template structure and buildability

## Repository Structure

```
SalesforceMobileSDK-Templates/
├── templates.json                         # Template registry (defines all templates)
├── test_template.sh                       # Template testing script
├── TESTING
```

</details>
