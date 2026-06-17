---
name: UI5__webcomponents__skill
source: https://github.com/UI5/webcomponents/blob/b41f99e0c4c56b3869d2abc3ab698cde3baebb22/skills/accessibility/SKILL.md
repo: UI5/webcomponents
kind: skill
stars: 1754
last_pushed: 2026-06-15T00:55:52Z
license: apache-2.0
score: 9
domains: [web-frontend, accessibility]
tags: [ui5, sap, aria, shadow-dom]
curated: 2026-06-15
curated_by: config-scout
---

# UI5/webcomponents — skill

**Why it's worth keeping:** It provides exact mappings for proprietary properties like accessibleNameRef that bypass standard HTML/ARIA constraints within web components.

**Summary:** A technical reference for implementing accessibility in UI5 Web Components, specifically addressing Shadow DOM limitations.

**Source credibility:** High; official documentation from the highly-starred SAP UI5 repository.

**Recency:** Current; aligns with modern web component and accessibility standards.

**Source:** [UI5/webcomponents/skills/accessibility/SKILL.md](https://github.com/UI5/webcomponents/blob/b41f99e0c4c56b3869d2abc3ab698cde3baebb22/skills/accessibility/SKILL.md) · 1754★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: accessibility
description: How to make UI5 Web Components applications accessible. Covers accessibility APIs (accessibleName, accessibleNameRef, accessibleDescription, accessibleRole, accessibilityAttributes), label-input relationships, invisible messaging, keyboard handling, high contrast themes, and screen reader support. Use when the user asks about ARIA attributes, screen readers, keyboard navigation, accessibility properties, or making their app accessible.
user-invocable: false
---

# Accessibility in UI5 Web Components

UI5 Web Components have built-in accessibility: ARIA roles, keyboard navigation, screen reader support, and high contrast themes are handled automatically in the shadow DOM. Applications should use the accessibility APIs described here to provide additional context that only the app can know (labels, descriptions, relationships).

## Built-in Accessibility (No App Code Needed)

Components automatically provide:
- **ARIA roles and attributes** mapped in the shadow DOM (e.g., `ui5-combobox` renders `role="combobox"` internally)
- **Keyboard navigation** within complex components (arrow keys in lists, tables, date pickers, etc.)
- **Focus management**
```

</details>
