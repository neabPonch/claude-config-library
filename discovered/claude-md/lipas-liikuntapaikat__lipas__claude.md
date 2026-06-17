---
name: lipas-liikuntapaikat__lipas__claude
source: https://github.com/lipas-liikuntapaikat/lipas/blob/53ee6cd06b8adb34f825f3d0e464939a4dd7e207/webapp/CLAUDE.md
repo: lipas-liikuntapaikat/lipas
kind: claude-md
stars: 79
last_pushed: 2026-06-13T14:26:19Z
license: mit
score: 9
domains: [backend-api, clojure, cli-tools]
tags: [clojure, repl, token-efficiency]
curated: 2026-06-16
curated_by: config-scout
---

# lipas-liikuntapaikat/lipas — claude-md

**Why it's worth keeping:** The instruction to use `clj-surgeon` for token efficiency is an elite technique for navigating large files. It also provides exact shell command templates for REPL interaction to avoid escaping errors.

**Summary:** Provides highly specific instructions for interacting with a Clojure ecosystem, including nREPL patterns and custom 'surgeon' tools.

**Source credibility:** 79 stars and recent activity indicate a professional, well-maintained codebase.

**Recency:** Very current; incorporates sophisticated agent-specific workflows like custom skill loading and token management.

**Source:** [lipas-liikuntapaikat/lipas/webapp/CLAUDE.md](https://github.com/lipas-liikuntapaikat/lipas/blob/53ee6cd06b8adb34f825f3d0e464939a4dd7e207/webapp/CLAUDE.md) · 79★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# LIPAS Development Guide

## Clojure codebase exploration

Use the `clj-surgeon` skill (auto-loaded from `.claude/skills/clj-surgeon/`) for structural ops on .clj files. ALWAYS run `/clj-surgeon` with `:op :ls` before reading any .clj file over 500 lines or spawning an Explore agent for Clojure code — measured 150x more token-efficient (~1k tokens vs ~150k) and returns in ms vs ~100s. Use `:ls` for form boundaries, then Read only the specific line ranges you need. Only spawn Explore agents for targeted follow-ups with specific file paths.

## REPL Access

nREPL runs on port 7888. Use `clj-nrepl-eval` to evaluate Clojure code:

```bash
# Simple expression
clj-nrepl-eval -p 7888 "(+ 1 2 3)"

# Multiline with heredoc (avoids shell escaping)
clj-nrepl-eval -p 7888 <<'EOF'
(require '[lipas.backend.core :as core] :reload)
(core/get-sports-site db 123456)
EOF
```

Key options: `-t 300000` (custom timeout), `--reset-session` (clear corrupted state)

**Always use `:reload`** when requiring namespaces to pick up changes.

## Common Commands

```clojure
(user/reset)                    ; Reload code and restart system
(user/db)                       ; Get database connection
(user/search)
```

</details>
