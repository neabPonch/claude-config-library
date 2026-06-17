---
name: eunomia-bpf__eunomia.dev
source: https://github.com/eunomia-bpf/eunomia.dev/blob/3b8626b1f7836dedfe295fe79070b170ba347e3f/CLAUDE.md
repo: eunomia-bpf/eunomia.dev
kind: claude-md
stars: 219
last_pushed: 2026-06-15T02:30:38Z
license: mit
score: 9
domains: [web-frontend, documentation, content-management]
tags: [style-guide, nextjs, architecture-rules, content-pipeline]
curated: 2026-06-16
curated_by: config-scout
---

# eunomia-bpf/eunomia.dev — claude-md

**Why it's worth keeping:** The 'Blog Writing Style Guide' uses specific negative constraints (e.g., no em dashes) that are highly effective for AI; the architectural warnings prevent breaking site structure during edits.

**Summary:** Defines a complex hybrid build pipeline between Next.js and MkDocs while providing an incredibly detailed, constraint-based prose style guide.

**Source credibility:** High-quality eBPF project with active maintenance and significant stars.

**Recency:** Very current, referencing modern stacks like React 19 and Node 22.

**Source:** [eunomia-bpf/eunomia.dev/CLAUDE.md](https://github.com/eunomia-bpf/eunomia.dev/blob/3b8626b1f7836dedfe295fe79070b170ba347e3f/CLAUDE.md) · 219★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the source code for the eunomia-bpf project website (https://eunomia.dev). The site provides comprehensive tutorials and documentation for eBPF programming, the eunomia-bpf framework, bpftime, and related projects.

### Tech stack (current)

The site is rendered by a **custom Next.js + React + Tailwind CSS frontend** living in `app/`, statically exported to plain HTML/CSS/JS. It is **not** a runtime MkDocs site anymore.

- **Next.js** (pages router under `app/pages/`, `output: "export"` static export) — note the directory is named `app/` but uses the *pages* router, not the App Router
- **React 19** + **TypeScript** for components in `app/components/` and content/loader logic in `app/lib/`
- **Tailwind CSS** (`app/tailwind.config.ts`) for styling
- Content is still authored as **Markdown in `docs/**`**; a build-time pipeline (`app/scripts/generate-*`) parses it into JSON artifacts (content index, search index, manifest, static metadata) that the Next.js pages consume.
- **`mkdocs.yaml` is retained as the site IA / navigation configuration
```

</details>
