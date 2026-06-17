---
name: crytic__slither
source: https://github.com/crytic/slither/blob/5e78b88c0235885aa0a3f0ac3124d5eace3f1c40/CLAUDE.md
repo: crytic/slither
kind: claude-md
stars: 6294
last_pushed: 2026-06-11T00:45:49Z
license: agpl-3.0
score: 10
domains: [security, cli-tools, blockchain]
tags: [ast-grep, pitfall-prevention, structural-search, domain-specific]
curated: 2026-06-15
curated_by: config-scout
---

# crytic/slither — claude-md

**Why it's worth keeping:** It teaches the agent how to navigate via AST patterns rather than just text search and provides 'anti-pattern' warnings (like the ElementaryType pitfall) that prevent common logic errors.

**Summary:** A high-density guide that combines architectural mapping, specific structural search patterns using `ast-grep`, and critical domain-specific implementation pitfalls.

**Source credibility:** High; Slither is a gold-standard, highly starred static analyzer for smart contract security.

**Recency:** Extremely current; uses modern toolchains like `uv` and reflects active development.

**Source:** [crytic/slither/CLAUDE.md](https://github.com/crytic/slither/blob/5e78b88c0235885aa0a3f0ac3124d5eace3f1c40/CLAUDE.md) · 6294★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Slither

Static analyzer for Solidity smart contracts. Detects vulnerabilities, prints contract information, and provides an intermediate representation (SlithIR) for analysis.

## Architecture

```
slither/
├── analyses/      # Data dependency, dominators, control flow
├── core/          # Core classes: SlitherCore, Contract, Function
├── detectors/     # Security checks (subclass AbstractDetector)
├── printers/      # Output formatters (subclass AbstractPrinter)
├── slithir/       # Intermediate representation for analysis
├── solc_parsing/  # Solidity AST parsing
└── tools/         # CLI tools (slither-read-storage, slither-mutate, etc.)
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed architecture and how to add detectors.

## Development

| tool    | purpose       |
|---------|---------------|
| `uv`    | deps & venv   |
| `ruff`  | lint & format |
| `prek`  | pre-commit hooks |
| `pytest`| tests         |

```bash
make dev                    # Setup dev environment + pre-commit hooks
make lint                   # Run ruff check
make reformat               # Run ruff format
make test                   # Run all tests
pytest tests/unit/ -q       # Fast unit tests only
```

</details>
