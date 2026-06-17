---
name: anomalyco__sst
source: https://github.com/anomalyco/sst/blob/4f1a634f0346794d882aa2ec23525dbfbe4f5e5f/CLAUDE.md
repo: anomalyco/sst
kind: claude-md
stars: 26075
last_pushed: 2026-06-04T12:20:18Z
license: mit
score: 8
domains: [cli-tools, infrastructure, fullstack]
tags: [architecture-map, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# anomalyco/sst — claude-md

**Why it's worth keeping:** It utilizes precise cross-referencing of source paths and provides a clear 'Verification' sequence to ensure the agent can validate its own work.

**Summary:** A high-density structural map that links multi-language components (Go/TS) via explicit file relationships.

**Source credibility:** SST is an industry-standard infrastructure tool with high star count and active maintenance.

**Recency:** Highly current; reflects modern tooling like Bun and Go.

**Source:** [anomalyco/sst/CLAUDE.md](https://github.com/anomalyco/sst/blob/4f1a634f0346794d882aa2ec23525dbfbe4f5e5f/CLAUDE.md) · 26075★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Layout

- `platform/` — TS Pulumi components embedded via `//go:embed` (`platform/platform.go:16`)
- `examples/` — sample apps
- `cmd/sst/` — Go CLI entry, orchestrates everything
- `cmd/sst/mosaic/` — live dev TUI
- `pkg/server/` — JSON-RPC bridge for custom Pulumi dynamic providers (`rpc/rpc.ts` ↔ `pkg/server`)
- `pkg/bus/` — pub/sub event bus
- `sdk/js/` — runtime SDK for reading linked resources
- `www/` — docs site (auto-generated from JSDoc comments in platform and extracted from the Go CLI)

## Commands

- **Setup**: `bun run setup`
- **Build platform**: `bun run build:platform`
- **Build CLI**: `bun run build:cli`
- **Run CLI locally**: `cd examples/<app> && go run ../../cmd/sst <command>`
- **Go tests**: `bun run test:cli`
- **Typecheck**: `bun run typecheck`
- **Generate docs**: `bun run docs:generate`
- **Run docs locally**: `bun run docs:dev`

## Verification

1. Build the platform
2. `cd examples/<app> && bun install`
3. `go run ../../cmd/sst deploy`
4. Verify with `curl` or AWS CLI
5. Don't clean up unless told to
6. `sst dev --mode=basic` for dev mode
```

</details>
