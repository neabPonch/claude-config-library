---
name: compute-toys__compute.toys
source: https://github.com/compute-toys/compute.toys/blob/6c62642b145a48147fa195cdfe560b16f28c5908/CLAUDE.md
repo: compute-toys/compute.toys
kind: claude-md
stars: 187
last_pushed: 2026-05-12T04:31:48Z
license: mit
score: 9
domains: [web-frontend, graphics-webgpu, fullstack]
tags: [nextjs, webgpu, wasm, supabase, cloudflare-workers]
curated: 2026-06-15
curated_by: config-scout
---

# compute-toys/compute.toys — claude-md

**Why it's worth keeping:** Excellent detail on non-obvious setup steps (like manual WASM downloads) and critical configuration warnings regarding Cloudflare/TypeScript compatibility.

**Summary:** Provides an exhaustive technical map of a complex WebGPU/WASM stack including specialized command workflows and deployment nuances.

**Source credibility:** High-quality repository with significant technical depth and recent maintenance activity.

**Recency:** Very current, utilizing modern tech like Next.js 15 and OpenNext.

**Source:** [compute-toys/compute.toys/CLAUDE.md](https://github.com/compute-toys/compute.toys/blob/6c62642b145a48147fa195cdfe560b16f28c5908/CLAUDE.md) · 187★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

**Setup:**
- `git submodule update --init --recursive` - Clone submodules (required for dependencies)
- `yarn` - Install dependencies
- `npx supabase start` - Start local database

**Core Development:**
- `yarn dev` - Start development server
- `yarn build` - Build for production (required for CI/CD)
- `yarn lint` - Check for lint errors/warnings  
- `yarn fix` - Auto-fix lint errors

**Specialized Commands:**
- `yarn preview` - Build and preview with OpenNext Cloudflare (Workers deployment)
- `yarn download-wasm` - Download Slang WASM files (auto-runs in prebuild)
- `yarn download-wasm:force` - Force re-download WASM files
- `yarn cf-typegen` - Generate Cloudflare Worker types
- `yarn supabase:types` - Generate database types from local Supabase
- `yarn supabase:reset` - Reset local database

**Environment Setup:**
Set these in `.env`:
- `NEXT_PUBLIC_SUPABASE_URL=http://127.0.0.1:54321` (local development)
- `NEXT_PUBLIC_SUPABASE_PUBLIC_API_KEY=<anon key from supabase start output>`
- Test user: `user@example.com` / `pass`

## Architecture O
```

</details>
