---
name: iota-uz__iota-sdk__claude
source: https://github.com/iota-uz/iota-sdk/blob/cbc71edc1d718be8d92d26ff57410bc21994c501/pkg/lens/CLAUDE.md
repo: iota-uz/iota-sdk
kind: claude-md
stars: 440
last_pushed: 2026-06-14T23:31:31Z
license: apache-2.0
score: 9
domains: [backend, data-visualization]
tags: [architectural-patterns, framework-spec]
curated: 2026-06-15
curated_by: config-scout
---

# iota-uz/iota-sdk — claude-md

**Why it's worth keeping:** It defines explicit 'contracts' between controllers and templates, provides checklists for adding dimensions, and clarifies complex state-handling rules like drill URL formats.

**Summary:** Provides rigorous architectural guidelines and implementation contracts for the 'Lens' dashboard framework.

**Source credibility:** High; comes from a professional-grade Go ERP SDK with active maintenance.

**Recency:** Current; aligns with modern HTMX/Go/Templ development patterns used today.

**Source:** [iota-uz/iota-sdk/pkg/lens/CLAUDE.md](https://github.com/iota-uz/iota-sdk/blob/cbc71edc1d718be8d92d26ff57410bc21994c501/pkg/lens/CLAUDE.md) · 440★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Lens Dashboard Framework

Lens supports two patterns:

- Manual `lens.DashboardSpec`: use when the layout and datasets are bespoke and there is no multi-level drill flow.
- `cube.New(...)`: use when you want a dashboard that starts with KPIs plus dimension panels and drills through ordered `_f=dimension:value` state.

## Manual DashboardSpec

Use plain `lens.DashboardSpec` when:

- Panels are unrelated to one another
- You already know the exact dataset graph you want
- Drill-through is row/panel specific instead of hierarchical cube drilling
- A dashboard is mostly one-off presentation work

## Cube Pattern

Use `cube.New(...)` when:

- The dashboard is a KPI summary plus a set of dimensions
- Each click should narrow the same analytical slice
- Raw leaf views should receive accumulated drill context
- You want Lens to build breadcrumbs, remaining-dimension pills, and chart drill actions for you

Basic flow:

```go
spec := cube.New("sales", "Sales Overview").
	SQL("primary", "insurance.contracts c").
	ParamLiteral("tenant_id", tenantID).
	Where("(c.tenant_id = @tenant_id OR c.tenant_id IS NULL)").
	Dimension("product", "Product").
	Column("COALESCE(pr.id::text, '')").
	LabelColu
```

</details>
