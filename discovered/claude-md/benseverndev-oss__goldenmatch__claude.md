---
name: benseverndev-oss__goldenmatch__claude
source: https://github.com/benseverndev-oss/goldenmatch/blob/9e72ebe4b6f839b313e5dc5fe6ed601123e378f4/packages/rust/extensions/CLAUDE.md
repo: benseverndev-oss/goldenmatch
kind: claude-md
stars: 111
last_pushed: 2026-06-15T05:54:45Z
license: mit
score: 9
domains: [systems-programming, data-engineering, database-extensions]
tags: [rust, postgres, environment-setup, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# benseverndev-oss/goldenmatch — claude-md

**Why it's worth keeping:** Uses explicit environmental 'preambles' to solve pathing issues; documents specific tool-chain gotchas like workspace exclusions due to pgrx bugs; includes strict branching and authentication SOPs.

**Summary:** Provides hyper-specific environmental configuration and architectural mapping for a multi-language (Rust/Python/SQL) extension suite. It bridges high-level project architecture with low-level shell requirements.

**Source credibility:** High-density technical documentation for a specialized, actively maintained OSS toolkit.

**Recency:** Very current (includes future-dated roadmap details).

**Source:** [benseverndev-oss/goldenmatch/packages/rust/extensions/CLAUDE.md](https://github.com/benseverndev-oss/goldenmatch/blob/9e72ebe4b6f839b313e5dc5fe6ed601123e378f4/packages/rust/extensions/CLAUDE.md) · 111★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# GoldenMatch Extensions

Native SQL extensions for [GoldenMatch](https://github.com/benseverndev-oss/goldenmatch) (`D:\show_case\goldenmatch`).

## Related Projects
- **Main repo:** `D:\show_case\goldenmatch` -- Python entity resolution toolkit (v1.1.0+). Has its own CLAUDE.md with full architecture docs.
- **This repo:** Rust bridge + Postgres extension + DuckDB Python UDFs
- **PyPI packages:** `goldenmatch` (Python), `goldenmatch-duckdb` (DuckDB UDFs)

## Branch & Merge SOP (all Golden Suite repos)
- Feature work goes on `feature/<name>` branches, never directly to main
- Merge via **squash merge PR** (watchers see PR activity, history stays clean)
- PR title format: `feat: <description>` or `fix: <description>`
- PR body: summary bullets + test plan
- Merge when: tests pass, docs updated. Days not weeks.
- After merge: delete remote branch

## Environment
- Windows 11, bash shell (Git Bash) -- use Unix paths
- Two GitHub accounts: `benzsevern` (personal, for this repo) and `benzsevern-mjh` (work)
- MUST `gh auth switch --user benzsevern` before push, switch back to `benzsevern-mjh` after
- Rust 1.94.0 at `C:\Users\bsevern\.cargo\bin` -- must set `RUSTUP_HOME="C:/Users/bsevern/.
```

</details>
