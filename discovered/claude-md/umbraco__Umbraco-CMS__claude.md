---
name: umbraco__Umbraco-CMS__claude
source: https://github.com/umbraco/Umbraco-CMS/blob/3ee7b142b3c7cbb1fb3ef3520d27d2d8e5308e96/src/Umbraco.Web.UI.Client/src/packages/tiptap/CLAUDE.md
repo: umbraco/Umbraco-CMS
kind: claude-md
stars: 5201
last_pushed: 2026-06-15T09:14:14Z
license: mit
score: 9
domains: [web-frontend, typescript, ui-framework]
tags: [architecture-patterns, extension-api, implementation-recipes]
curated: 2026-06-15
curated_by: config-scout
---

# umbraco/Umbraco-CMS — claude-md

**Why it's worth keeping:** It provides concrete code templates/base classes and explains the 'why' behind complex architectural decisions (like the indirection/bundling strategy), which is crucial for AI to understand intent.

**Summary:** Defines the architectural patterns, file naming conventions, and implementation recipes for the Tiptap extension system.

**Source credibility:** High; part of a major, highly-starred open-source CMS project.

**Recency:** Modern; uses current TypeScript and ESM patterns relevant to today's development environments.

**Source:** [umbraco/Umbraco-CMS/src/Umbraco.Web.UI.Client/src/packages/tiptap/CLAUDE.md](https://github.com/umbraco/Umbraco-CMS/blob/3ee7b142b3c7cbb1fb3ef3520d27d2d8e5308e96/src/Umbraco.Web.UI.Client/src/packages/tiptap/CLAUDE.md) · 5201★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Umbraco Tiptap package - @umbraco-cms/backoffice/tiptap

[Umbraco Backoffice](../../../CLAUDE.md) | [Umbraco CMS Root](../../../../../CLAUDE.md)

---

## Overview

Extensible rich text editor (RTE) framework for the Umbraco CMS backoffice. Built on **Tiptap v3** (based on ProseMirror), this package provides a plugin architecture with 50+ built-in extensions for content editing.

**Package**: `@umbraco-cms/backoffice/tiptap`
**Name**: `Umbraco.Core.Tiptap`

### External Resources

- **Tiptap**: [tiptap.dev](https://tiptap.dev/) | [Documentation](https://tiptap.dev/docs) | [Source](https://github.com/ueberdosis/tiptap/)
- **ProseMirror** (underlying framework): [prosemirror.net](https://prosemirror.net/) | [Documentation](https://prosemirror.net/docs/) | [Source](https://github.com/ProseMirror/prosemirror)

---

## Directory Structure

```
tiptap/
├── components/                            # UI components
│   ├── input-tiptap/                      # Main editor component (`umb-input-tiptap`)
│   ├── toolbar/                           # Editor toolbar (`umb-tiptap-toolbar`)
│   ├── statusbar/                         # Editor status bar (`umb-tiptap-statusbar`)
│   ├── menu/
```

</details>
