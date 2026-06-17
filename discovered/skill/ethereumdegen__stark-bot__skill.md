---
name: ethereumdegen__stark-bot__skill
source: https://github.com/ethereumdegen/stark-bot/blob/93bf92205485efe508f3ab5b92317488ca3116ff/modules/supabase_cli/skill.md
repo: ethereumdegen/stark-bot
kind: skill
stars: 48
last_pushed: 2026-03-30T18:21:44Z
license: mit
score: 9
domains: [devops, database, cli-tools, infrastructure]
tags: [supabase, backend, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# ethereumdegen/stark-bot — skill

**Why it's worth keeping:** Uses advanced agentic patterns like `define_tasks` for progress tracking and explicitly mandates human confirmation for destructive actions.

**Summary:** A highly structured skill file that automates Supabase CLI management through multi-step workflows and safety protocols.

**Source credibility:** High quality; follows professional documentation standards despite being from a smaller repository.

**Recency:** Very current, utilizing modern Claude Code task-definition capabilities.

**Source:** [ethereumdegen/stark-bot/modules/supabase_cli/skill.md](https://github.com/ethereumdegen/stark-bot/blob/93bf92205485efe508f3ab5b92317488ca3116ff/modules/supabase_cli/skill.md) · 48★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: supabase
description: "Manage Supabase projects - databases, migrations, edge functions, storage, and secrets using the Supabase CLI."
version: 1.0.0
author: starkbot
homepage: https://supabase.com
metadata: {"requires_auth": true, "clawdbot":{"emoji":"⚡"}}
requires_tools: [exec, api_keys_check, define_tasks]
tags: [development, devops, supabase, database, infrastructure, hosting]
---

# Supabase Integration

Manage your Supabase projects using the Supabase CLI. Run SQL queries, manage migrations, deploy edge functions, handle secrets, and more.

## Authentication

**First, check if SUPABASE_ACCESS_TOKEN is configured:**
```tool:api_keys_check
key_name: SUPABASE_ACCESS_TOKEN
```

If not configured, ask the user to create a Personal Access Token at https://supabase.com/dashboard/account/tokens and add it in Settings > API Keys as `SUPABASE_ACCESS_TOKEN`.

The `SUPABASE_ACCESS_TOKEN` env var is automatically injected into all `exec` commands.

---

## Prerequisites

Ensure the Supabase CLI is installed:

```tool:exec
command: supabase --version
timeout: 30
```

Supabase CLI is installed by the `supabase_cli` module. If missing, reinstall via `manage_modules(action="install"
```

</details>
