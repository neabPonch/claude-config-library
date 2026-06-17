---
name: jhobbs__mathnotes
source: https://github.com/jhobbs/mathnotes/blob/970f5269cf63df3c20c6055a5d12413f781a0a04/CLAUDE.md
repo: jhobbs/mathnotes
kind: claude-md
stars: 1
last_pushed: 2026-06-15T01:36:42Z
license: unknown
score: 9
domains: [web-frontend, static-site-generator, devops]
tags: [ssg, typescript, docker, mathjax]
curated: 2026-06-16
curated_by: config-scout
---

# jhobbs/mathnotes — claude-md

**Why it's worth keeping:** It provides critical 'under the hood' logic (math processing phases) to prevent errors and specific troubleshooting workflows for containerized build failures.

**Summary:** A highly detailed instruction set for a custom math-focused static site generator that covers complex build pipelines and demo integration.

**Source credibility:** Low star count, but reflects a highly structured personal toolset with sophisticated requirements.

**Recency:** Current; explicitly mentions Claude Code capabilities/workflows.

**Source:** [jhobbs/mathnotes/CLAUDE.md](https://github.com/jhobbs/mathnotes/blob/970f5269cf63df3c20c6055a5d12413f781a0a04/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

Mathnotes is a static site generator that renders mathematics notes with interactive demonstrations into static HTML files served by nginx. The application features:
- Structured mathematical content with semantic markup (theorems, proofs, definitions)
- TypeScript interactive demos using p5.js for 2D/WebGL graphics and Plotly.js for 3D scientific visualizations
- Wiki-style cross-references using `[[slug]]` syntax
- Dark mode support with automatic detection
- Comprehensive security headers with Content Security Policy
- Modern CSS system with PostCSS, CSS custom properties, and hot module replacement

## Security and Best Practices

**Demo Crawler Guidelines**:
* do not every read the screenshots from the demo crawler directly, only use --ask
* Hey - you're not supposed to look at screenshots yourself. Only use --ask to do that.

## Development Guidelines

### Coding Best Practices

* Don't check types after every single change
* For styling guidelines, see [STYLE.md](./STYLE.md)
* we never put styles directly in typescript
* You don't need
```

</details>
