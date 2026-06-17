---
name: webiny__webiny-js__skill
source: https://github.com/webiny/webiny-js/blob/61109e7a2f248e3eebf634f02e1de28c6bf53647/skills/user-skills/project-structure/SKILL.md
repo: webiny/webiny-js
kind: skill
stars: 7992
last_pushed: 2026-06-15T18:15:17Z
license: other
score: 9
domains: [web-development, cloud-infrastructure]
tags: [architecture, typescript, configuration, serverless]
curated: 2026-06-15
curated_by: config-scout
---

# webiny/webiny-js — skill

**Why it's worth keeping:** It uses high-value 'YOU MUST' constraint rules to prevent common build errors and provides clear mapping tables between JSX elements and implementation requirements.

**Summary:** This skill file defines the specific architectural patterns and registration rules for a Webiny project using a central configuration file.

**Source credibility:** High; from a highly starred (7.9k+) and actively maintained enterprise CMS project.

**Recency:** 

**Source:** [webiny/webiny-js/skills/user-skills/project-structure/SKILL.md](https://github.com/webiny/webiny-js/blob/61109e7a2f248e3eebf634f02e1de28c6bf53647/skills/user-skills/project-structure/SKILL.md) · 7992★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: webiny-project-structure
context: webiny-extensions
description: >
  Webiny project layout, webiny.config.tsx anatomy, and extension registration.
  Use this skill when the developer asks about folder structure, where custom code goes,
  how to register extensions, what webiny.config.tsx does, or how the project is organized.
  Also use when they need to understand the relationship between extensions/, webiny.config.tsx,
  and the different extension types (Api, Admin, Infra, CLI).
---

# Webiny Project Structure

## TL;DR

A Webiny project has a flat structure centered around `webiny.config.tsx` -- the single configuration file where all extensions are registered. Custom code lives in the `extensions/` folder. Extensions are registered as React components (`<Api.Extension>`, `<Admin.Extension>`, `<Infra.*>`, `<Cli.Command>`) and can be conditionally loaded per environment.

## Project Layout

```
my-webiny-project/
├── extensions/          # All custom code -- API, Admin, Infra, CLI extensions
│   └── README.md
├── public/              # Static assets for the Admin app
│   ├── favicon.ico
│   ├── global.css
│   ├── index.html
│   └── robots.txt
├── package.json         #
```

</details>
