---
name: 2chevskii__wgconf
source: https://github.com/2chevskii/wgconf/blob/49f4370a027c47938e62d33d9cc7d775d601c77d/CLAUDE.md
repo: 2chevskii/wgconf
kind: claude-md
stars: 1
last_pushed: 2026-03-04T04:01:52Z
license: mit
score: 8
domains: [dotnet, security, cli-tools]
tags: [architecture-mapping, patterns, .net]
curated: 2026-06-16
curated_by: config-scout
---

# 2chevskii/wgconf — claude-md

**Why it's worth keeping:** Demonstrates the 'knowledge hub' pattern by linking to granular docs in a .claude/ directory and explicitly defining domain-specific coding patterns like error handling and API design.

**Summary:** Provides high-level technical specifications, build commands, and a structured map to specialized documentation.

**Source credibility:** Small repository, but the highly structured documentation suggests a disciplined author.

**Recency:** Very current; uses modern .NET 8.0 and contemporary tooling standards.

**Source:** [2chevskii/wgconf/CLAUDE.md](https://github.com/2chevskii/wgconf/blob/49f4370a027c47938e62d33d9cc7d775d601c77d/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

**WgConf**: .NET library for WireGuard configuration files with strongly-typed models.

## Quick Reference

- **Framework**: .NET 8.0 LTS
- **SDK**: 10.0.102 (global.json)
- **Solution**: XML `.slnx` format
- **Formatter**: CSharpier 1.2.5

### Commands

```bash
dotnet build                    # Build
dotnet test                     # Run tests
dotnet csharpier format .       # Format code
```

### Projects

- **WgConf**: Base library (Interface/Peer configs, CIDR, Endpoint, Reader/Writer)
- **WgConf.Amnezia**: Extension with 20 AmneziaWG obfuscation parameters (H1-H4 support single values and ranges)

### Documentation

- [Architecture](.claude/architecture.md) - Domain models, reader/writer patterns, extensibility
- [Development](.claude/development.md) - Build setup, tooling, code style
- [Testing](.claude/testing.md) - Test structure, coverage (80% threshold)
- [CI/CD](.claude/cicd.md) - Pipeline, versioning, release process
- [Project Structure](.claude/project-structure.md) - File organization, dependencies

### Key Patterns

- **Dual API**: `Read()`/`TryRead()` (throw vs bool return)
- **Error handling**: Structured `ParseError` with context aggregation
- **Exte
```

</details>
