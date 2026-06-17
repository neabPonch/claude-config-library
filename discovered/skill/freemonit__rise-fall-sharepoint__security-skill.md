---
name: freemonit__rise-fall-sharepoint__security-skill
source: https://github.com/freemonit/rise-fall-sharepoint/blob/63b0ccc6b949e86aa6b7d5923cc9dc79662408a7/skills/security-skill.md
repo: freemonit/rise-fall-sharepoint
kind: skill
stars: 0
last_pushed: 2026-05-01T03:08:39Z
license: unknown
score: 9
domains: [security, devops, ci-cd, containerization]
tags: [SLSA, SBOM, Hardening, SupplyChain]
curated: 2026-06-16
curated_by: config-scout
---

# freemonit/rise-fall-sharepoint — skill

**Why it's worth keeping:** It provides highly specific, actionable CLI commands for SBOM generation, vulnerability scanning (Trivy/Snyk), and cryptographic signing via Cosign.

**Summary:** This file establishes a rigorous SLSA Level 3 security standard for software supply chains and containerized deployments.

**Source credibility:** Low social proof on GitHub, but the technical depth suggests professional DevOps/SecOps engineering expertise.

**Recency:** Highly current, utilizing modern industry standards like digest pinning, Sigstore/Cosign, and CycloneDX SBOMs.

**Source:** [freemonit/rise-fall-sharepoint/skills/security-skill.md](https://github.com/freemonit/rise-fall-sharepoint/blob/63b0ccc6b949e86aa6b7d5923cc9dc79662408a7/skills/security-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# security.skill.md
## Software Supply Chain & Security Standards

---

## 1. Core Principle

Security is not a scan step—it is a property of the system.

Every artifact we produce must be:

- **Traceable** → tied to source, commit, and pipeline
- **Verifiable** → cryptographically signed
- **Inspectable** → includes SBOM + scan results
- **Reproducible** → built deterministically in CI
- **Minimal** → ships only what runs — no source, no dev deps, no scripts

If we cannot prove where it came from, how it was built, and what it contains, we do not ship it.

---

## 2. SLSA Level 3 Target (Operationalized)

### 2.1 Build Environment

- All builds occur in CI only (Azure Pipelines / GitHub Actions)
- No local builds for release artifacts
- Ephemeral runners only — no persistent build agents
- Build steps defined entirely in code (YAML) — no manual portal config
- Build environment must be isolated — no network access during compilation

### 2.2 Source Integrity

- All code must originate from version control (Git)
- Protected branches (`main`, `release/*`)
- PR review required — no direct commits to production branches
- Signed commits preferred (`git config commit.gpgsign true`)
- B
```

</details>
