---
name: donaldgifford__forge-registry__claude-tmpl
source: https://github.com/donaldgifford/forge-registry/blob/12267f10ad78173587a6bab0b0911b975cfec4ad/homelab/charts/CLAUDE.md.tmpl
repo: donaldgifford/forge-registry
kind: claude-md
stars: 0
last_pushed: 2026-06-01T02:34:07Z
license: apache-2.0
score: 8
domains: [devops, infrastructure-as-code]
tags: [helm, oci, ci-cd, k8s]
curated: 2026-06-16
curated_by: config-scout
---

# donaldgifford/forge-registry — claude-md

**Why it's worth keeping:** Includes critical operational specifics like exact environment loading methods via 1Password, task runner usage, and strict rules for appVersion vs version bumps to ensure CI/CD compliance.

**Summary:** Defines toolchain requirements, versioning conventions, and OCI-based publishing workflows for a Helm chart registry.

**Source credibility:** Low social proof (0 stars), but reflects a sophisticated personal DevOps infrastructure.

**Recency:** Current; utilizes modern tooling such as mise, just, and OCI-native workflows.

**Source:** [donaldgifford/forge-registry/homelab/charts/CLAUDE.md.tmpl](https://github.com/donaldgifford/forge-registry/blob/12267f10ad78173587a6bab0b0911b975cfec4ad/homelab/charts/CLAUDE.md.tmpl) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Per-repo orientation for `${project_org}/${project_name}` — Helm charts
published as OCI artifacts to Harbor and Forgejo Packages.

## Homelab universals

- **Toolchain pinned via `mise.toml`**; task runner `just`.
- **`.env` is a [1Password Developer Environment](https://developer.1password.com/docs/environments/local-env-file)** file. `op run --env-file=.env -- <cmd>`. Never `source .env`.
- **`docz create <type> "Title"`** for new docs.
- **`grep` is `rg`** — drop `-E`.

## Repo layout

```
charts/<chart-name>/
  Chart.yaml
  values.yaml
  templates/
  README.md            # generated via helm-docs
  README.md.gotmpl     # helm-docs template
  ci/                  # ct lint test values (optional)
```

## Conventions

- **One chart per directory** under `charts/`.
- **Chart.yaml `appVersion` + `version` are independent**. Bump
  `appVersion` when the upstream image bumps; bump `version` when the
  chart shape (templates / defaults / required values) changes.
- **Image pinning + Renovate**: pin the image tag in `values.yaml` with
  `# renovate: image=<repo>` one line above. Renovate's `appVersion`
  manager also fires off `Chart.yaml` — see homelab universal renovate
```

</details>
