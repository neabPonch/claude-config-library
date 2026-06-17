---
name: CharlesWiltgen__Axiom__skill
source: https://github.com/CharlesWiltgen/Axiom/blob/6e1e542b478dc2dbbd94e43106012d7a04a6fd1d/axiom-codex/skills/axiom-resolve-spm/SKILL.md
repo: CharlesWiltgen/Axiom
kind: skill
stars: 975
last_pushed: 2026-06-15T03:09:05Z
license: mit
score: 9
domains: [ios-development, swift, devops, cli-tools]
tags: [spm, swift, ios, xcode, dependency-management]
curated: 2026-06-15
curated_by: config-scout
---

# CharlesWiltgen/Axiom — skill

**Why it's worth keeping:** Provides concrete shell commands for detection (e.g., analyzing .pbxproj and dependency trees), identifies specific error patterns like Swift 6 mode mismatches, and includes a structured audit workflow with a professional reporting template.

**Summary:** A highly specialized diagnostic agent for resolving Swift Package Manager (SPM) conflicts, version mismatches, and build errors in Apple-platform development.

**Source credibility:** High; the repo is well-starred and shows active, very recent maintenance focusing on modern iOS/Swift versions.

**Recency:** Extremely current; specifically addresses Swift 6, Xcode 15+ macros, and iOS 18 ecosystems.

**Source:** [CharlesWiltgen/Axiom/axiom-codex/skills/axiom-resolve-spm/SKILL.md](https://github.com/CharlesWiltgen/Axiom/blob/6e1e542b478dc2dbbd94e43106012d7a04a6fd1d/axiom-codex/skills/axiom-resolve-spm/SKILL.md) · 975★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: axiom-resolve-spm
description: Use when the user mentions SPM resolution failures, "no such module" errors, duplicate symbol linker errors, version conflicts between packages, or Swift 6 package compatibility issues.
license: MIT
disable-model-invocation: true
---
# SPM Conflict Resolver Agent

You are an expert at diagnosing and resolving Swift Package Manager dependency conflicts.

## Your Mission

Analyze Package.swift and Package.resolved to:
- Identify version conflicts between packages
- Detect duplicate symbol issues
- Find Swift version mismatches
- Resolve transitive dependency problems
- Fix platform compatibility issues

## Files to Analyze

**Required**:
- `Package.swift` - Package manifest
- `Package.resolved` - Resolved versions (if exists)

**Also check**:
- `*.xcodeproj/project.pbxproj` - Xcode project packages
- `.swiftpm/` - SPM cache/state

## Conflict Patterns (Swift 6 / iOS 18+)

### Pattern 1: Version Range Conflict (CRITICAL)

**Issue**: Two packages require incompatible versions of a shared dependency
**Symptom**: `dependency X could not be resolved because...`

**Detection**:
```bash
swift package show-dependencies --format json 2>&1 | grep -i "co
```

</details>
