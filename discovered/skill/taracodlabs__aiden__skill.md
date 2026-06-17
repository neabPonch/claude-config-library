---
name: taracodlabs__aiden__skill
source: https://github.com/taracodlabs/aiden/blob/02667a21cf69459ef9abd37ccd5668302dd637ad/skills/github-auth/SKILL.md
repo: taracodlabs/aiden
kind: skill
stars: 405
last_pushed: 2026-05-27T16:13:05Z
license: agpl-3.0
score: 7
domains: [cli-tools, security, devops]
tags: [github, auth, git, ssh]
curated: 2026-06-15
curated_by: config-scout
---

# taracodlabs/aiden — skill

**Why it's worth keeping:** Includes specific verification commands (like `ssh -T`) to ensure the setup actually works. It also covers protocol transitions such as switching from HTTPS to SSH.

**Summary:** Provides comprehensive procedures for GitHub authentication via gh CLI, SSH keys, and HTTPS PATs.

**Source credibility:** High; a well-starred, actively maintained repository with specialized focus.

**Recency:** 

**Source:** [taracodlabs/aiden/skills/github-auth/SKILL.md](https://github.com/taracodlabs/aiden/blob/02667a21cf69459ef9abd37ccd5668302dd637ad/skills/github-auth/SKILL.md) · 405★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: github-auth
description: GitHub auth setup via gh CLI, SSH keys, HTTPS PATs
category: developer
version: 1.0.0
origin: aiden
license: Apache-2.0
tags: github, auth, ssh, pat, token, credentials, gh-cli, authentication, git, https
---

# GitHub Authentication Setup

Configure GitHub authentication for `git` and `gh` CLI operations using the GitHub CLI (`gh`), SSH keys, or HTTPS personal access tokens (PATs).

## When to Use

- User needs to authenticate with GitHub from a new machine
- User is getting `Permission denied (publickey)` or `Authentication failed` errors
- User wants to switch from HTTPS to SSH authentication
- User wants to create or rotate a personal access token
- User wants to verify their current GitHub credentials are working

## How to Use

### 1. Authenticate with gh CLI (recommended)

```powershell
# Interactive login — opens browser for OAuth
gh auth login

# Choose: GitHub.com → HTTPS → Authenticate with browser
# Or choose SSH if preferred

# Verify authentication
gh auth status
```

### 2. Create an SSH key

```powershell
# Generate Ed25519 key (modern, secure)
ssh-keygen -t ed25519 -C "your-email@example.com" -f "$env:USERPROFILE\.ssh\github_ed255
```

</details>
