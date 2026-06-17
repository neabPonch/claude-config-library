---
name: mikkelkrogsholm__api-mapper
source: https://github.com/mikkelkrogsholm/api-mapper/blob/33a7d29e93ccf6e1454cf28daa740b97ee16241f/CLAUDE.md
repo: mikkelkrogsholm/api-mapper
kind: claude-md
stars: 200
last_pushed: 2025-07-04T16:28:06Z
license: mit
score: 9
domains: [chrome-extension, web-development, api-tools]
tags: [manifest-v3, architecture, data-flow, browser-extension]
curated: 2026-06-15
curated_by: config-scout
---

# mikkelkrogsholm/api-mapper — claude-md

**Why it's worth keeping:** It includes highly actionable 'Technical Constraints' (like serialization rules) and a 'Data Flow' section that prevents the AI from hallucinating incorrect communication patterns.

**Summary:** Provides a deep architectural breakdown of a Chrome Extension, focusing on how different scripts interact and the specific limitations of Manifest V3.

**Source credibility:** 200 stars indicates a validated, useful tool; maintenance status is slightly aged but technical context remains relevant.

**Recency:** Highly current as it specifically addresses modern Manifest V3 constraints which are essential for today's browser development.

**Source:** [mikkelkrogsholm/api-mapper/CLAUDE.md](https://github.com/mikkelkrogsholm/api-mapper/blob/33a7d29e93ccf6e1454cf28daa740b97ee16241f/CLAUDE.md) · 200★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

API Mapper is a Chrome Extension that captures and documents API calls from websites. It adds a panel to Chrome DevTools that monitors network requests and exports them as OpenAPI 3.0 specifications.

## Architecture

### Core Components

1. **Background Script (`background.js`)**
   - Uses Chrome's webRequest API to intercept XHR and Fetch requests
   - Maintains a Map of API endpoints with their captured data
   - Implements memory management to limit stored data
   - Communicates with DevTools panel via Chrome runtime messaging
   - Critical: Must include `chrome.runtime.sendMessage()` to send updates to panel

2. **DevTools Panel (`panel.js`)**
   - Main UI logic displaying captured API calls
   - Implements filtering by host, method, and search text
   - Generates OpenAPI 3.0 specifications from captured data
   - Uses port-based messaging for initial connection and runtime messaging for updates
   - Creates cURL commands with optional complete header capture

3. **Security & Configuration (`config.js`)**
   - Contains SecurityUtils object f
```

</details>
