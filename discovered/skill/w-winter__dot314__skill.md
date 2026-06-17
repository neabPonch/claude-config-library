---
name: w-winter__dot314__skill
source: https://github.com/w-winter/dot314/blob/8c184b6fd47c4c6cccc54626f66d009057321283/skills/gdcli/SKILL.md
repo: w-winter/dot314
kind: skill
stars: 112
last_pushed: 2026-05-19T01:48:26Z
license: mit
score: 8
domains: [cli-tools, cloud-api]
tags: [google-drive, search-syntax, oauth]
curated: 2026-06-15
curated_by: config-scout
---

# w-winter/dot314 — skill

**Why it's worth keeping:** The detailed 'Query Syntax' section provides a perfect blueprint for teaching agents how to use tool-specific filtering logic accurately without guessing syntax.

**Summary:** A comprehensive operational guide for gdcli that covers complex OAuth setup and specific command usage.

**Source credibility:** Reputable source with 112 stars and recent updates.

**Recency:** Current; aligns with modern CLI/OAuth workflows used in agentic tasks.

**Source:** [w-winter/dot314/skills/gdcli/SKILL.md](https://github.com/w-winter/dot314/blob/8c184b6fd47c4c6cccc54626f66d009057321283/skills/gdcli/SKILL.md) · 112★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
disable-model-invocation: true
name: gdcli
description: Google Drive CLI for listing, searching, uploading, downloading, and sharing files and folders.
---

# Google Drive CLI

Command-line interface for Google Drive operations.

## Installation

```bash
npm install -g @mariozechner/gdcli
```

## Setup

### Google Cloud Console (one-time)

1. [Create a new project](https://console.cloud.google.com/projectcreate) (or select existing)
2. [Enable the Google Drive API](https://console.cloud.google.com/apis/api/drive.googleapis.com)
3. [Set app name](https://console.cloud.google.com/auth/branding) in OAuth branding
4. [Add test users](https://console.cloud.google.com/auth/audience) (all Gmail addresses you want to use)
5. [Create OAuth client](https://console.cloud.google.com/auth/clients):
   - Click "Create Client"
   - Application type: "Desktop app"
   - Download the JSON file

### Configure gdcli

First check if already configured:
```bash
gdcli accounts list
```

If no accounts, guide the user through setup:
1. Ask if they have a Google Cloud project with Drive API enabled
2. If not, walk them through the Google Cloud Console steps above
3. Have them download the OAuth credent
```

</details>
