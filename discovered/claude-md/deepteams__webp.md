---
name: deepteams__webp
source: https://github.com/deepteams/webp/blob/1c6ff1b9a4dd77e6025a0236705294d09c750c11/CLAUDE.md
repo: deepteams/webp
kind: claude-md
stars: 20
last_pushed: 2026-06-12T13:53:46Z
license: other
score: 9
domains: [image-processing, cli-tools, go]
tags: [go, codec, low-level]
curated: 2026-06-15
curated_by: config-scout
---

# deepteams/webp — claude-md

**Why it's worth keeping:** The inclusion of 'Key Types' prevents signature hallucinations, while the 'Important Notes' warn about high-risk bit-level logic. The command section provides specific test patterns instead of just generic ones.

**Summary:** A high-quality technical guide for a low-level Go image codec that provides essential API signatures and architecture layers.

**Source credibility:** High; it is a specialized, recently updated Go library with specific technical detail.

**Recency:** Extremely current, referencing Go 1.24.2.

**Source:** [deepteams/webp/CLAUDE.md](https://github.com/deepteams/webp/blob/1c6ff1b9a4dd77e6025a0236705294d09c750c11/CLAUDE.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

Pure Go WebP image encoder/decoder (`github.com/deepteams/webp`). No CGo dependencies. Supports VP8 (lossy), VP8L (lossless), VP8X (extended format with metadata), alpha channels, and animation.

## Tech Stack

- **Go 1.24.2** - No external dependencies
- Integrates with Go's `image` package via `image.RegisterFormat()`
- CLI tool: `cmd/gwebp`

## Commands

```bash
# Build
go build ./...

# Build CLI
go build -o gwebp ./cmd/gwebp

# Run all tests
go test ./...

# Run specific package tests
go test ./internal/lossy
go test ./internal/lossless
go test ./animation
go test ./mux

# Run tests with verbose output
go test -v ./...

# Run benchmarks
go test -bench=. ./...
```

## Project Structure

```
webp.go / encode.go       # Public API (Decode, Encode, Options)
doc.go                     # Package documentation
animation/                 # Animation support (ANIM/ANMF frames)
cmd/gwebp/                 # CLI tool (encode/decode/info)
mux/                       # WebP multiplex/demultiplex
sharpyuv/                  # Sharp YUV color space conversion
internal/
  bitio/                   # Bit-level I/O (boolean arithmetic, lossless streams)
  container
```

</details>
