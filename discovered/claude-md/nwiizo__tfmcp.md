---
name: nwiizo__tfmcp
source: https://github.com/nwiizo/tfmcp/blob/db4ea8d9d774d30b6793807972e3b94effdfcd3c/CLAUDE.md
repo: nwiizo/tfmcp
kind: claude-md
stars: 368
last_pushed: 2026-03-26T07:29:30Z
license: mit
score: 9
domains: [cli-tools, rust, devops, mcp-server]
tags: [rust, terraform, mcp, strict-rules]
curated: 2026-06-14
curated_by: config-scout
---

# nwiizo/tfmcp — claude-md

**Why it's worth keeping:** The 'Key Rules' section establishes zero-tolerance guardrails (e.g., no .unwrap()) that are highly effective for LLMs, while the documentation table provides a clear map of specialized sub-rule files.

**Summary:** Provides high-density technical context including exact verification commands, structural mapping, and strict coding constraints for a Rust project.

**Source credibility:** Strong; 368 stars indicates a legitimate, widely used tool in the MCP ecosystem.

**Recency:** Highly current, utilizing modern Rust quality workflows and Claude-centric tool structures.

**Source:** [nwiizo/tfmcp/CLAUDE.md](https://github.com/nwiizo/tfmcp/blob/db4ea8d9d774d30b6793807972e3b94effdfcd3c/CLAUDE.md) · 368★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

tfmcp is a Rust-based MCP server for Terraform operations using the RMCP SDK.

## Quick Reference

```bash
# Quality checks (run before commits)
cargo fmt --all && RUSTFLAGS="-Dwarnings" cargo clippy --all-targets --all-features && cargo test --locked --all-features
```

## Project Structure

| Module | Purpose |
|--------|---------|
| `src/core/` | Main application logic |
| `src/mcp/` | RMCP-based MCP server (21 tools, 3 resources) |
| `src/terraform/` | Terraform CLI integration |
| `src/registry/` | Terraform Registry API client |

## Key Rules

- **No mocks**: Use real implementations only
- **No dead code**: Remove unused code immediately
- **No warnings**: `RUSTFLAGS="-Dwarnings"` in CI
- **No `.unwrap()`**: Use proper error handling

## Documentation

| File | Contents |
|------|----------|
| [rules/quality-commands.md](.claude/rules/quality-commands.md) | Build, test, CI commands |
| [rules/development-guidelines.md](.claude/rules/development-guidelines.md) | Code style, security rules |
| [docs/architecture.md](.claude/docs/architecture.md) | Module structure, features |
| [docs/configuration.md](.claude/docs/configuration.md) | Environment variables, Docker
```

</details>
