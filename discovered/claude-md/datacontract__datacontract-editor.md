---
name: datacontract__datacontract-editor
source: https://github.com/datacontract/datacontract-editor/blob/43c534a68f16679b898ff91d070b732fdc71d026/CLAUDE.md
repo: datacontract/datacontract-editor
kind: claude-md
stars: 99
last_pushed: 2026-06-13T07:26:29Z
license: mit
score: 7
domains: [web-frontend, react]
tags: [documentation-links, domain-specific, styling-rules]
curated: 2026-06-15
curated_by: config-scout
---

# datacontract/datacontract-editor — claude-md

**Why it's worth keeping:** The pattern of linking exact documentation sites for libraries and defining key terms via URL is highly effective at preventing hallucinations.

**Summary:** Provides explicit documentation URLs and defines domain-specific terminology to ensure model accuracy.

**Source credibility:** Moderate; a specialized repository with recent activity.

**Recency:** Current, as it references modern technologies like Tailwind v4.

**Source:** [datacontract/datacontract-editor/CLAUDE.md](https://github.com/datacontract/datacontract-editor/blob/43c534a68f16679b898ff91d070b732fdc71d026/CLAUDE.md) · 99★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
Automatically use context7 for code generation and library documentation.

We use React with Javascript and Vite.

As documentation and when looking up apis for the react libraries use the following context7 stuffs:
- https://react.dev/
- /remix-run/react-router 
- /eemeli/yaml
- /pmndrs/zustand
- /websites/reactflow_dev

Use Tailwind CSS with Tailwind Plus as a style guide.
Use TailwindPlus react for TailwindCSS v4.
Do never use Heroicons

Use Playwright CLI tool to test if you are unsure.
If you need to start a server, use port 9090 or greater.
To test stuff that is only available in embedded mode, use /embed suburl

When the term data contract is used, this refers to https://raw.githubusercontent.com/bitol-io/open-data-contract-standard/refs/heads/dev/docs/README.md
```

</details>
