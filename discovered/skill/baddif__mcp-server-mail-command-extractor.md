---
name: baddif__mcp-server-mail-command-extractor
source: https://github.com/baddif/mcp-server-mail-command-extractor/blob/c57f8250b502c9d5347f361f069bfdfbfed2c6ae/Skill.md
repo: baddif/mcp-server-mail-command-extractor
kind: skill
stars: 0
last_pushed: 2026-04-01T10:06:12Z
license: mit
score: 7
domains: [automation, agents-ai, cli-tools]
tags: [mcp, email-automation, rule-engine]
curated: 2026-06-14
curated_by: config-scout
---

# baddif/mcp-server-mail-command-extractor — skill

**Why it's worth keeping:** Provides a rigorous input/output contract with explicit error states. The inclusion of a 'priority' field in detection rules is a highly transferable technique for resolving overlapping agent triggers.

**Summary:** Converts raw email data into structured, actionable commands using rule-based matching logic including priority and duplicate handling.

**Source credibility:** Low; the repository has zero stars and appears to be an individual project.

**Recency:** Current; follows modern Model Context Protocol (MCP) standards used by Claude Code.

**Source:** [baddif/mcp-server-mail-command-extractor/Skill.md](https://github.com/baddif/mcp-server-mail-command-extractor/blob/c57f8250b502c9d5347f361f069bfdfbfed2c6ae/Skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Mail Command Extractor Skill

This skill extracts actionable commands from a list of emails using detection rules.

## Input Schema

- `emails` (required): array of email objects (directly the `matched_emails` array from gmail_check output)
  - each email object fields (required): `sender`, `sender_email`, `subject`, `content`, `date_received`, `email_id`

- `detection_rules` (required): object containing `rules` array. Each rule:
  - `sender` (required): exact email address to match against `sender_email` (case-insensitive)
  - `subjects` (optional): array of title keywords (string). Title matches if any keyword is contained in subject.
  - `contents` (optional): array of content keywords (string). Content matches if any keyword is contained in content.
  - `action` (required): command name to produce
  - `parameters` (optional): object, passed through to the produced command
  - `priority` (optional): integer priority (lower is higher priority)

- `merge_duplicates` (optional): boolean, default true

## Output Schema

All outputs MUST follow the core contract:

Success:

```json
{
  "success": true,
  "data": {
    "extracted_commands": [
      {
        "command": "...",
```

</details>
