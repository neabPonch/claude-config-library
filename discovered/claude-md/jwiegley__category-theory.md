---
name: jwiegley__category-theory
source: https://github.com/jwiegley/category-theory/blob/e4f9c6c4db80ed1c93ac52a27233ae45b022fbcb/CLAUDE.md
repo: jwiegley/category-theory
kind: claude-md
stars: 802
last_pushed: 2026-05-19T18:28:45Z
license: bsd-3-clause
score: 10
domains: [formal-verification, mathematics, type-theory]
tags: [coq, rocq, category-theory, formal-methods]
curated: 2026-06-15
curated_by: config-scout
---

# jwiegley/category-theory — claude-md

**Why it's worth keeping:** Includes 'Critical Design Patterns' to prevent common errors like using strict equality instead of equivalence. The 'Proof Automation' section gives Claude explicit tactical patterns to follow when generating proofs.

**Summary:** Provides a deep technical blueprint for formalizing category theory in Coq/Rocq. It bridges high-level mathematical architecture with specific implementation tactics and design constraints.

**Source credibility:** High; the repo is a significant, well-maintained formalization project with high community interest (802 stars).

**Recency:** Extremely current; it explicitly mentions Rocq, reflecting the most recent renaming and evolution of the Coq ecosystem.

**Source:** [jwiegley/category-theory/CLAUDE.md](https://github.com/jwiegley/category-theory/blob/e4f9c6c4db80ed1c93ac52a27233ae45b022fbcb/CLAUDE.md) · 802★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This codebase is a comprehensive formalization of category theory in Coq/Rocq. It contains 1,603 proof files with 225,209 lines implementing core categorical concepts with zero axioms in the core theory.

## Commands

### Building the Library

```bash
# Build the entire library (default: Rocq 9.1)
make

# Build for specific version (if using Nix)
nix-shell -p coqPackages_9_1.coq --run make

# Build using Nix flake
nix build .#category-theory

# Clean build artifacts
make clean
make fullclean  # removes Makefile.coq as well

# Install library
make install

# Check for admitted proofs or TODOs
make todo
```

### Single File Development

```bash
# Compile a single file
coqc -R . Category Theory/Category.v

# Interactive development (in coqide/vscoq)
# Ensure _CoqProject is loaded with: -R . Category
```

### Proof Development Patterns

The library uses custom tactics in `Lib/Tactics.v`:
- `cat` - standard simplification for category proofs
- `cat_simpl` - more aggressive simplification with program obligations
- `proper` - for proving morphism respectfulness
- `equivalence` - for proving equivalence relations

## Architecture

### Core Abstraction Hierarchy

The library i
```

</details>
