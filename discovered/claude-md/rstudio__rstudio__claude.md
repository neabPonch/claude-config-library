---
name: rstudio__rstudio__claude
source: https://github.com/rstudio/rstudio/blob/78ff96838f6ad668b841d7d221af40b16a1eaa57/.claude/CLAUDE.md
repo: rstudio/rstudio
kind: claude-md
stars: 5014
last_pushed: 2026-06-15T03:08:32Z
license: other
score: 9
domains: [backend-api, web-frontend, desktop-integration]
tags: [architectural-overview, workflow-checklists, rpc-communication]
curated: 2026-06-15
curated_by: config-scout
---

# rstudio/rstudio — claude-md

**Why it's worth keeping:** The 'Adding a New Feature' checklist and the explicit step-by-step explanation of the RPC/Event communication flow are highly actionable for an agent.

**Summary:** Provides deep architectural mapping of a complex multi-component system involving C++, GWT, and Electron.

**Source credibility:** High; based on the RStudio repository which is a major, well-maintained industry standard.

**Recency:** Extremely current, with activity reported within the last month.

**Source:** [rstudio/rstudio/.claude/CLAUDE.md](https://github.com/rstudio/rstudio/blob/78ff96838f6ad668b841d7d221af40b16a1eaa57/.claude/CLAUDE.md) · 5014★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# RStudio

These instructions apply to the RStudio open-source IDE repository.


## Code Structure

Broadly speaking, RStudio is split into three different components -- the front-end / user interface, the desktop integration, and the backend / server components.

- The user interface uses a mixture of Google GWT and JavaScript, in `src/gwt`.
- The desktop integration lives in `src/node/desktop`, as an Electron application.
- The backend and server components live in `src/cpp`, and are primarily authored in C++ and R.


### Backend Layout (`src/cpp`)

    src/cpp/
    ├── core/              # Foundation libraries (http, json, system, text, etc.)
    ├── shared_core/       # Shared between server and session
    ├── server_core/       # Server-specific core utilities
    ├── r/                 # R integration layer
    │   └── R/             # Core R functions (Api.R, Tools.R, etc.)
    ├── session/           # Session management (main IDE backend)
    │   ├── modules/       # Feature modules (one per feature)
    │   ├── include/       # Public headers
    │   └── resources/     # Schemas, templates, static resources
    ├── server/            # RStudio Server (auth, db, launcher)
```

</details>
