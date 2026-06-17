---
name: GPTomics__bioSkills__skill
source: https://github.com/GPTomics/bioSkills/blob/431e695cc806e1e123f8689f3be600ae8626a912/clinical-databases/myvariant-queries/SKILL.md
repo: GPTomics/bioSkills
kind: skill
stars: 902
last_pushed: 2026-06-15T01:16:57Z
license: mit
score: 9
domains: [bioinformatics, data-science, api-integration]
tags: [genomics, variant-annotation, api-documentation]
curated: 2026-06-15
curated_by: config-scout
---

# GPTomics/bioSkills — skill

**Why it's worth keeping:** Includes exact field lists (CLINICAL_FIELDS), a decision tree for query scenarios, and a critical protocol for scientific reproducibility using the _meta versioning field.

**Summary:** Provides highly specific, high-density technical specifications for querying the myvariant.info bioinformatics aggregator.

**Source credibility:** High; 902 stars indicates significant community validation in the bioinformatics domain.

**Recency:** Very current; references 2024/2025 data updates like AlphaMissense and gnomAD v4.

**Source:** [GPTomics/bioSkills/clinical-databases/myvariant-queries/SKILL.md](https://github.com/GPTomics/bioSkills/blob/431e695cc806e1e123f8689f3be600ae8626a912/clinical-databases/myvariant-queries/SKILL.md) · 902★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bio-clinical-databases-myvariant-queries
description: Queries myvariant.info BioThings aggregator for ClinVar, gnomAD, dbSNP, dbNSFP, COSMIC, CADD, and CIViC annotations in batched, version-tracked requests. Use when annotating variant lists from multiple databases simultaneously without managing per-source APIs, and when reproducibility-grade analyses require recording source data versions via _meta.
tool_type: python
primary_tool: myvariant
---

## Version Compatibility

Reference examples tested with: myvariant 1.0.0+, requests 2.31+, pandas 2.2+. myvariant.info aggregates >=21 sources; the operative version of each source is queryable via the `_meta` field and the `/v1/metadata` endpoint.

Before using code patterns, verify installed versions match. If versions differ:
- Python: `pip show <package>` then `help(module.function)` to check signatures

If code throws ImportError, AttributeError, or TypeError, introspect the installed package and adapt the example to match the actual API rather than retrying. dbNSFP version drift is the dominant staleness vector: AlphaMissense was added to dbNSFP v4.4 (~2024); querying `dbnsfp.alphamissense.score` returns whatever version
```

</details>
