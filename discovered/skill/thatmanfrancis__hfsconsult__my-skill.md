---
name: thatmanfrancis__hfsconsult__my-skill
source: https://github.com/thatmanfrancis/hfsconsult/blob/0f2edd81dbc5ad53b899a6183d1ac0c3f7810ea2/my-skill.md
repo: thatmanfrancis/hfsconsult
kind: skill
stars: 0
last_pushed: 2026-06-02T12:28:45Z
license: unknown
score: 9
domains: [web-frontend, design-systems]
tags: [tailwind, nextjs, ui-ux, specification]
curated: 2026-06-16
curated_by: config-scout
---

# thatmanfrancis/hfsconsult — skill

**Why it's worth keeping:** Uses powerful negative constraints (prohibited classes) to prevent AI drift and provides exact JSX/Tailwind snippets for complex components like mobile menus and heading hierarchies.

**Summary:** A highly prescriptive design system specification that enforces strict visual consistency through explicit constraints and code patterns.

**Source credibility:** Low public social proof, but represents high-quality professional design documentation.

**Recency:** Very current; utilizes modern Next.js and Tailwind CSS conventions.

**Source:** [thatmanfrancis/hfsconsult/my-skill.md](https://github.com/thatmanfrancis/hfsconsult/blob/0f2edd81dbc5ad53b899a6183d1ac0c3f7810ea2/my-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 📐 Design Pattern Specification — Hausevo (Shack) & HFS Consult

> **MANDATORY**: Any AI coding assistant, chatbot, or developer working in this workspace **MUST** read and apply this specification completely before writing, modifying, or refactoring any frontend code. No exceptions.

---

## 🎯 Overview

This document defines the complete frontend design language built across two projects:
- **Hausevo** (`/projects/shack`) — verified housing platform
- **HFS Consult** (`/projects/hfsconsult`) — investment consulting firm

Both projects share the same underlying design system: flat, clean, minimal, typographically-strong, and entirely shadow-free. The aesthetic is **premium but restrained** — it communicates trust and authority without heavy decoration.

---

## 🔤 1. Typography

### Font
- **Primary Font**: `Nunito` from Google Fonts (loaded via `next/font/google`)
- **No fallback font stacks** with serif fonts. Only: `system-ui, -apple-system, sans-serif` as a fallback
- **Font setup in `layout.tsx`**:
  ```tsx
  import { Nunito } from "next/font/google";
  const nunito = Nunito({ variable: "--font-nunito", subsets: ["latin"], weight: ["300","400","500","600","700","800"] });
  ``
```

</details>
