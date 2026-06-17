---
name: Matthew-Wise__Umbraco-CSP-manager
source: https://github.com/Matthew-Wise/Umbraco-CSP-manager/blob/eb6ce54a164c1c7d98e56838c26f4e52c1ba80a5/CLAUDE.md
repo: Matthew-Wise/Umbraco-CSP-manager
kind: claude-md
stars: 26
last_pushed: 2026-06-14T09:22:05Z
license: mit
score: 8
domains: [backend, cms, devops]
tags: [monorepo, dotnet, cicd]
curated: 2026-06-15
curated_by: config-scout
---

# Matthew-Wise/Umbraco-CSP-manager — claude-md

**Why it's worth keeping:** The inclusion of precise Git tag prefixes for different release triggers and explicit port mappings for dev sites provides highly actionable context for agentic CI/CD and testing workflows.

**Summary:** A high-signal project manifest defining a complex monorepo structure and specific technology versions.

**Source credibility:** Niche tool with consistent, recent maintenance.

**Recency:** Very current; uses cutting-edge versions like .NET 10 and Vite 7.

**Source:** [Matthew-Wise/Umbraco-CSP-manager/CLAUDE.md](https://github.com/Matthew-Wise/Umbraco-CSP-manager/blob/eb6ce54a164c1c7d98e56838c26f4e52c1ba80a5/CLAUDE.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Umbraco Community CSP Manager

CSP management package for Umbraco CMS. Monorepo with 3 independently releasable NuGet packages.

## Project Structure

```
src/
├── Umbraco.Community.CSPManager/          # Main package (NuGet)
│   └── Client/                            # TypeScript/Lit frontend
├── Umbraco.Community.CSPManager.TestSite/ # Dev/testing site (port 44370)
├── Umbraco.Community.CSPManager.Tests/    # Unit/integration tests
├── Umbraco.Community.CSPManager.Benchmarks/
├── Directory.Build.props                  # Shared NuGet metadata
├── Directory.Packages.props               # Central package versioning
└── uSync/                                 # uSync integration packages
    ├── Umbraco.Community.CSPManager.uSync/           # Base uSync serialization
    ├── Umbraco.Community.CSPManager.uSync.Complete/  # uSync Publisher push/pull
    ├── uSync.TestSite/                    # Test site A (port 44381)
    └── uSync.TestSiteB/                   # Test site B (port 44382)
```

## Tech Stack

- Backend: .NET 10, Umbraco 17+, NPoco ORM
- Frontend: Lit 3.x, Vite 7.x, Node 22+
- Testing: NUnit (backend), Playwright (frontend)
- API: OpenAPI code generation via @hey-api/open
```

</details>
