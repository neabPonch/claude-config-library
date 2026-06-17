---
name: LottieFiles__dotlottie-web
source: https://github.com/LottieFiles/dotlottie-web/blob/6795b9017ef09620c51c1a86a2900e84aad7ad61/SKILL.md
repo: LottieFiles/dotlottie-web
kind: skill
stars: 791
last_pushed: 2026-06-12T20:29:38Z
license: mit
score: 9
domains: [web-frontend, performance-optimization]
tags: [lottie, animation, react, canvas, web-workers]
curated: 2026-06-15
curated_by: config-scout
---

# LottieFiles/dotlottie-web — skill

**Why it's worth keeping:** It includes specific decision-making logic (e.g., when to use Web Workers) and provides deep patterns for complex features like state machines, theming slots, and segment control that generic docs often omit.

**Summary:** A high-quality technical implementation guide for using dotLottie animations in web projects via vanilla JS or React.

**Source credibility:** High; official documentation from LottieFiles with recent maintenance activity.

**Recency:** Current; includes modern performance optimizations and the dotLottie 2.0 spec.

**Source:** [LottieFiles/dotlottie-web/SKILL.md](https://github.com/LottieFiles/dotlottie-web/blob/6795b9017ef09620c51c1a86a2900e84aad7ad61/SKILL.md) · 791★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dotlottie-web
description: >-
  Implement Lottie animations using dotLottie runtimes (@lottiefiles/dotlottie-web
  and @lottiefiles/dotlottie-react). Use when building, debugging, or optimizing
  dotLottie or Lottie animations in web projects, including vanilla JS, React,
  and Next.js. Covers package selection, Web Workers, state machines, theming,
  dynamic slot overriding, performance best practices, and common patterns.
license: MIT
metadata:
  author: lottiefiles
  version: "1.0.0"
  source: "https://github.com/LottieFiles/dotlottie-web"
---

# dotLottie Implementation Guidelines

You are an expert at implementing Lottie animations using dotLottie runtimes. Follow these guidelines when working with dotLottie in web projects.

## Package Selection

### Use `@lottiefiles/dotlottie-web` when:

* You need direct canvas control
* Building framework-agnostic code
* Maximum performance is critical
* You want the smallest bundle

### Use `@lottiefiles/dotlottie-react` when:

* Building React applications
* You want declarative component API
* You need React lifecycle integration

## Installation

```bash
# Web (vanilla JS, Vue, Svelte, etc.)
npm install @lottiefiles/dotlotti
```

</details>
