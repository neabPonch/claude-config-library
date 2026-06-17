---
name: postalsys__emailengine
source: https://github.com/postalsys/emailengine/blob/883b9b487e3580c5b1240d28cd519d190c402b47/CLAUDE.md
repo: postalsys/emailengine
kind: claude-md
stars: 2172
last_pushed: 2026-06-14T14:29:11Z
license: other
score: 9
domains: [backend-api, distributed-systems, nodejs]
tags: [architecture, worker-threads, testing-strategy]
curated: 2026-06-15
curated_by: config-scout
---

# postalsys/emailengine — claude-md

**Why it's worth keeping:** Uses specific file mapping and detailed 'Main Process' orchestration rules that allow an AI to understand the system's lifecycle rather than just its syntax.

**Summary:** Provides a deep architectural blueprint of a complex multi-worker Node.js system, including startup sequences and state management logic. It explicitly differentiates between unit and integration testing tiers to guide troubleshooting.

**Source credibility:** High-quality open source project with significant stars and active maintenance.

**Recency:** Very current, referencing modern Node.js versions (20+) and contemporary patterns.

**Source:** [postalsys/emailengine/CLAUDE.md](https://github.com/postalsys/emailengine/blob/883b9b487e3580c5b1240d28cd519d190c402b47/CLAUDE.md) · 2172★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Development Guidelines

## Project Overview

EmailEngine is an email sync platform that provides REST API access to email accounts. It supports IMAP/SMTP, Gmail API, and Microsoft Graph (Outlook) with real-time webhooks for email events.

## Project Structure

- `server.js` - Main process orchestrator (see Main Process section)
- `/bin` - CLI executable entry point
- `/lib` - Core library modules (account, OAuth, email clients, API routes)
- `/lib/email-client` - Email client implementations (IMAP, Gmail API, Outlook Graph)
- `/lib/api-routes` - REST API route handlers
- `/lib/ui-routes` - Web UI route handlers
- `/lib/lua` - Redis Lua scripts for atomic operations
- `/lib/oauth` - OAuth provider implementations
- `/lib/imapproxy` - IMAP proxy server implementation
- `/workers` - Worker thread modules (8 worker types, see Workers section)
- `/test` - Unit and integration tests
- `/config` - TOML configuration files
- `/views` - Handlebars templates for web UI
- `/static` - Frontend assets (CSS, JS)
- `/translations` - i18n translation files (7 languages)

### Key Files

- `lib/account.js` - Account class, manages IMAP/SMTP interactions
- `lib/account/account-state.js` - Ac
```

</details>
