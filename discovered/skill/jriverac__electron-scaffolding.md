---
name: jriverac__electron-scaffolding
source: https://github.com/jriverac/electron-scaffolding/blob/3caa425b42292e087b24e4987e57cd7dcfcb65e1/skill.md
repo: jriverac/electron-scaffolding
kind: skill
stars: 0
last_pushed: 2026-01-26T15:35:24Z
license: unknown
score: 8
domains: [desktop-apps, frontend-tooling]
tags: [electron, react, vite, typescript, scaffolding]
curated: 2026-06-14
curated_by: config-scout
---

# jriverac/electron-scaffolding — skill

**Why it's worth keeping:** It provides specific boilerplate for the security-critical bridge between Main and Renderer processes (IPC + Preload) and detailed configuration files for TypeScript and Vite.

**Summary:** A comprehensive prompt template that directs an agent to scaffold a production-ready Electron application with React, Vite, and optional SQLite/Knex integration.

**Source credibility:** Low star count suggests a niche utility, but the technical specifications are high-quality and follow modern best practices.

**Recency:** Very current; uses modern versions of Vite, React, and TypeScript.

**Source:** [jriverac/electron-scaffolding/skill.md](https://github.com/jriverac/electron-scaffolding/blob/3caa425b42292e087b24e4987e57cd7dcfcb65e1/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Electron App Scaffolder

Creates a production-ready Electron application with TypeScript, React, Vite, and best practices.

## Usage

```bash
/electron-app <app-name> [--with-db] [--with-tests] [--with-storybook]
```

## Arguments

- `app-name` (required): Name of the application (kebab-case recommended)
- `--with-db`: Include SQLite database with Knex.js migrations
- `--with-tests`: Include Jest testing setup
- `--with-storybook`: Include Storybook for component development

## Instructions

When this skill is invoked, create a new Electron application following these steps:

### 1. Project Initialization

Create the project directory and initialize:

```bash
mkdir <app-name>
cd <app-name>
npm init -y
```

### 2. Directory Structure

Create the following structure:

```
<app-name>/
├── electron/
│   ├── main.ts
│   └── preload.ts
├── src/
│   ├── renderer/
│   │   ├── components/
│   │   ├── types/
│   │   │   └── electron.d.ts
│   │   ├── utils/
│   │   ├── App.tsx
│   │   ├── main.tsx
│   │   └── index.css
│   └── main/
├── dist/
│   ├── main/
│   └── renderer/
├── index.html
├── tsconfig.json
├── tsconfig.node.json
├── vite.config.ts
└── package.json
```

If `--with-db` is sp
```

</details>
