---
name: passwordless-lib__fido2-net-lib
source: https://github.com/passwordless-lib/fido2-net-lib/blob/b141b59bc9328564144da839f9b00e16186be731/CLAUDE.md
repo: passwordless-lib/fido2-net-lib
kind: claude-md
stars: 1436
last_pushed: 2026-04-20T15:45:25Z
license: mit
score: 9
domains: [.net, security, backend]
tags: [dotnet, architecture-map, cli-commands]
curated: 2026-06-17
curated_by: config-scout
---

# passwordless-lib/fido2-net-lib — claude-md

**Why it's worth keeping:** The breakdown of the project structure (Architecture) combined with explicit 'dotnet' CLI commands and C# coding standards creates a perfect context for agentic development.

**Summary:** Provides a comprehensive map of a multi-project .NET solution including specific build/test commands and architectural boundaries.

**Source credibility:** Highly credible; the repo is a well-starred, actively maintained security library.

**Recency:** Very current, targeting .NET 8/C# 12.

**Source:** [passwordless-lib/fido2-net-lib/CLAUDE.md](https://github.com/passwordless-lib/fido2-net-lib/blob/b141b59bc9328564144da839f9b00e16186be731/CLAUDE.md) · 1436★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the FIDO2 .NET Library (WebAuthn) - a working implementation library for FIDO2 and WebAuthn using .NET. It provides a developer-friendly and well-tested .NET FIDO2 Server/WebAuthn relying party library for validation of registration (attestation) and authentication (assertion) of FIDO2/WebAuthn credentials.

## Architecture

The solution is organized into several key projects:

### Core Library Projects

- **Src/Fido2.Models** - Core data models and DTOs for FIDO2/WebAuthn, shared across all projects
- **Src/Fido2** - Main FIDO2 library with attestation/assertion verification logic, cryptographic operations, and metadata service integration
- **Src/Fido2.AspNet** - ASP.NET Core integration helpers and extensions
- **Src/Fido2.Ctap2** - CTAP2 protocol implementation for FIDO2 authenticators
- **Src/Fido2.BlazorWebAssembly** - Blazor WebAssembly-specific components and helpers
- **Src/Fido2.Development** - Development and testing utilities

### Demo/Example Projects

- **Demo** - ASP.NET Core demo application showing FIDO2 registration and
```

</details>
