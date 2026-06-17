---
name: zakirkun__deep-eye
source: https://github.com/zakirkun/deep-eye/blob/0245daba768108cbe448adb0644bdc25799eec61/CLAUDE.md
repo: zakirkun/deep-eye
kind: claude-md
stars: 1756
last_pushed: 2026-05-28T03:45:01Z
license: other
score: 9
domains: [security, cli-tools, ai-agents]
tags: [architecture-driven, extension-patterns, comprehensive-commands]
curated: 2026-06-15
curated_by: config-scout
---

# zakirkun/deep-eye — claude-md

**Why it's worth keeping:** The 'Development Patterns' section is a premier example of how to provide actionable recipes for extending a system without breaking it. The highly specific command list also allows an agent to verify its own work through various test suites.

**Summary:** This file provides high-density context covering execution commands, architectural hierarchy, and core design decisions. It ensures an AI agent can navigate the codebase and understand the 'why' behind the implementation.

**Source credibility:** High; well-starred (1756) and actively maintained repository.

**Recency:** Very current, with updates within the last month.

**Source:** [zakirkun/deep-eye/CLAUDE.md](https://github.com/zakirkun/deep-eye/blob/0245daba768108cbe448adb0644bdc25799eec61/CLAUDE.md) · 1756★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Deep Eye is an AI-driven penetration testing tool. It orchestrates multiple AI providers for payload generation, scans targets for 45+ vulnerability types, and produces professional reports. Python 3.8+, MIT license, v1.4.0 (Code Name: Hanzou).

## Commands

```bash
# Setup
pip install -r requirements.txt
cp config/config.example.yaml config/config.yaml

# Browser automation (optional)
pip install playwright && playwright install chromium

# Run
python deep_eye.py -u https://example.com
python deep_eye.py -c config/config.yaml
python deep_eye.py -u https://example.com -v        # verbose
python deep_eye.py -u https://example.com --no-banner

# CVE database update
python scripts/update_cve_database.py

# Build RAG index for CVE intelligence
python scripts/build_cve_rag_index.py

# Tests
pytest
pytest tests/test_litellm_provider.py -v            # single test file
pytest tests/test_export_formats.py -v              # export formats
pytest tests/test_compliance_mapping.py -v          # compliance
pytest tests/test_scan_diff.py -v                   # scan di
```

</details>
