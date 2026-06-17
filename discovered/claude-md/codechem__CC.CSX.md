---
name: codechem__CC.CSX
source: https://github.com/codechem/CC.CSX/blob/468ec18c7c2d0199b04730c225b80c92e4f107b9/CLAUDE.md
repo: codechem/CC.CSX
kind: claude-md
stars: 34
last_pushed: 2026-06-12T00:40:37Z
license: apache-2.0
score: 9
domains: [csharp, web-frameworks, dsl]
tags: [dsl, code-generation, dotnet, html]
curated: 2026-06-16
curated_by: config-scout
---

# codechem/CC.CSX — claude-md

**Why it's worth keeping:** Provides explicit warnings against editing generated files and explains the 'magic' behind its declarative syntax (implicit conversions), which prevents the AI from making incorrect assumptions about types or workflows.

**Summary:** A highly detailed guide for a C# HTML DSL that covers package responsibilities, type hierarchies, and specific rendering paths. It includes vital instructions on how the DSL syntax is achieved through implicit conversions.

**Source credibility:** High-quality technical documentation for a specialized, actively maintained C# library.

**Recency:** 

**Source:** [codechem/CC.CSX/CLAUDE.md](https://github.com/codechem/CC.CSX/blob/468ec18c7c2d0199b04730c225b80c92e4f107b9/CLAUDE.md) · 34★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CC.CSX is a C# HTML generation library that allows developers to create HTML declaratively using pure C# code (JSX-like / Hiccup-like). Five NuGet packages live in this repo:

- **CC.CSX** (`src/CC.CSX/`): Core library — HTML element/attribute factories and rendering
- **CC.CSX.Web** (`src/CC.CSX.Web/`): ASP.NET Core integration — `HtmlResult` (implements `IResult`, `IActionResult`, `IEndpointMetadataProvider`)
- **CC.CSX.Htmx** (`src/CC.CSX.Htmx/`): HTMX attribute extensions (`hxPost`, `hxGet`, `target`, …) and `HtmxImports`
- **CC.CSX.Css** (`src/CC.CSX.Css/`): Strongly typed CSS sidecar — `CssClass` (incl. virtual/higher-order composed classes), `CssDeclaration` + lowercase `CssProperties` factories, `CssUnits` (`8.px()`), `CssBundle`/`CssImports`. Ships the `src/CC.CSX.Css.Generator/` source generator (netstandard2.0) which turns `.css` files registered as `AdditionalFiles` into typed members: `Css.<FileName>.<className>` constants, a baked-in `Source` const and a `Bundle`. Convention: elements are PascalCase, styles/classes are lowercase. Pl
```

</details>
