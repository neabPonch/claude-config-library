---
name: ryan-pip__pulumi-astronomer
source: https://github.com/ryan-pip/pulumi-astronomer/blob/045fe01cd052e5d3c285b02d7660d0b89fb03b65/claude.md
repo: ryan-pip/pulumi-astronomer
kind: claude-md
stars: 0
last_pushed: 2026-06-09T04:34:36Z
license: apache-2.0
score: 8
domains: [infrastructure-as-code, devops]
tags: [architecture-diagram, build-system, workflow-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# ryan-pip/pulumi-astronomer — claude-md

**Why it's worth keeping:** The ASCII architecture diagram explains complex data flow for the LLM, and the 'Where to look' section provides a clear map of logic distribution.

**Summary:** Provides high-density technical context including architectural diagrams, build command sets, and CI/CD workflow overviews.

**Source credibility:** High; part of a specialized infrastructure-as-code project with sophisticated automation requirements.

**Recency:** Current; references modern tooling like mise and specific bridge versions.

**Source:** [ryan-pip/pulumi-astronomer/claude.md](https://github.com/ryan-pip/pulumi-astronomer/blob/045fe01cd052e5d3c285b02d7660d0b89fb03b65/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

`pulumi-astronomer` is a [Pulumi](https://www.pulumi.com/) resource provider for [Astronomer Astro](https://www.astronomer.io/), bridged from the upstream Terraform provider [`astronomer/terraform-provider-astro`](https://github.com/astronomer/terraform-provider-astro) via [`pulumi-terraform-bridge`](https://github.com/pulumi/pulumi-terraform-bridge) v3.

## Architecture

```
upstream terraform-provider-astro (Go module)
            │
            ▼
provider/resources.go ─────► tfgen binary (bin/pulumi-tfgen-astronomer)
                                   │
                                   ▼
                       provider/cmd/pulumi-resource-astronomer/
                       ├── schema.json
                       ├── bridge-metadata.json
                       └── schema-embed.json
                                   │
              ┌────────────────────┼────────────────────┬──────────────────┐
              ▼                    ▼                    ▼                  ▼
        sdk/nodejs/           sdk/python/            sdk/go/         sdk/dotnet/
```

- [provider/](provider/) — Go module with bridge wiring ([provider/resources.go](provider/resources.go)) and two bi
```

</details>
