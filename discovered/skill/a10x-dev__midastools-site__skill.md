---
name: a10x-dev__midastools-site__skill
source: https://github.com/a10x-dev/midastools-site/blob/5493d2975852c4dc4e82bc28f9e7a72f10b57db6/.skill.md
repo: a10x-dev/midastools-site
kind: skill
stars: 0
last_pushed: 2026-06-16T04:25:21Z
license: unknown
score: 7
domains: [agents-ai, cli-tools, automation]
tags: [browser-automation, google-workspace, firecrawl, command-line]
curated: 2026-06-16
curated_by: config-scout
---

# a10x-dev/midastools-site — skill

**Why it's worth keeping:** The inclusion of explicit 'Usage Examples' for complex CLI commands is an excellent pattern for teaching agents how to interact with custom tools; the addition of rate limits also helps guide autonomous planning.

**Summary:** A service manifest defining capabilities for a co-founder agent, covering browser automation, Google Workspace CLI, and web research.

**Source credibility:** Low credibility due to 0 stars and a single-purpose repository structure.

**Recency:** Current, utilizing modern automation patterns like Firecrawl and Playwright.

**Source:** [a10x-dev/midastools-site/.skill.md](https://github.com/a10x-dev/midastools-site/blob/5493d2975852c4dc4e82bc28f9e7a72f10b57db6/.skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: co-founder-services
description: Connected services available to the Co-Founder autonomous agent
version: 1.0.0
---

# Connected Services

These are the real-world tools available to this agent.

## Browser (Playwright)

- **Type**: mcp
- **Command**: `npx`
- **Description**: Browse the web, post to social media, fill forms, extract data — uses persistent login sessions
- **Capabilities**: browser.navigate, browser.click, browser.type, browser.screenshot, browser.tab_management
- **Rate limit**: 200/hour, 2000/day

## Google Workspace

- **Type**: cli
- **Command**: `gws`
- **Description**: Gmail, Calendar, Drive, Sheets, Docs — full Google Workspace access via CLI
- **Capabilities**: email.send, email.read, calendar.create, calendar.list, drive.list, drive.upload, sheets.read, sheets.write, docs.create
- **Rate limit**: 60/hour, 500/day

### Usage Examples

```bash
# Send an email
gws gmail send --to user@example.com --subject "Subject" --body "Body"

# List recent emails
gws gmail list --max-results 10

# Create a calendar event
gws calendar create --summary "Meeting" --start "2026-03-30T10:00:00" --end "2026-03-30T11:00:00"

# List files in Drive
gws drive list --max-r
```

</details>
