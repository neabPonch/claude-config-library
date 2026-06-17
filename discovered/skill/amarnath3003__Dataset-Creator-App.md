---
name: amarnath3003__Dataset-Creator-App
source: https://github.com/amarnath3003/Dataset-Creator-App/blob/25cddecbc1ecc0de08709d51676b736eb2bece4d/skill.md
repo: amarnath3003/Dataset-Creator-App
kind: skill
stars: 4
last_pushed: 2026-04-25T06:53:36Z
license: unknown
score: 8
domains: [web-frontend, ui-design-systems]
tags: [skeuomorphism, tailwind-css, dark-mode, ui-kit]
curated: 2026-06-14
curated_by: config-scout
---

# amarnath3003/Dataset-Creator-App — skill

**Why it's worth keeping:** The explicit definition of 'shadow physics' variables (e.g., --sh-press, --sh-trough) allows an agent to create highly tactile, professional UI components consistently. It moves beyond basic utility classes into structured design system patterns.

**Summary:** Provides a comprehensive design system for a dark, skeuomorphic 'hardware console' aesthetic. It includes specific shadow physics, color palettes, and component patterns for React/Tailwind projects.

**Source credibility:** High quality documentation despite a smaller repository footprint.

**Recency:** Very recent and perfectly aligned with modern Tailwind/React workflows.

**Source:** [amarnath3003/Dataset-Creator-App/skill.md](https://github.com/amarnath3003/Dataset-Creator-App/blob/25cddecbc1ecc0de08709d51676b736eb2bece4d/skill.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Dataset Lab UI Kit - Replication Skill

This document contains everything needed to replicate the **Dark Skeuomorphic / "Control Console"** design system used in the Dataset-Creator-App. 

## 1. Core Concept & Theme
- **Style:** Neumorphic / Skeuomorphic Hardware Console.
- **Lighting:** Constant top-left (↖) light source, creating true-black drop shadows and highlights.
- **Vibe:** Physical hardware, glowing LED indicators, deep terminal screens.
- **Stack:** Tailwind CSS + Vanilla CSS Variables + React.

## 2. Tailwind Configuration
Add these extensions to your `tailwind.config.js`:

```javascript
/** @type {import('tailwindcss').Config} */
export default {
    content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
    theme: {
        extend: {
            colors: {
                neu: {
                    base: '#212529',
                    dark: '#1a1d21',
                    text: '#e0e0e0',
                    dim: '#8a8f98',
                    accent: '#ff6b00',  /* Warm Orange */
                    warning: '#ffb300'
                }
            },
            borderRadius: {
                'xl': '20px',
                '2xl': '30px'
            }
        },
```

</details>
