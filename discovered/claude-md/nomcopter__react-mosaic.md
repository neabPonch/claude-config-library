---
name: nomcopter__react-mosaic
source: https://github.com/nomcopter/react-mosaic/blob/6f07fd525a5459a30dce811717ec96725688aea0/claude.md
repo: nomcopter/react-mosaic
kind: claude-md
stars: 4754
last_pushed: 2026-04-21T19:02:51Z
license: other
score: 9
domains: [web-frontend, ui-library]
tags: [react, architecture, monorepo, component-library]
curated: 2026-06-15
curated_by: config-scout
---

# nomcopter/react-mosaic — claude-md

**Why it's worth keeping:** Employs 'mental model' documentation (tree/path logic) rather than just file lists; uses explicit labels like '[CRITICAL]' and '[PRIMARY FOCUS]' to guide LLM attention toward business logic.

**Summary:** Provides deep architectural mental models of a complex N-ary tree structure and path system used for layout management. It explicitly maps out the relationship between core components, types, and critical utility functions.

**Source credibility:** High: Popular open-source project with 4.7k+ stars and recent activity.

**Recency:** Current: Uses modern toolchain including Nx, Vite, and React 16-19 support.

**Source:** [nomcopter/react-mosaic/claude.md](https://github.com/nomcopter/react-mosaic/blob/6f07fd525a5459a30dce811717ec96725688aea0/claude.md) · 4754★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# React Mosaic - LLM Integration Guide

## Project Overview

**React Mosaic** is a powerful React component library that provides a tiling window manager for building sophisticated, user-controlled interfaces. Users can dynamically resize, rearrange, and customize panel layouts through an intuitive drag-and-drop interface.

**Key Information:**

- **Package**: `react-mosaic-component`
- **Version**: 7.0.0-beta0
- **License**: Apache License 2.0
- **React Support**: React 16-19
- **TypeScript**: Full TypeScript support
- **Build System**: Nx monorepo with Vite and tsup

## Architecture

### Core Concepts

#### 1. N-ary Tree Structure

The layout system uses an n-ary tree structure where nodes can have multiple children:

```typescript
type MosaicNode<T> = MosaicSplitNode<T> | MosaicTabsNode<T> | T;

interface MosaicSplitNode<T> {
  type: 'split';
  direction: 'row' | 'column';
  children: MosaicNode<T>[];
  splitPercentages?: number[]; // Defaults to equal distribution
}

interface MosaicTabsNode<T> {
  type: 'tabs';
  tabs: T[];
  activeTabIndex: number;
}
```

- **Split Nodes**: Container nodes that divide space between multiple children (horizontally or vertically)
- **Tab Nodes*
```

</details>
