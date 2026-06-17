---
name: K9i-0__ccpocket
source: https://github.com/K9i-0/ccpocket/blob/fe18fccdc68632d9cb4661e8a690f80108572a75/CLAUDE.md
repo: K9i-0/ccpocket
kind: claude-md
stars: 896
last_pushed: 2026-06-12T14:15:42Z
license: mit
score: 9
domains: [mobile-app, fullstack, agents-ai, cli-tools]
tags: [websocket, flutter, mcp, orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# K9i-0/ccpocket — claude-md

**Why it's worth keeping:** The 'MCP Tool vs CLI' decision matrix is a masterclass in guiding agents on when to use specific toolsets, alongside its rigorous 3-phase development workflow (Plan/Implement/Verify).

**Summary:** A highly sophisticated instruction file for a full-stack mobile/bridge project that defines precise communication protocols and tool-use heuristics.

**Source credibility:** Highly credible; the repo has significant star count (896) and active maintenance.

**Recency:** Current; it includes modern MCP tool usage patterns and is explicitly designed for Claude Code.

**Source:** [K9i-0/ccpocket/CLAUDE.md](https://github.com/K9i-0/ccpocket/blob/fe18fccdc68632d9cb4661e8a690f80108572a75/CLAUDE.md) · 896★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ccpocket

Claude Code / Codex 対応モバイルクライアント

## プロジェクト構成

```
ccpocket/
├── packages/bridge/    # Bridge Server (TypeScript, WebSocket)
│   └── src/
│       ├── index.ts           # エントリーポイント
│       ├── websocket.ts       # WebSocket接続管理・マルチセッション
│       ├── session.ts         # セッション管理 (SessionManager)
│       ├── claude-process.ts  # Claude CLIプロセス管理 (SDK経由)
│       ├── codex-process.ts   # Codex CLIプロセス管理 (SDK経由)
│       └── parser.ts          # stream-json パース・型定義
├── apps/mobile/        # Flutter Mobile App
│   └── lib/
│       ├── main.dart
│       ├── features/                      # Feature-first ディレクトリ
│       │   ├── chat_session/              # 共通チャットセッション (state/widgets)
│       │   ├── claude_session/            # Claude Code セッション画面
│       │   ├── codex_session/             # Codex セッション画面
│       │   ├── session_list/              # セッション一覧 (ホーム)
│       │   ├── connection/                # 接続・マシン管理
│       │   ├── diff/                      # Diff表示画面
│       │   ├── gallery/                   # ギャラリー画面
│       │   ├── message_images/            # メッセージ画像ビューア
│       │   ├── prompt_history/            # プロンプト履歴
│       │   ├── settings/                  # 設定画面
│
```

</details>
