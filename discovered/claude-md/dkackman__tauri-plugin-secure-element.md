---
name: dkackman__tauri-plugin-secure-element
source: https://github.com/dkackman/tauri-plugin-secure-element/blob/886ddbfe370b5512e917e1b373ad7fa23f591953/CLAUDE.md
repo: dkackman/tauri-plugin-secure-element
kind: claude-md
stars: 5
last_pushed: 2026-06-15T13:49:49Z
license: apache-2.0
score: 9
domains: [rust, mobile-development, cross-platform, security]
tags: [monorepo, multi-language, build-workflow, plugin-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# dkackman/tauri-plugin-secure-element — claude-md

**Why it's worth keeping:** The 'Important Files' section maps high-level logic to specific file paths, and the 'Common Tasks' provides a clear algorithmic workflow for cross-platform feature implementation.

**Summary:** A highly structured guide for a multi-language monorepo spanning Rust, Swift, Kotlin, and TypeScript. It detail specific build orders and platform dependencies.

**Source credibility:** High; professional-grade documentation for a specialized security plugin with active maintenance.

**Recency:** 

**Source:** [dkackman/tauri-plugin-secure-element/CLAUDE.md](https://github.com/dkackman/tauri-plugin-secure-element/blob/886ddbfe370b5512e917e1b373ad7fa23f591953/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Tauri Plugin Secure Element

A Tauri plugin providing secure element functionality for iOS, Android, macOS, and Windows platforms.

## Project Structure

This is a **pnpm workspace monorepo** with the following structure:

```bash
tauri-plugin-secure-element/          # Root monorepo
├── tauri-plugin-secure-element/      # Main plugin code
│   ├── src/                          # Rust plugin implementation
│   ├── guest-js/                     # TypeScript guest bindings
│   ├── swift/                        # Shared Swift code (Secure Enclave, FFI)
│   ├── ios/                          # Swift iOS plugin wrapper
│   ├── android/                      # Kotlin implementation
│   ├── permissions/                  # Plugin permissions
│   └── dist-js/                      # Built JavaScript bindings (generated)
├── test-app/                         # Example Tauri application
│   ├── src/                          # Svelte frontend
│   └── src-tauri/                    # Tauri backend
└── docs/                             # Additional documentation
```

## Tech Stack

- **Rust**: Plugin backend (v1.77.2+)
- **TypeScript**: Guest JavaScript API
- **Swift**: iOS implementation
- **Kotli
```

</details>
