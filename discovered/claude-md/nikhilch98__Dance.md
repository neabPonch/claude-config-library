---
name: nikhilch98__Dance
source: https://github.com/nikhilch98/Dance/blob/81368fa412bf904002e3897b1a2313a2a9d0ee6a/CLAUDE.md
repo: nikhilch98/Dance
kind: claude-md
stars: 1
last_pushed: 2026-01-25T18:21:19Z
license: unknown
score: 9
domains: [mobile-app, flutter, ui-ux]
tags: [design-system, flutter, ui-patterns, responsive-design]
curated: 2026-06-16
curated_by: config-scout
---

# nikhilch98/Dance — claude-md

**Why it's worth keeping:** The 'Overflow Prevention' patterns are exceptional for preventing UI breakage with dynamic data, and the exact code snippets for glassmorphism ensure visual consistency.

**Summary:** This file acts as both a design system and a coding standard specifically tailored for a Flutter mobile application.

**Source credibility:** Low star count, but the highly specific design tokens and component rules suggest it is a hand-crafted developer asset.

**Recency:** 5 months old; remains highly relevant for modern Flutter development workflows.

**Source:** [nikhilch98/Dance/CLAUDE.md](https://github.com/nikhilch98/Dance/blob/81368fa412bf904002e3897b1a2313a2a9d0ee6a/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# Nachna App - Design Language & Development Rules

## Design Language Guidelines

### Color Palette
- **Primary Gradient**: `LinearGradient(colors: [Color(0xFF00D4FF), Color(0xFF9C27B0)])`
- **Background Gradient**: 
  ```dart
  LinearGradient(
    begin: Alignment.topLeft,
    end: Alignment.bottomRight,
    colors: [
      Color(0xFF0A0A0F),
      Color(0xFF1A1A2E),
      Color(0xFF16213E),
      Color(0xFF0F3460),
    ],
  )
  ```
- **Accent Colors**:
  - Blue: `Color(0xFF3B82F6)` to `Color(0xFF1D4ED8)`
  - Green: `Color(0xFF10B981)` to `Color(0xFF059669)`
  - Purple: `Color(0xFF8B5CF6)`
  - Pink/Red: `Color(0xFFFF006E)` to `Color(0xFFDC2626)`
- **Text Colors**:
  - Primary: `Colors.white`
  - Secondary: `Colors.white.withOpacity(0.7)`
  - Tertiary: `Colors.white.withOpacity(0.5)`

### Typography
- **Headers**: Bold, white text with appropriate sizing
- **Body Text**: Regular weight, white or white with opacity
- **Font Sizes**: Use responsive sizing based on screen width/height percentages
- **Letter Spacing**: Use `letterSpacing: 1.2` for headers

### Overflow
```

</details>
