---
name: J-Tech-Japan__Sekiban__claude
source: https://github.com/J-Tech-Japan/Sekiban/blob/d1cfd8a5e57887246a39a77961e2ad2b2ae5c8c5/tasks/876/infra/v2/claude.md
repo: J-Tech-Japan/Sekiban
kind: claude-md
stars: 335
last_pushed: 2026-05-27T15:08:38Z
license: other
score: 9
domains: [cloud-infrastructure, backend-architecture, devops]
tags: [aws, csharp, orleans, iac]
curated: 2026-06-16
curated_by: config-scout
---

# J-Tech-Japan/Sekiban — claude-md

**Why it's worth keeping:** The document uses structured comparison tables (Option A vs B) to justify architectural decisions and provides exact configuration snippets (NuGet, Silo code, Security Groups) that eliminate ambiguity.

**Summary:** A highly detailed AWS architecture specification for a Microsoft Orleans-based system, including trade-off analyses between different database and language providers.

**Source credibility:** High; part of the Sekiban project, a starred C# event-sourcing framework.

**Recency:** Current; uses modern AWS/Orleans/CDK patterns.

**Source:** [J-Tech-Japan/Sekiban/tasks/876/infra/v2/claude.md](https://github.com/J-Tech-Japan/Sekiban/blob/d1cfd8a5e57887246a39a77961e2ad2b2ae5c8c5/tasks/876/infra/v2/claude.md) · 335★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AWS Infrastructure Design v2 - Sekiban DCB + Orleans

> **v2 の目的**: 既存設計 (orleans-aws.md, claude.v1.md, iac-aws.md, iac-aws-claude.md) を統合し、矛盾点を整理した上でベストな設計を提案する。

---

## 既存設計のレビュー

### 共通点（確定事項）
| 項目 | 決定内容 |
|------|----------|
| コンピュート | ECS Fargate |
| ストリーム | SQS (`Microsoft.Orleans.Streaming.SQS`) |
| イベントストア | DynamoDB (DCB) |
| スナップショット | S3 |
| 外部公開 | ALB (HTTP/HTTPS のみ) |
| 内部通信 | Silo Port (11111), Gateway Port (30000) - VPC 内部のみ |
| IaC | AWS CDK |
| CI/CD | GitHub Actions + OIDC |

### 議論点（選択が必要）

| 項目 | Option A | Option B | 考察 |
|------|----------|----------|------|
| Orleans クラスタ/State | DynamoDB | RDS PostgreSQL | 後述 |
| CDK 言語 | C# | TypeScript | 後述 |
| 初期構成 | 2 silo | 1 silo | コスト vs 可用性 |

---

## 議論点の整理

### 1. Orleans データストア: DynamoDB vs RDS

#### DynamoDB (claude.v1.md の推奨)
```
✅ 長所
- 完全サーバーレス、従量課金
- Free Tier が永続 (25 RCU/WCU)
- DCB イベントストアと同じ技術スタック
- 運用が簡素

❌ 短所
- Orleans DynamoDB Provider は AdoNet より新しい
- Reminders Provider の成熟度に懸念あり
- トランザクション機能が限定的
```

#### RDS PostgreSQL (orleans-aws.md の推奨)
```
✅ 長所
- AdoNet Provider は Orleans で最も成熟
- トランザクション対応
- 既存の運用ノウハウが豊富
- Reminders/PubSubStore が安定

❌ 短所
- 固定費 (~$12/月、Free Tier 後)
- 別のデータベース技術が増える
- 運用コストが若干増加
```

</details>
