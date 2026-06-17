---
name: tmforum-oda__oda-canvas__skill
source: https://github.com/tmforum-oda/oda-canvas/blob/23e0b1198414f590ba41ca6c60fe8c163429eaf1/skills/helm-chart-development/SKILL.md
repo: tmforum-oda/oda-canvas
kind: skill
stars: 51
last_pushed: 2026-06-14T18:42:45Z
license: apache-2.0
score: 9
domains: [devops, kubernetes]
tags: [helm, k8s-architecture, infrastructure]
curated: 2026-06-15
curated_by: config-scout
---

# tmforum-oda/oda-canvas — skill

**Why it's worth keeping:** The pattern of using a prerelease suffix to toggle image pull policies between development and production is a highly practical, transferable technique.

**Summary:** Establishes strict architectural patterns for umbrella Helm charts, including sub-chart dependency management and standardized template helpers.

**Source credibility:** High; part of the TM Forum ODA Canvas project with active maintenance.

**Recency:** Current; utilizes modern Helm v2 patterns and Kubernetes best practices.

**Source:** [tmforum-oda/oda-canvas/skills/helm-chart-development/SKILL.md](https://github.com/tmforum-oda/oda-canvas/blob/23e0b1198414f590ba41ca6c60fe8c163429eaf1/skills/helm-chart-development/SKILL.md) · 51★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: helm-chart-development
description: Guide for developing Helm charts in the ODA Canvas project. Covers umbrella chart architecture, sub-chart conventions, _helpers.tpl patterns, values.yaml structure, RBAC templates, Docker image construction, versioning with prerelease suffixes, and dependency management. Use this skill when creating or modifying Helm charts.
---

# Helm Chart Development — Skill Instructions

## Architecture

The ODA Canvas uses an **umbrella chart** pattern:

- `charts/canvas-oda/` — Main umbrella chart, aggregates all sub-charts
- `charts/<sub-chart>/` — Individual operator/service charts

Sub-charts are referenced as local dependencies in the umbrella `Chart.yaml`.

## Chart.yaml Conventions

```yaml
apiVersion: v2
name: <chart-name>
description: <one-line description>
type: application
version: <semver>           # e.g., 1.2.5 or 1.2.5-LT5 (prerelease)
appVersion: "v1"            # tracks CRD spec version
```

- **Version changelog**: Maintain as comments in `Chart.yaml` — each version with date and description
- **Prerelease suffix**: Author initials (e.g., `-LT5`, `-JS3`). Clear for releases.

## Dependency Management

### Local Sub-Chart Dependen
```

</details>
