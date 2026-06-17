---
name: ewwollesen__claude-stuff__claude
source: https://github.com/ewwollesen/claude-stuff/blob/0ec430705f244c29efae31953b91920b16404e2b/ClaudeFiles/Mattermost-Enterprise/CLAUDE.md
repo: ewwollesen/claude-stuff
kind: claude-md
stars: 0
last_pushed: 2026-05-20T16:34:09Z
license: mit
score: 9
domains: [backend, infrastructure, devops]
tags: [architecture-mapping, cross-repo-context, support-investigation]
curated: 2026-06-14
curated_by: config-scout
---

# ewwollesen/claude-stuff — claude-md

**Why it's worth keeping:** It uses highly effective 'interface-to-implementation' mapping and cross-repository dependency descriptions which are crucial for LLM navigation in large systems. It also provides specific pattern recognition (e.g., error prefixing) that speeds up debugging.

**Summary:** An architecturally-dense mapping of an enterprise codebase that links specific implementations back to their required interfaces and parent repositories.

**Source credibility:** Low star count, but the extreme technical specificity suggests high-quality, human-authored domain knowledge.

**Recency:** Highly current; it solves the core problem of multi-repo context awareness for modern AI agents.

**Source:** [ewwollesen/claude-stuff/ClaudeFiles/Mattermost-Enterprise/CLAUDE.md](https://github.com/ewwollesen/claude-stuff/blob/0ec430705f244c29efae31953b91920b16404e2b/ClaudeFiles/Mattermost-Enterprise/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Mattermost Enterprise Codebase Guide (Support Focus)

This guide helps navigate the Mattermost Enterprise repo to answer support questions about enterprise-only features like LDAP, SAML, clustering, compliance, data retention, etc.

> **READ-ONLY REFERENCE COPY**
> This is a read-only reference for code search and support investigations.
> - DO NOT make local code changes, create branches, or commit to this repo
> - Before searching, refresh from remote: `git fetch origin && git pull`
> - Source of truth for this file: `~/Repositories/Claude-Stuff/ClaudeFiles/Mattermost-Enterprise/CLAUDE.md`

## Related Repository

The open-source Mattermost server lives at `../Mattermost`. That repo defines the interfaces this code implements, all config structs, error translation strings, API endpoints, and the store layer. Its `CLAUDE.md` has a full guide to navigating that codebase. When investigating an enterprise feature, you'll often need both repos:

- **Interfaces**: `../Mattermost/server/einterfaces/` defines the contracts
- **Registration hooks**: `../Mattermost/server/channels/app/enterprise.go` and `../Mattermost/server/channels/app/platform/enterprise.go`
- **License model**: `../Ma
```

</details>
