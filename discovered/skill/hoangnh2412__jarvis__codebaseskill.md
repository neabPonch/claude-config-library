---
name: hoangnh2412__jarvis__codebaseskill
source: https://github.com/hoangnh2412/jarvis/blob/8050d0a27ea109c43a234f3cefc6ba682f793ef9/CodeBaseSkill.md
repo: hoangnh2412/jarvis
kind: skill
stars: 12
last_pushed: 2026-06-04T16:30:05Z
license: unknown
score: 8
domains: [backend-api, dotnet-core, architecture]
tags: [refactoring, design-patterns, dependency-injection, infrastructure]
curated: 2026-06-14
curated_by: config-scout
---

# hoangnh2412/jarvis — skill

**Why it's worth keeping:** Includes highly specific patterns for 'safe' dependency injection (using TryAdd), configuration design via sentinel values, and structured file organization to prevent technical debt in modular systems.

**Summary:** Provides rigorous architectural standards and refactoring rules for building infrastructure-level .NET libraries. It focuses on clear boundaries between core framework logic and host application implementations.

**Source credibility:** Low star count but shows high-level engineering sophistication typical of professional-grade frameworks.

**Recency:** Extremely current; references C# 12 features like primary constructors and targets .NET 9.

**Source:** [hoangnh2412/jarvis/CodeBaseSkill.md](https://github.com/hoangnh2412/jarvis/blob/8050d0a27ea109c43a234f3cefc6ba682f793ef9/CodeBaseSkill.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Jarvis Codebase Skill — Refactoring Rules

Tài liệu này mô tả **mindset, behavior và style code** rút ra từ `Jarvis.HealthChecks`, `Jarvis.OpenTelemetry`, `Jarvis.EntityFramework`. Dùng làm checklist khi refactor các module khác (Caching, BlobStorage, Notification, Authentication, …).

---

## 1. Triết lý kiến trúc

### 1.1 Jarvis.* = thư viện hạ tầng, không phải app code

- Mỗi project là **NuGet package** độc lập (`PackageId`, `GeneratePackageOnBuild`, `net9.0`).
- Phụ thuộc `Jarvis.Domain` cho contract; implementation nằm trong project Jarvis tương ứng.
- Host (Sample / app thật) chỉ gọi vài dòng extension; logic domain nằm ở host.

### 1.2 Core vs Host-owned (ranh giới rõ)

| Jarvis cung cấp (core) | Host tự đăng ký (owned) |
|------------------------|-------------------------|
| Liveness, startup, process-resources | Readiness: SQL, Redis, HTTP deps, … |
| Map `/health/live`, `/ready`, `/startup`, `/health` | Custom `IHealthCheck` có tag `readiness` |
| OTEL resource, ASP.NET/HttpClient trace, OTLP mặc định | `ITraceInstrumentation`, enricher, exporter plugin |
| Repository base, multitenancy resolver, `AddCoreDbContext` | `TDbContext`, migration, connection string thật, UoW
```

</details>
