---
name: BeaconCMS__beacon
source: https://github.com/BeaconCMS/beacon/blob/79083779aa1d5601e05ae038fda95da8f91b6d0b/CLAUDE.md
repo: BeaconCMS/beacon
kind: claude-md
stars: 1242
last_pushed: 2026-05-12T16:50:46Z
license: mit
score: 9
domains: [ai-agents, cli-tools, devops]
tags: [orchestration, batching, delegation, engineering-standards]
curated: 2026-06-15
curated_by: config-scout
---

# BeaconCMS/beacon — claude-md

**Why it's worth keeping:** The 'Batching Rules' for reducing LLM round-trips and the formal 'Truth Hierarchy/Delegation' patterns are elite examples of how to guide an agent through complex tasks.

**Summary:** Combines rigorous engineering standards with advanced AI orchestration instructions for tool usage, batching, and sub-agent delegation.

**Source credibility:** High; demonstrates sophisticated internal tool integration and advanced prompt engineering logic.

**Recency:** Current; incorporates modern patterns like MCP tools and structured sub-agent handoffs.

**Source:** [BeaconCMS/beacon/CLAUDE.md](https://github.com/BeaconCMS/beacon/blob/79083779aa1d5601e05ae038fda95da8f91b6d0b/CLAUDE.md) · 1242★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Development Workflow

*NEVER* change old migrations that are already in git history.
*ALWAYS* run the entire test suite before declaring any work is complete.
*ALWAYS* TDD: write failing tests first, implement minimum code to pass, run `mix test` locally, push only when green.

**No fallbacks.** When refactoring, fully commit to the new approach. Remove old code entirely. If the new approach fails, that's a bug to surface, not hide.
j
## Release Process

When the user says "release" (or similar), follow this procedure:

### 1. Determine the version

- If the user specifies a version, use it.
- *MUST* read the current version from `build.zig.zon` first and treat that source-code version as the canonical baseline for the next release. Do not derive the baseline version from git tags, commit messages, or GitHub releases when they disagree with the source tree.
- Do not bump to a new major version while the project is still on `0.x` unless the user explicitly instructs you to start a `1.x` (or higher) release. When the project is still on `0.x`, default to the appropriate `0.x` bump even if the changes would normally look "major" under full SemVer.
- Otherwise, analyze the unrelease
```

</details>
