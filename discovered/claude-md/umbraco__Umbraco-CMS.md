---
name: umbraco__Umbraco-CMS
source: https://github.com/umbraco/Umbraco-CMS/blob/ae92b0b0a94418eeccd44ec640f4bd667b6b7cce/CLAUDE.md
repo: umbraco/Umbraco-CMS
kind: claude-md
stars: 5201
last_pushed: 2026-06-15T05:21:59Z
license: mit
score: 8
domains: [backend-api, .net]
tags: [architecture, workflow, dotnet]
curated: 2026-06-15
curated_by: config-scout
---

# umbraco/Umbraco-CMS — claude-md

**Why it's worth keeping:** Uses explicit dependency flow diagrams to prevent architectural violations and provides strict branching/naming protocols for Git automation.

**Summary:** A high-level architectural blueprint and workflow specification for a large-scale multi-project ecosystem.

**Source credibility:** High; Umbraco is an industry-standard, highly-starred enterprise CMS.

**Recency:** Current (references .NET 10.0).

**Source:** [umbraco/Umbraco-CMS/CLAUDE.md](https://github.com/umbraco/Umbraco-CMS/blob/ae92b0b0a94418eeccd44ec640f4bd667b6b7cce/CLAUDE.md) · 5201★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Umbraco CMS - Multi-Project Repository

Enterprise-grade CMS built on .NET 10.0. This repository contains 21 production projects organized in a layered architecture with clear separation of concerns.

**Repository**: https://github.com/umbraco/Umbraco-CMS
**License**: MIT
**Main Branch**: `main`

---

## 1. Overview

### What This Repository Contains

**21 Production Projects** organized in 3 main categories:

1. **Core Architecture** (Domain & Infrastructure)
   - `Umbraco.Core` - Interface contracts, domain models, notifications
   - `Umbraco.Infrastructure` - Service implementations, data access, caching

2. **Web & APIs** (Presentation Layer)
   - `Umbraco.Web.UI` - Main ASP.NET Core web application
   - `Umbraco.Web.Common` - Shared web functionality, controllers, middleware
   - `Umbraco.Cms.Api.Management` - Backoffice Management API (REST)
   - `Umbraco.Cms.Api.Delivery` - Content Delivery API (headless)
   - `Umbraco.Cms.Api.Common` - Shared API infrastructure

3. **Specialized Features** (Pluggable Modules)
   - Persistence: EF Core (modern), NPoco (legacy) for SQL Server & SQLite
   - Caching: `PublishedCache.HybridCache` (in-memory + distributed)
   - Search: `Examine
```

</details>
