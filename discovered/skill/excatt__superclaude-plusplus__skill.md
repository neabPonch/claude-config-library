---
name: excatt__superclaude-plusplus__skill
source: https://github.com/excatt/superclaude-plusplus/blob/9c36a87a9edcfed243bf4de922e3bf4f592940f6/skills/graphql/SKILL.md
repo: excatt/superclaude-plusplus
kind: skill
stars: 13
last_pushed: 2026-05-20T02:13:12Z
license: mit
score: 8
domains: [backend-api, graphql]
tags: [graphql, schema-design, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# excatt/superclaude-plusplus — skill

**Why it's worth keeping:** Includes high-value industry patterns like Relay Connection pagination, N+1 prevention via DataLoader, and directive-based authentication logic.

**Summary:** Provides a comprehensive blueprint for enterprise-grade GraphQL schema design, focusing on scalability, performance, and security.

**Source credibility:** Specialized repository containing curated architectural standards.

**Recency:** Current; reflects modern industry standards for GraphQL implementation.

**Source:** [excatt/superclaude-plusplus/skills/graphql/SKILL.md](https://github.com/excatt/superclaude-plusplus/blob/9c36a87a9edcfed243bf4de922e3bf4f592940f6/skills/graphql/SKILL.md) · 13★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "graphql"
description: "GraphQL 스키마 설계 가이드를 실행합니다."
user-invocable: true
---
# GraphQL Skill

GraphQL 스키마 설계 가이드를 실행합니다.

## 스키마 기본

### 타입 정의
```graphql
# 스칼라 타입
type User {
  id: ID!
  name: String!
  email: String!
  age: Int
  isActive: Boolean!
  balance: Float
  createdAt: DateTime!
}

# 열거형
enum OrderStatus {
  PENDING
  PROCESSING
  SHIPPED
  DELIVERED
  CANCELLED
}

# 인터페이스
interface Node {
  id: ID!
}

type User implements Node {
  id: ID!
  name: String!
}

# 유니온
union SearchResult = User | Product | Order
```

### 관계 모델링
```graphql
type User {
  id: ID!
  name: String!
  orders: [Order!]!          # 1:N
  profile: Profile           # 1:1
  friends: [User!]!          # N:N
}

type Order {
  id: ID!
  user: User!                # N:1
  items: [OrderItem!]!
}

type OrderItem {
  id: ID!
  product: Product!
  quantity: Int!
}
```

## Query 설계

### 기본 쿼리
```graphql
type Query {
  # 단일 조회
  user(id: ID!): User

  # 목록 조회 (페이지네이션)
  users(
    first: Int
    after: String
    filter: UserFilter
    orderBy: UserOrderBy
  ): UserConnection!

  # 검색
  search(query: String!): [SearchResult!]!

  # 뷰어 패턴 (현재 사용자)
  viewer: User
}

# 필터 입력
input UserFilter {
  status: Use
```

</details>
