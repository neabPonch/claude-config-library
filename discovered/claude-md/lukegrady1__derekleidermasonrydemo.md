---
name: lukegrady1__derekleidermasonrydemo
source: https://github.com/lukegrady1/derekleidermasonrydemo/blob/5575e7e96c53a96f371655acf226e4ea75ad507b/claude.md
repo: lukegrady1/derekleidermasonrydemo
kind: claude-md
stars: 0
last_pushed: 2025-10-23T19:55:44Z
license: unknown
score: 9
domains: [web-frontend, seo]
tags: [prd, nextjs, performance-optimization]
curated: 2026-06-14
curated_by: config-scout
---

# lukegrady1/derekleidermasonrydemo — claude-md

**Why it's worth keeping:** It replaces vague goals with strict quantitative metrics (Lighthouse scores, JS budgets) and includes ready-to-use structured data/Schema.org patterns. This ensures the agent produces optimized, professional-grade code rather than generic templates.

**Summary:** A high-fidelity project specification that provides exhaustive technical, performance, and SEO constraints for a production-ready web application.

**Source credibility:** Single-author demo repository; quality of technical constraints suggests high engineering standards.

**Recency:** Highly current; utilizes modern stacks like Next.js 14 and App Router.

**Source:** [lukegrady1/derekleidermasonrydemo/claude.md](https://github.com/lukegrady1/derekleidermasonrydemo/blob/5575e7e96c53a96f371655acf226e4ea75ad507b/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
Project

Build a new, mobile-first marketing website for Derek Leider Masonry that outperforms the current site in design, speed, SEO, accessibility, and lead generation. Use the information on the existing site as factual input, but rewrite all copy in clear, professional, benefit-driven language. Do not copy text verbatim.

Tech & Delivery

Stack: Next.js 14 (App Router) + TypeScript + Tailwind CSS. No heavy UI kits; keep bundle lean.

Images: Next/Image, responsive sizes, AVIF/WebP with JPEG fallbacks; blur-up placeholders.

CMS (optional): Filesystem Markdown for FAQs & service pages; simple to edit.

Hosting: Vercel (or Netlify). Include preview env + production.

Analytics: GA4 + Google Ads (hook ready) + Meta Pixel (opt-in). Consent banner with localStorage.

Forms: Server Actions (Next) + SMTP (nodemailer) with file upload (images/PDF under 15MB), basic spam controls (honeypot + rate limit).

Telemetry: Vercel Speed Insights + Lighthouse CI GitHub Action.

Performance Targets (strict)

Lighthouse (Mobile): Performance ≥ 95, Accessibility ≥ 95, SEO ≥ 100, Best Practices ≥ 95.

Core Web Vitals: LCP ≤ 2.5s, INP ≤ 200ms, CLS ≤ 0.1 on a mid-tier phone (throttled).

Total JS < 12
```

</details>
