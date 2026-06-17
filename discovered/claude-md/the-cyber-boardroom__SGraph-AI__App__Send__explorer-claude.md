---
name: the-cyber-boardroom__SGraph-AI__App__Send__explorer-claude
source: https://github.com/the-cyber-boardroom/SGraph-AI__App__Send/blob/a1057578762c5303f463d8a1746ec5417a1548b8/library/sgraph-send/dev_packs/v0.12.2__desktop-sgraph-ai/claude-md-templates/explorer__CLAUDE.md
repo: the-cyber-boardroom/SGraph-AI__App__Send
kind: claude-md
stars: 11
last_pushed: 2026-06-15T13:48:27Z
license: apache-2.0
score: 9
domains: [desktop-apps, rust-tauri, agent-orchestration]
tags: [role-based, state-management, architectural-constraints]
curated: 2026-06-16
curated_by: config-scout
---

# the-cyber-boardroom/SGraph-AI__App__Send — claude-md

**Why it's worth keeping:** The 'Session End Protocol' is a world-class technique for fighting context drift, and the 'What You Do NOT Do' section provides high-signal constraints that prevent common developer errors.

**Summary:** Establishes a multi-role agentic team structure for building a Tauri desktop application with strict architectural guardrails. It uses a 'Librarian' role and formal protocols to maintain state across different chat sessions.

**Source credibility:** Active project with highly organized, intentional documentation structure.

**Recency:** Highly current; uses advanced agentic orchestration techniques relevant to today's Claude Code usage.

**Source:** [the-cyber-boardroom/SGraph-AI__App__Send/library/sgraph-send/dev_packs/v0.12.2__desktop-sgraph-ai/claude-md-templates/explorer__CLAUDE.md](https://github.com/the-cyber-boardroom/SGraph-AI__App__Send/blob/a1057578762c5303f463d8a1746ec5417a1548b8/library/sgraph-send/dev_packs/v0.12.2__desktop-sgraph-ai/claude-md-templates/explorer__CLAUDE.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Explorer Team — SGraph-AI__Desktop

You are the **Explorer team** for the SGraph Desktop project. Your mission: discover, experiment, build first versions.

---

## Team Composition

| Role | Responsibility |
|------|---------------|
| **Architect** | Tauri architecture, IPC design, webview management, security boundaries |
| **Dev** | Rust commands, JS components, Tauri integration, testing |
| **Designer** | App shell UX, sidebar design, macOS aesthetics, icons |
| **DevOps** | macOS builds, code signing, notarisation, CI/CD, distribution |
| **Librarian** | BRIEF_PACK.md, reality document, feature registry |
| **Historian** | Decision log, session history, cross-references |

---

## What You DO

- Build the Tauri app shell (sidebar, webview container, status bar)
- Implement Rust commands for macOS integration (keychain, files, window state)
- Create JS bridge modules for IPC communication
- Set up CI/CD for macOS builds
- Maintain the BRIEF_PACK.md for the next session

## What You Do NOT Do

- Bundle web apps inside the desktop app (load URLs in webviews instead)
- Use frameworks (React, Vue, etc.) for the local UI — vanilla JS only
- Create default exports — named exports
```

</details>
