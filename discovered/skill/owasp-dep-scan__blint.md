---
name: owasp-dep-scan__blint
source: https://github.com/owasp-dep-scan/blint/blob/d74d6b83293bf3db4da1af72217ef303fb432f86/SKILL.md
repo: owasp-dep-scan/blint
kind: skill
stars: 450
last_pushed: 2026-05-25T00:38:25Z
license: mit
score: 9
domains: [cli-tools, security, binary-analysis]
tags: [architecture-mapping, testing-protocols, technical-constraints]
curated: 2026-06-14
curated_by: config-scout
---

# owasp-dep-scan/blint — skill

**Why it's worth keeping:** The template excels at mapping 'intent' (e.g., SBOM generation) to 'implementation paths' and includes highly specific technical caveats like architecture-specific regressions and rule stability requirements. The inclusion of mode-specific testing protocols is a top-tier technique for minimizing regression.

**Summary:** This file provides a sophisticated architectural map that connects project capabilities to specific files and logic flows. It translates high-level intent into actionable constraints for an agent.

**Source credibility:** High; OWASP-backed project with active maintenance and clear structural ownership.

**Recency:** Current; provides detailed, actionable instructions suitable for modern agentic workflows.

**Source:** [owasp-dep-scan/blint/SKILL.md](https://github.com/owasp-dep-scan/blint/blob/d74d6b83293bf3db4da1af72217ef303fb432f86/SKILL.md) · 450★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SKILL.md

This file defines practical skills an AI agent should apply when working on `blint`.

## Skill: Navigate blint architecture quickly

- Start at `blint/cli.py` to identify mode (`default`, `sbom`, `db`).
- Follow orchestration in `blint/lib/runners.py`.
- Review coordination lives in `blint/lib/review_runner.py`.
- For extraction logic, use `blint/lib/binary.py` and `blint/lib/android.py`.
- For rule behavior, use `blint/lib/analysis.py`, `blint/lib/review_utils.py`, `blint/lib/function_reviews.py`, and `blint/data/annotations/*.yml`.
- For SBOM behavior, use `blint/lib/sbom.py` and `blint/cyclonedx/spec.py`.

## Skill: Implement rule-driven behavior safely

- Understand rule types:
  - `rules.yml` -> hardening checks (`run_checks`).
  - annotations -> reviews (`METHOD_REVIEWS`, `SYMBOL_REVIEWS`, etc.).
  - `FUNCTION_REVIEWS` -> disassembly-derived behavior checks implemented in `blint/lib/function_reviews.py`.
- Keep rule IDs stable and unique.
- Match field paths used in `function_metric` with actual metadata shape.
- Respect evidence limits (`EVIDENCE_LIMIT`) to avoid noisy output.

## Skill: Work with binary metadata extraction

- Preserve format-specific fields whil
```

</details>
