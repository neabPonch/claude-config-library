---
name: affaan-m__ECC__django-api-claude
source: https://github.com/affaan-m/ECC/blob/5b173d2e6c11b976a0f13b2f59125e08956c1d47/docs/ja-JP/examples/django-api-CLAUDE.md
repo: affaan-m/ECC
kind: claude-md
stars: 215736
last_pushed: 2026-06-15T04:56:13Z
license: mit
score: 9
domains: [backend-api, python, django]
tags: [ddd, rest-api, tdd, best-practices]
curated: 2026-06-15
curated_by: config-scout
---

# affaan-m/ECC — claude-md

**Why it's worth keeping:** It uses explicit 'Good vs Bad' code examples to teach the AI nuance and provides complete architectural patterns (Service/View/Test) rather than just list of tools. The directory structure and specific pattern implementations prevent logic fragmentation during agentic development.

**Summary:** An opinionated blueprint for a Django REST API following Domain-Driven Design and service-layer patterns. It defines strict standards for database optimization, type safety, and testing.

**Source credibility:** High; from an active, high-star repository focused on agent harness optimization.

**Recency:** Very current, utilizing Python 3.12 and Django 5.x standards.

**Source:** [affaan-m/ECC/docs/ja-JP/examples/django-api-CLAUDE.md](https://github.com/affaan-m/ECC/blob/5b173d2e6c11b976a0f13b2f59125e08956c1d47/docs/ja-JP/examples/django-api-CLAUDE.md) · 215736★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Django REST API — プロジェクト CLAUDE.md

> PostgreSQL と Celery を使用した Django REST Framework API の実世界サンプル。
> これをプロジェクトのルートにコピーしてサービスに合わせてカスタマイズしてください。

## プロジェクト概要

**スタック:** Python 3.12+, Django 5.x, Django REST Framework, PostgreSQL, Celery + Redis, pytest, Docker Compose

**アーキテクチャ:** ビジネスドメインごとにアプリを持つドメイン駆動設計。APIレイヤーにDRF、非同期タスクにCelery、テストにpytestを使用。すべてのエンドポイントはJSONを返す — テンプレートレンダリングなし。

## 重要なルール

### Python の規約

- すべての関数シグネチャに型ヒントを付ける — `from __future__ import annotations` を使用
- `print()` 文は使用しない — `logging.getLogger(__name__)` を使用
- 文字列フォーマットにはf-stringを使用し、`%` や `.format()` は使用しない
- ファイル操作には `os.path` ではなく `pathlib.Path` を使用
- isortでインポートをソートする: stdlib、サードパーティ、ローカル（ruffにより強制）

### データベース

- すべてのクエリはDjango ORMを使用 — 生SQLは `.raw()` とパラメータ化クエリのみ
- マイグレーションはgitにコミットする — 本番環境では `--fake` を絶対に使用しない
- N+1クエリを防ぐために `select_related()` と `prefetch_related()` を使用する
- すべてのモデルには `created_at` と `updated_at` の自動フィールドが必要
- `filter()`, `order_by()`, または `WHERE` 句で使用されるフィールドにはインデックスを付ける

```python
# 悪い例: N+1クエリ
orders = Order.objects.all()
for order in orders:
    print(order.customer.name)  # 各注文ごとにDBをヒット

# 良い例: JOINによる単一クエリ
orders = Order.objects.select_related("customer").all()
```

### 認証

- `dj
```

</details>
