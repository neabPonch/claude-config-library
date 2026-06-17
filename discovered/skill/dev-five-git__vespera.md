---
name: dev-five-git__vespera
source: https://github.com/dev-five-git/vespera/blob/6242533483056b20bb363c34917133a395044aa8/SKILL.md
repo: dev-five-git/vespera
kind: skill
stars: 26
last_pushed: 2026-06-15T12:18:36Z
license: unknown
score: 8
domains: [backend-api, rust]
tags: [openapi, axum, validation]
curated: 2026-06-15
curated_by: config-scout
---

# dev-five-git/vespera — skill

**Why it's worth keeping:** It contains specific macro patterns (route discovery), type-to-schema mappings, and the crucial `Validated<T>` pattern for error handling. The 'File Structure → URL Mapping' section is perfect context for an AI to understand project routing logic without manual probing.

**Summary:** A highly structured technical reference for Vespera, a Rust framework that automates OpenAPI generation and request validation for Axum.

**Source credibility:** Small-scale enthusiast project (26 stars) with exceptionally high-quality documentation density.

**Recency:** Current; utilizes modern Rust, Axum, and OpenAPI 3.1 standards.

**Source:** [dev-five-git/vespera/SKILL.md](https://github.com/dev-five-git/vespera/blob/6242533483056b20bb363c34917133a395044aa8/SKILL.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vespera
description: Build APIs with Vespera - FastAPI-like DX for Rust/Axum. Covers route handlers, Schema derivation, and OpenAPI generation.
---

# Vespera Usage Guide

Vespera = FastAPI DX for Rust. Zero-config OpenAPI 3.1 generation via compile-time macro scanning.

## Quick Start

```rust
use vespera::{vespera, Serve, Schema, Validated, axum::Json};
use axum::extract::Path;
use serde::{Deserialize, Serialize};
use garde::Validate;

// 1. Custom types — derive Schema for OpenAPI inclusion.
//    Add `garde::Validate` to opt into 422 validation.
#[derive(Serialize, Deserialize, Schema, Validate)]
pub struct CreateUser {
    #[garde(length(min = 3, max = 32))]
    pub name: String,
    #[garde(email)]
    pub email: String,
}

// 2. Route handlers — MUST be `pub async fn`.
#[vespera::route(get, path = "/{id}", tags = ["users"])]
pub async fn get_user(Path(id): Path<u32>) -> Json<CreateUser> { /* ... */ }

// 3. Validated extractor → automatic 422 on bad input.
#[vespera::route(post, tags = ["users"])]
pub async fn create_user(
    Validated(Json(req)): Validated<Json<CreateUser>>,
) -> Json<&'static str> {
    // `req` already passed validation. Failures never reach he
```

</details>
