---
name: mkorman90__regipy
source: https://github.com/mkorman90/regipy/blob/f315415864889c3ee2a03d8a9e5c52486dcb631b/CLAUDE.md
repo: mkorman90/regipy
kind: claude-md
stars: 275
last_pushed: 2026-06-13T16:31:50Z
license: mit
score: 9
domains: [security, forensics, cli-tools]
tags: [api-reference, plugin-system, extension-guide]
curated: 2026-06-14
curated_by: config-scout
---

# mkorman90/regipy — claude-md

**Why it's worth keeping:** It includes 'how-to' code templates for both using the library and building new plugins, which is crucial for agentic task completion. The semantic mapping of artifacts to hive types also provides excellent context for forensic reasoning.

**Summary:** A high-density technical manual that provides structural hierarchy, core API usage patterns via code snippets, and a rigorous protocol for extending the system through plugins.

**Source credibility:** High-quality niche security tool with active maintenance and significant community interest.

**Recency:** Current; includes highly relevant modern patterns like MCP (Model Context Protocol) integration.

**Source:** [mkorman90/regipy/CLAUDE.md](https://github.com/mkorman90/regipy/blob/f315415864889c3ee2a03d8a9e5c52486dcb631b/CLAUDE.md) · 275★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - regipy

> OS-independent Python library for parsing offline Windows registry hives

## Project Overview

regipy is a forensic-focused library for parsing Windows registry hive files (files with REGF header). It's designed for digital forensics and incident response (DFIR) workflows, providing both a Python API and CLI tools.

### Core Capabilities

- Parse offline registry hives without Windows dependencies
- Recursive traversal of keys and values from any path
- Transaction log recovery (dirty hive reconstruction)
- Hive comparison/diffing (like RegShot)
- Extensible plugin system for artifact extraction
- Timeline generation for forensic analysis

## Architecture

```
regipy/
├── registry.py          # Core RegistryHive class - entry point for all parsing
├── structs.py           # Binary struct definitions (REGF header, NK/VK records, etc.)
├── hive_types.py        # Hive type constants (NTUSER, SYSTEM, SOFTWARE, SAM, etc.)
├── exceptions.py        # Custom exceptions (RegistryKeyNotFoundException, etc.)
├── utils.py             # Helpers: convert_wintime, boomerang_stream, etc.
├── recovery.py          # Transaction log application logic
├── plugins/
│   ├── plugi
```

</details>
