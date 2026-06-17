---
name: forcedotcom__salesforcedx-vscode__skill
source: https://github.com/forcedotcom/salesforcedx-vscode/blob/a2f075bf942d5a3785ac524ca510e2700aae73bd/.claude/skills/paths/SKILL.md
repo: forcedotcom/salesforcedx-vscode
kind: skill
stars: 1020
last_pushed: 2026-06-13T17:31:01Z
license: bsd-3-clause
score: 8
domains: [vs-code-extensions, tooling]
tags: [paths, uris, filesystem]
curated: 2026-06-15
curated_by: config-scout
---

# forcedotcom/salesforcedx-vscode — skill

**Why it's worth keeping:** It provides precise function mappings (e.g., mapping path.join to Utils.joinPath) and defines clear 'exit hatch' exceptions for when standard paths are acceptable.

**Summary:** Enforces the use of vscode-uri over node:path to ensure cross-platform and web-compatible path handling in VS Code extension development.

**Source credibility:** High; originates from an official, highly-starred Salesforce repository with active maintenance.

**Recency:** Very current; the source repository is actively maintained within the last month.

**Source:** [forcedotcom/salesforcedx-vscode/.claude/skills/paths/SKILL.md](https://github.com/forcedotcom/salesforcedx-vscode/blob/a2f075bf942d5a3785ac524ca510e2700aae73bd/.claude/skills/paths/SKILL.md) · 1020★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: paths
description: Prefer vscode-uri over node:path. Use when .ts files in /src import from node:path or use path.join, path.basename, path.dirname, path.resolve.
---

# Paths

Scope: .ts files in /src

- Prefer vscode-uri URIs over paths (file, memfs; cross-platform; FsService/workspace.fs accept URIs)
- Use `Utils` from vscode-uri instead of node:path:
  - `Utils.joinPath(baseUri, 'a', 'b')` — path.join
  - `Utils.basename(uri)`, `Utils.dirname(uri)`, `Utils.extname(uri)` — path.\*
  - `Utils.resolvePath(baseUri, 'rel')` — path.resolve
- URI↔path via FsService: `toUri(filePath)` / `uriToPath(uri)` (Effect; extensions with salesforcedx-vscode-services)
- Raw path→URI: `URI.file(path)` or `toUri` for memfs in web
- FsService setup: [services-extension-consumption](../services-extension-consumption/SKILL.md)
- Exit hatch: build scripts, esbuild configs, tests, desktop-only extension, host-FS-only tooling → node:path ok
```

</details>
