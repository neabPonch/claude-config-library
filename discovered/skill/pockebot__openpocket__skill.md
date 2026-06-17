---
name: pockebot__openpocket__skill
source: https://github.com/pockebot/openpocket/blob/200a97975df60e7878f7cf3bd46abe488326cf53/skills/human-auth-oauth/SKILL.md
repo: pockebot/openpocket
kind: skill
stars: 832
last_pushed: 2026-03-23T03:12:19Z
license: mit
score: 8
domains: [agents-ai, security, human-in-the-loop]
tags: [auth, oauth, credentials, security]
curated: 2026-06-15
curated_by: config-scout
---

# pockebot/openpocket — skill

**Why it's worth keeping:** It enforces critical security hygiene by instructing the agent to delete plaintext credential artifacts immediately after use. It also handles complex edge cases like multi-step authentication flows and state changes during input.

**Summary:** Provides a structured protocol for an agent to request sensitive login credentials via a UI template and execute them on-screen.

**Source credibility:** High; 832 stars indicates a significant and active project in the intelligent device space.

**Recency:** Very current; pushed within the last few months.

**Source:** [pockebot/openpocket/skills/human-auth-oauth/SKILL.md](https://github.com/pockebot/openpocket/blob/200a97975df60e7878f7cf3bd46abe488326cf53/skills/human-auth-oauth/SKILL.md) · 832★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "human-auth-oauth"
description: "Handle account login credential delegation from Human Phone. Covers username/password entry, social sign-in walls, and multi-step login flows."
metadata: {"openclaw":{"triggers":{"any":["oauth","login","sign in","credentials","username","password","account","authentication","social login","google sign"]}}}
---

# Human Auth: OAuth / Login

Use this when an app requires the user to log in with their account credentials.

## When to Trigger

- App shows a login screen with username/email and password fields.
- App redirects to a social sign-in page (Google, Apple, Facebook, etc.).
- App requires account authentication to proceed.

## How to Call

```
request_human_auth(
  capability: "oauth",
  instruction: "Please provide your login credentials for [app/service name].",
  uiTemplate: {
    fields: [
      { id: "username", label: "Username / Email", type: "text", required: true, autocomplete: "username" },
      { id: "password", label: "Password", type: "password", required: true, autocomplete: "current-password" }
    ],
    artifactKind: "credentials",
    requireArtifactOnApprove: true,
    title: "Account Login Required",
    summary:
```

</details>
