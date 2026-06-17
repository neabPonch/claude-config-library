---
name: spring-projects__spring-tools
source: https://github.com/spring-projects/spring-tools/blob/cbb8bba0e8898e024b97b1c77818e8645079d372/CLAUDE.md
repo: spring-projects/spring-tools
kind: claude-md
stars: 968
last_pushed: 2026-06-12T20:13:07Z
license: epl-1.0
score: 10
domains: [language-servers, developer-tools, java, ide-extensions]
tags: [multi-build-system, lsp, maven, vscode-extension, technical-documentation]
curated: 2026-06-15
curated_by: config-scout
---

# spring-projects/spring-tools — claude-md

**Why it's worth keeping:** Uses highly specific command snippets for different levels of granularity; includes critical 'how-to' documentation for connecting running processes to debug them; provides architectural context essential for high-level reasoning.

**Summary:** A comprehensive technical manual detailing multi-layered build systems (Maven, Tycho, npm) and complex debugging workflows for a language server project. It provides exact commands for granular building, testing, and runtime connection procedures.

**Source credibility:** High-quality professional maintenance by the Spring Projects organization.

**Recency:** Extremely current, with active development and recent updates.

**Source:** [spring-projects/spring-tools/CLAUDE.md](https://github.com/spring-projects/spring-tools/blob/cbb8bba0e8898e024b97b1c77818e8645079d372/CLAUDE.md) · 968★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

Spring Tools (STS4) is a comprehensive IDE tooling suite for Spring Boot development. It provides extensions for Eclipse IDE, Visual Studio Code, and Eclipse Theia. The core architecture uses the Language Server Protocol (LSP): Java language servers run as separate processes, with thin client integrations for each IDE.

## Directory Structure

```
sts4/
├── headless-services/          # Java Language Servers (Maven-based)
│   ├── commons/                # Shared libraries and LSP infrastructure
│   ├── spring-boot-language-server/      # Core Spring Boot language server (with JDT LS)
│   ├── spring-boot-language-server-standalone/  # Standalone variant (Jandex, no JDT LS)
│   ├── manifest-yaml-language-server/   # Cloud Foundry manifest YAML support
│   ├── concourse-language-server/       # Concourse CI pipeline support
│   ├── bosh-language-server/            # BOSH configuration support
│   ├── jdt-ls-extension/       # Eclipse JDT Language Server extensions
│   └── xml-ls-extension/       # XML language server extension
├── eclipse-extensi
```

</details>
