---
name: shioneko2026__fanfan-gallery-dl
source: https://github.com/shioneko2026/fanfan-gallery-dl/blob/dae263c58c83a27ae8da12ff508119f31913c8e5/CLAUDE.md
repo: shioneko2026/fanfan-gallery-dl
kind: claude-md
stars: 15
last_pushed: 2026-04-17T17:23:36Z
license: mit
score: 8
domains: [desktop-app, cli-tools, python]
tags: [pyqt6, architectural-constraints, security]
curated: 2026-06-16
curated_by: config-scout
---

# shioneko2026/fanfan-gallery-dl — claude-md

**Why it's worth keeping:** Provides explicit architectural constraints and security rules that prevent LLM errors, such as the instruction to never import the CLI tool as a module.

**Summary:** Defines a PyQt6 desktop application utilizing gallery-dl as a backend subprocess with specific database and security protocols.

**Source credibility:** Small niche project (15 stars) with high-quality documentation structure.

**Recency:** Very recent; updated within the last few months.

**Source:** [shioneko2026/fanfan-gallery-dl/CLAUDE.md](https://github.com/shioneko2026/fanfan-gallery-dl/blob/dae263c58c83a27ae8da12ff508119f31913c8e5/CLAUDE.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FanFan Gallery-DL - Claude Code Context

## Project Overview
A PyQt6 desktop GUI for downloading media from artist subscription platforms (Pixiv Fanbox, Patreon, Fantia, SubscribeStar) using gallery-dl as the backend.

## Tech Stack
- **Frontend**: PyQt6 (desktop GUI)
- **Backend**: gallery-dl (CLI tool in /bin/)
- **Database**: SQLite (data/appdata.db)
- **Language**: Python 3.9+
- **Platform**: Windows (credential storage via Windows Credential Manager)

## Key References
- Original inspiration: https://github.com/KJHJason/Cultured-Downloader
- Backend: https://github.com/mikf/gallery-dl

## Project Structure
- `main.py` - Entry point
- `ui/` - PyQt6 UI modules (main_window, dashboard, downloads, creators, settings)
- `core/` - Business logic (gallery_dl_manager, download_queue, credential_manager)
- `db/` - Database layer (SQLite operations)
- `bin/` - gallery-dl executables
- `config/` - Configuration files
- `data/` - Application data (appdata.db)

## Development Guidelines
1. Follow existing PyQt6 patterns in ui/ modules
2. Use database.py for all database operations
3. Credentials stored in Windows Credential Manager (never in files)
4. Gallery-dl runs as subprocess, never
```

</details>
