---
name: 1amageek__SwiftAgent
source: https://github.com/1amageek/SwiftAgent/blob/7b4db2fa3b36add8d6314cb365e3e20f3e6e703b/CLAUDE.md
repo: 1amageek/SwiftAgent
kind: claude-md
stars: 89
last_pushed: 2026-05-01T06:32:51Z
license: unknown
score: 9
domains: [swift, ai-agents, frameworks]
tags: [dsl, type-safety, concurrency]
curated: 2026-06-16
curated_by: config-scout
---

# 1amageek/SwiftAgent — claude-md

**Why it's worth keeping:** Includes highly specific code patterns for custom DSLs like @Memory/Relay and @Contextable macros. This density allows an LLM to replicate complex, non-standard logic correctly.

**Summary:** A high-density technical guide for a type-safe AI agent framework in Swift. It defines unique architectural patterns for state management and task propagation.

**Source credibility:** 89 stars on GitHub; recently active (2 months ago).

**Recency:** Very current, utilizing modern Swift concurrency and macro patterns.

**Source:** [1amageek/SwiftAgent/CLAUDE.md](https://github.com/1amageek/SwiftAgent/blob/7b4db2fa3b36add8d6314cb365e3e20f3e6e703b/CLAUDE.md) · 89★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SwiftAgent

Apple FoundationModelsを基盤とした型安全で宣言的なAIエージェントフレームワーク。

> **Note**: デフォルトはApple FoundationModelsを使用。`--traits OpenFoundationModels` で OpenFoundationModels に切り替え可能。

## コア概念

| 概念 | 説明 |
|------|------|
| **Step** | `Input -> Output` の非同期変換単位。`run(_:)` を直接実装するか、`body` を定義して宣言的に合成 |
| **Session** | TaskLocalベースのセッション伝播（`@Session`, `.session()`） |
| **Memory/Relay** | Step間の状態共有（`@Memory` で保持、`$` で `Relay` を取得） |
| **Context** | 汎用TaskLocal伝播（`@Contextable`, `@Context`, `.context()`） |
| **Generate** | LLMによる構造化出力生成 |

## Step 一覧

| 種別 | Steps |
|------|-------|
| プリミティブ | `Transform`, `Generate`, `GenerateText`, `EmptyStep`, `Join`, `Gate` |
| 合成 | `Chain2-8`, `Pipeline`, `Parallel`, `Race`, `Loop`, `Map`, `Reduce` |
| 修飾 | `Monitor`, `TracingStep`, `AnyStep` |

## 基本パターン

```swift
// Session伝播（TaskLocal経由で自動伝播）
struct MyStep: Step {
    @Session var session: LanguageModelSession
    func run(_ input: String) async throws -> String {
        try await session.respond { Prompt(input) }.content
    }
}
try await MyStep().session(session).run("Hello")

// Memory/Relay による状態共有
struct OrchestratorStep: Step {
    @Memory var visitedURLs: Set<URL> = []  // 状態を保持

    func run(_
```

</details>
