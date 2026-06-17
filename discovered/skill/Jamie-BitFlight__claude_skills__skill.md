---
name: Jamie-BitFlight__claude_skills__skill
source: https://github.com/Jamie-BitFlight/claude_skills/blob/058c3a80e01b8e1b5c81d2f07a54e6fe4714aa34/plugins/dasel/skills/enterprise-maven-pom/SKILL.md
repo: Jamie-BitFlight/claude_skills
kind: skill
stars: 52
last_pushed: 2026-06-15T01:24:55Z
license: mit
score: 8
domains: [backend, java, cli-tools]
tags: [maven, xml, dasel, dependency-management]
curated: 2026-06-15
curated_by: config-scout
---

# Jamie-BitFlight/claude_skills — skill

**Why it's worth keeping:** Uses a structured CLI tool (dasel) rather than fragile regex/grep, which ensures reliable data extraction; it also correctly addresses enterprise nuances like dependencyManagement vs dependencies.

**Summary:** Provides high-precision 'dasel' commands for querying Maven POM XML files, including dependency filtering, scope analysis, and module hierarchy extraction.

**Source credibility:** The repo shows active maintenance and the content is highly specialized for professional Java environments.

**Recency:** Very current; utilizes dasel v3 syntax optimized for modern CLI-based agent workflows.

**Source:** [Jamie-BitFlight/claude_skills/plugins/dasel/skills/enterprise-maven-pom/SKILL.md](https://github.com/Jamie-BitFlight/claude_skills/blob/058c3a80e01b8e1b5c81d2f07a54e6fe4714aa34/plugins/dasel/skills/enterprise-maven-pom/SKILL.md) · 52★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: enterprise-maven-pom
description: Dasel v3 selector patterns for Maven POM XML files — use when querying dependency versions, filtering by groupId or scope, extracting module hierarchy from parent POMs, or detecting version conflicts across enterprise multi-module Java projects. Load this skill when working with pom.xml files using dasel.
---

# Maven POM Query Patterns

<when_to_use>

Load this skill when querying any `pom.xml` file — extracting dependency versions, filtering by groupId or scope, mapping module hierarchy from parent POMs, or detecting version conflicts across a multi-module Java project.

</when_to_use>

Domain skill for querying Maven POM XML files using dasel v3. Always pass `-i xml` explicitly. Child element text content (groupId, artifactId, version, scope) is accessed by element name directly — no `#text` needed. Write intermediate batch results to `/tmp/`, never to the source tree.

## Dependency Extraction

```bash
# All dependency groupIds from a single POM
cat pom.xml | dasel -i xml 'project.dependencies.dependency.map(groupId)'
```

## Framework Version Filtering

Filter dependencies by groupId to isolate framework-specific versions.

```bash
#
```

</details>
