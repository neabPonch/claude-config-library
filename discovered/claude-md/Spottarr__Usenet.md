---
name: Spottarr__Usenet
source: https://github.com/Spottarr/Usenet/blob/2d24300c718659cd805c9bf5c861d897381f8d21/CLAUDE.md
repo: Spottarr/Usenet
kind: claude-md
stars: 3
last_pushed: 2026-06-14T18:58:31Z
license: mit
score: 8
domains: [.net, backend]
tags: [csharp, dotnet, ci-cd]
curated: 2026-06-15
curated_by: config-scout
---

# Spottarr/Usenet — claude-md

**Why it's worth keeping:** Highly effective use of negative constraints (no warning suppression) and precise instructions for central package management via Directory.Packages.props.

**Summary:** Provides strict coding standards, CI/CD workflows, and specific technical constraints for a .NET project.

**Source credibility:** A niche library with high recent activity and clear-cut development standards.

**Recency:** Current; explicitly mentions Claude Code and modern .NET workflows.

**Source:** [Spottarr/Usenet/CLAUDE.md](https://github.com/Spottarr/Usenet/blob/2d24300c718659cd805c9bf5c861d897381f8d21/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code (and any other AI agent or human) working in this repository.

If you are adding documentation, prefer extending the files under `docs/` and updating the index below. Use [Mermaid](https://mermaid.js.org/) for any diagrams or charts — GitHub renders them natively. Do not draw diagrams as ASCII art.

## Key conventions

- **Use idiomatic C# with the latest language features.**

## CI

`.github/workflows/build-and-test.yml` (on push/PR to `main`): `dotnet tool restore` → `dotnet restore` → CSharpier check → `dotnet build` → CodeQL (public repos) → `dotnet test` with cobertura coverage. Test results and coverage are posted as sticky PR comments. A separate scheduled `codeql.yml` re-runs CodeQL weekly.

`.github/workflows/release.yml` (on GitHub release): `dotnet pack` then `dotnet nuget push` to publish the `Spottarr.Usenet` package to NuGet, versioned from the release tag.

## Notes for AI agents

- **Always run CSharpier** (`dotnet csharpier format .`) after writing C# — CI fails otherwise and `TreatWarningsAsErrors=true` will catch a lot too.
- **Don't pin package versions in `.csproj`** — add or update the `PackageVersion` entry in `Directory.
```

</details>
