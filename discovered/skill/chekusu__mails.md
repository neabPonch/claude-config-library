---
name: chekusu__mails
source: https://github.com/chekusu/mails/blob/cb2dc7e01137489b5e22a666f34457f5588c7a12/skill.md
repo: chekusu/mails
kind: skill
stars: 326
last_pushed: 2026-06-10T06:29:18Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, email]
tags: [email, verification-code, automation]
curated: 2026-06-14
curated_by: config-scout
---

# chekusu/mails — skill

**Why it's worth keeping:** The 'mails code' command implements a critical agentic pattern: a high-level, polling-based primitive for capturing verification codes without complex IMAP parsing.

**Summary:** A specialized CLI toolset that provides AI agents with structured email capabilities including sending, searching, and inbox management.

**Source credibility:** 326 stars suggests a highly useful, community-vetted tool for niche automation tasks.

**Recency:** Current; uses modern developer tooling like Bun and Cloudflare Workers.

**Source:** [chekusu/mails/skill.md](https://github.com/chekusu/mails/blob/cb2dc7e01137489b5e22a666f34457f5588c7a12/skill.md) · 326★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# mails — Email for AI Agents

Send and receive emails. Get a free `@mails.dev` mailbox or use your own domain.

## Onboarding (follow these steps in order)

### Step 1: Install

```bash
npm install -g mails
```

Verify: `mails version` should print a version number.

### Step 2: Claim a mailbox

You need a `@mails.dev` email address. This requires a human to approve (one-time).

```bash
mails claim <pick-a-name>
```

**If you have a browser** (local machine): it will open automatically. The human approves, and the CLI receives the API key.

**If you don't have a browser** (sandbox, SSH, CI): the CLI will show a code like this:

```
  Claiming myagent@mails.dev

  To complete, ask a human to visit:

    https://mails.dev

  and enter this code:

    KDNR-CHPC

  Waiting...
```

Relay the URL and code to your human user. Once they confirm, the CLI will continue and save the credentials to `~/.mails/config.json`.

Verify: `mails config get mailbox` should print your address. `mails config get api_key` should print `mk_...`.

### Step 3: Test receiving — check your inbox

Your mailbox is ready to receive emails. Check it:

```bash
mails inbox
```

Expected: `No emails found.` (empty i
```

</details>
