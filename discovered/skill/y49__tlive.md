---
name: y49__tlive
source: https://github.com/y49/tlive/blob/9580aae847b63c3c869243c2fec5eb0f5084427c/SKILL.md
repo: y49/tlive
kind: skill
stars: 203
last_pushed: 2026-04-20T10:14:43Z
license: mit
score: 8
domains: [cli-tools, agents-ai]
tags: [im-bridge, system-management, interactive-setup]
curated: 2026-06-15
curated_by: config-scout
---

# y49/tlive — skill

**Why it's worth keeping:** Demonstrates excellent state-management logic (checking config existence before execution) and high-quality interactive UX patterns like single-field secret collection and masked output.

**Summary:** Provides an integrated IM bridge allowing users to interact with Claude Code via Telegram, Discord, or Feishu. It manages local configuration, runtime status, and a multi-step interactive setup wizard.

**Source credibility:** High; 203 stars suggests a functional, community-vetted tool rather than a throwaway script.

**Recency:** Current; updated within the last few months.

**Source:** [y49/tlive/SKILL.md](https://github.com/y49/tlive/blob/9580aae847b63c3c869243c2fec5eb0f5084427c/SKILL.md) · 203★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tlive
description: |
  IM bridge for AI coding tools — chat with Claude Code / Codex from
  Telegram, Discord, or Feishu. Approve permissions, get streaming responses,
  manage sessions from your phone.
  Use for: starting IM bridge, configuring IM platforms, checking status,
  diagnosing issues.
  Trigger phrases: "tlive", "IM bridge", "消息桥接", "手机交互", "启动桥接",
  "连接飞书", "连接Telegram", "诊断", "查看日志", "配置".
  Do NOT use for: building bots, webhook integrations, or general coding tasks.
argument-hint: "setup | stop | status | logs [N] | reconfigure | doctor"
allowed-tools:
  - Bash
  - Read
  - Write
  - Edit
  - AskUserQuestion
  - Grep
  - Glob
---

# TLive — IM Bridge Skill

You are managing the TLive IM Bridge — bidirectional chat with AI coding tools from Telegram, Discord, or Feishu.

The Bridge uses the Claude Agent SDK (or Codex SDK) to interact with the AI coding tool. It is completely independent from the optional Go Core web terminal server.

User data: `~/.tlive/`

## Command Parsing

| User says (examples) | Subcommand |
|---|---|
| (no args), `start`, `启动`, `启动桥接` | start |
| `setup`, `configure`, `配置`, `帮我连接 Telegram` | setup |
| `stop`, `停止`, `关闭` | stop |
| `s
```

</details>
