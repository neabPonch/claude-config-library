---
name: mk-knight23__AGENTS-COLLECTION__gws-skill
source: https://github.com/mk-knight23/AGENTS-COLLECTION/blob/41d09336e6aa7f881389b585edfb34768b0a8ca3/DOCS/NANOBOT/gws-SKILL.md
repo: mk-knight23/AGENTS-COLLECTION
kind: skill
stars: 72
last_pushed: 2026-04-16T07:24:00Z
license: unknown
score: 9
domains: [cli-tools, automation, productivity]
tags: [gws, google-workspace, shell-commands]
curated: 2026-06-15
curated_by: config-scout
---

# mk-knight23/AGENTS-COLLECTION — skill

**Why it's worth keeping:** Includes specific shell-piping patterns (e.g., using jq for Gmail raw data) and precise flag structures for complex operations like spreadsheet range updates and calendar recurrences.

**Summary:** Provides a highly detailed command reference for interacting with Google Workspace services via the gws CLI.

**Source credibility:** Part of a high-density, multi-platform agent collection with active maintenance.

**Recency:** Current; provides highly relevant CLI patterns for modern agent workflows.

**Source:** [mk-knight23/AGENTS-COLLECTION/DOCS/NANOBOT/gws-SKILL.md](https://github.com/mk-knight23/AGENTS-COLLECTION/blob/41d09336e6aa7f881389b585edfb34768b0a8ca3/DOCS/NANOBOT/gws-SKILL.md) · 72★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: gws
description: Google Workspace CLI for managing Gmail, Sheets, Calendar, and Drive from the command line.
homepage: https://github.com/googleapis/google-workspace-cli
metadata: {"nanobot":{"emoji":"📧","requires":{"bins":["gws"]}}}
---

# Google Workspace CLI (gws)

**Powerful command-line interface for Google Workspace services**

---

## 🚀 Overview

The `gws` CLI provides a unified interface to interact with Google Workspace services directly from your terminal:
- 📧 **Gmail** - Manage emails, labels, filters
- 📊 **Sheets** - Read/write spreadsheets, data manipulation
- 📅 **Calendar** - Events, scheduling, reminders
- 📁 **Drive** - File operations, sharing, permissions

Perfect for automation scripts, batch operations, and integration with nanobot workflows.

---

## 📦 Installation

### Prerequisites
```bash
# Python 3.8+ required
python3 --version

# Install via pip
pip3 install google-workspace-cli

# Or install from source
git clone https://github.com/googleapis/google-workspace-cli.git
cd google-workspace-cli
pip3 install -e .
```

### Quick Setup
```bash
# Initialize gws (interactive wizard)
gws init

# Verify installation
gws --version
gws --help
```

---

## 🔐 O
```

</details>
