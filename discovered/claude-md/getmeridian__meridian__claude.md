---
name: getmeridian__meridian__claude
source: https://github.com/getmeridian/meridian/blob/4b868fbacfd38a240304d9b928489af91646cbde/src/meridian/templates/pwa/CLAUDE.md
repo: getmeridian/meridian
kind: claude-md
stars: 459
last_pushed: 2026-06-14T06:45:54Z
license: mit
score: 8
domains: [web-frontend, security, pwa]
tags: [architecture, pitfalls, design-decisions]
curated: 2026-06-15
curated_by: config-scout
---

# getmeridian/meridian — claude-md

**Why it's worth keeping:** The 'Pitfalls' section provides high-value guardrails that prevent the agent from re-introducing specific CSS, service worker, and pathing errors.

**Summary:** Technical documentation of a security-focused PWA architecture, detailing design decisions and runtime configurations.

**Source credibility:** High; comes from a well-starred (450+) active repository for censorship-resistant proxy services.

**Recency:** Current; addresses modern PWA requirements like Service Worker scopes and mobile wake locks.

**Source:** [getmeridian/meridian/src/meridian/templates/pwa/CLAUDE.md](https://github.com/getmeridian/meridian/blob/4b868fbacfd38a240304d9b928489af91646cbde/src/meridian/templates/pwa/CLAUDE.md) · 459★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PWA Connection Page

Server-hosted Progressive Web App. The old `connection-info.html.j2` is kept for local-save pages only.

## Design decisions

**Vanilla ES5, no build step** — zero external dependencies, no CDN requests. Target users live in censored regions where external resources are blocked. The whole app is ~1000 lines in an IIFE.

**Runtime config** — `config.json` fetched at load, not baked into HTML. Enables server-side credential rotation without redeploying pages.

**Shared/per-client split** — static assets (`app.js`, `styles.css`, `sw.js`, `icon.svg`) deployed once to `/pwa/`. Per-client files (`index.html`, `config.json`, `manifest.webmanifest`, `sub.txt`) in `/{uuid}/`. Saves bandwidth, enables independent updates.

**Security model** — all user/config data goes through `escapeHtml()` (uses `textContent` via dummy div). QR base64 validated with `/^[A-Za-z0-9+/=]+$/` before `<img src>` injection. iOS deep links stored in `data-` attributes, never inline JS strings.

**i18n** — English is the HTML default, NOT a translation dict. Non-EN languages swap via `data-t` attributes. Switching back to EN requires full `renderPage()` re-render.

**Subscription QR hero layo
```

</details>
