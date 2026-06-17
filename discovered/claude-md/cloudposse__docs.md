---
name: cloudposse__docs
source: https://github.com/cloudposse/docs/blob/cd0fbe565e594da6c0813567c4763376eed56331/CLAUDE.md
repo: cloudposse/docs
kind: claude-md
stars: 97
last_pushed: 2026-05-21T21:22:43Z
license: other
score: 9
domains: [docs-as-code, devops, static-site-generation]
tags: [docusaurus, mdx, infrastructure]
curated: 2026-06-15
curated_by: config-scout
---

# cloudposse/docs — claude-md

**Why it's worth keeping:** Includes high-stakes 'Critical' instructions regarding redirects to prevent deployment failures and demonstrates a mature 'Skills' architecture via specialized sub-modules.

**Summary:** Provides rigorous protocols for documentation maintenance, specifically targeting link integrity and URL resolution patterns in Docusaurus/MDX environments.

**Source credibility:** High; Cloud Posse is an established Terraform/AWS engineering firm with highly structured documentation standards.

**Recency:** Very current, updated within the last month.

**Source:** [cloudposse/docs/CLAUDE.md](https://github.com/cloudposse/docs/blob/cd0fbe565e594da6c0813567c4763376eed56331/CLAUDE.md) · 97★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Cloud Posse Reference Architecture Documentation

Public documentation site published to [docs.cloudposse.com](https://docs.cloudposse.com). Built with Docusaurus.

## Content Sources

**Important:** This repo is NOT always the source of truth. Content flows from multiple sources:

| Content Type | Source of Truth | Location in This Repo |
|--------------|----------------|----------------------|
| Atmos workflows (YAML) | `refarch-scaffold/` | `examples/snippets/stacks/workflows/` |
| GitHub Action workflows | `refarch-scaffold/` | `examples/snippets/.github/workflows/` |
| Other snippets (Dockerfile, Makefile) | `refarch-scaffold/` | `examples/snippets/` |
| Component docs | `cloudposse-terraform-components/` | `docs/components/library/` (auto-generated) |
| Module docs | `cloudposse/terraform-aws-*` repos | `docs/modules/library/` (auto-generated) |
| GitHub Actions docs | `cloudposse/github-action-*` repos | `docs/github-actions/library/` (auto-generated) |
| Layer guides, tutorials | **This repo** | `docs/` |

Before editing snippets or workflows in `examples/`, verify changes should be made in `refarch-scaffold/` first.

## Quick Reference

### Development

```bash
npm insta
```

</details>
