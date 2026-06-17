---
name: autonomys-ambassadors__ambassador-os-peer-review
source: https://github.com/autonomys-ambassadors/ambassador-os-peer-review/blob/50aeba4efeabcc85b5d8975ea9a3a607a3433564/claude.md
repo: autonomys-ambassadors/ambassador-os-peer-review
kind: claude-md
stars: 1
last_pushed: 2026-02-27T03:46:26Z
license: unknown
score: 8
domains: [automation, google-apps-script, scripting]
tags: [spreadsheet-automation, environment-management, gas]
curated: 2026-06-15
curated_by: config-scout
---

# autonomys-ambassadors/ambassador-os-peer-review — claude-md

**Why it's worth keeping:** The 'Column Access Pattern' is a brilliant specific instruction that prevents an LLM from writing fragile code by mandating dynamic column lookups instead of hardcoded indices.

**Summary:** Provides detailed instructions for managing multi-environment configurations and fragile spreadsheet-based data access in a Google Apps Script project.

**Source credibility:** Low social proof (1 star), but contains highly technical, domain-specific structural instructions.

**Recency:** Current; includes modern tooling like 'clasp' and specific environment management strategies relevant to today's coding agents.

**Source:** [autonomys-ambassadors/ambassador-os-peer-review/claude.md](https://github.com/autonomys-ambassadors/ambassador-os-peer-review/blob/50aeba4efeabcc85b5d8975ea9a3a607a3433564/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Google Apps Script project that implements the Autonomys Ambassador OS Peer Review system. It manages ambassador submissions, evaluations, and scoring through Google Sheets, Forms, and automated email workflows. The process has 3 major stages:

1. Each month, all active ambassadors are asked to submit evidence via a google form of their work for the prior month. Module1-Submissions.js handles the submission processes.
2. After submissions are recevied (or the deadline passes), 3 ambassadors are randomly selected to evaluate each submission (again via a google form). Module2-Evaluations.js manages the evaluation process.
3. After evaluations are received, a scoring process is run to update the scores and check compliance with the rules. This is managed by Module3-Compliance.js.

## Development Commands

- `clasp push` - Deploy code to Google Apps Script
- `clasp open` - Open the Apps Script editor for debugging
- `clasp pull` - Pull latest code from Google Apps Script
- No traditional build/test commands - this is a Google Apps Script pr
```

</details>
