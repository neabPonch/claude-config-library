---
name: flamingo-stack__openframe-oss-tenant
source: https://github.com/flamingo-stack/openframe-oss-tenant/blob/5f47273ab3b328589ce078bd76e048e230e80306/CLAUDE.md
repo: flamingo-stack/openframe-oss-tenant
kind: claude-md
stars: 61
last_pushed: 2026-06-16T05:57:44Z
license: other
score: 9
domains: [backend-api, web-frontend, distributed-systems]
tags: [polyglot, microservices, architecture, java, rust]
curated: 2026-06-16
curated_by: config-scout
---

# flamingo-stack/openframe-oss-tenant — claude-md

**Why it's worth keeping:** Explicitly documents complex behavioral patterns like the JWT cookie-to-header conversion and Kafka data pipelines. The inclusion of OS-specific startup scripts and a detailed service hierarchy is highly transferable.

**Summary:** A high-density architectural blueprint for a polyglot microservices project involving Java, Next.js, and Rust. It provides crucial context on data flow, authentication patterns, and service interactions.

**Source credibility:** Active open-source project with decent social proof (61 stars).

**Recency:** Highly current, using cutting-edge tech stacks like Java 21 and React 19.

**Source:** [flamingo-stack/openframe-oss-tenant/CLAUDE.md](https://github.com/flamingo-stack/openframe-oss-tenant/blob/5f47273ab3b328589ce078bd76e048e230e80306/CLAUDE.md) · 61★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Essential Commands

### Build Commands
```bash
mvn clean install                           # Build all Java services and libraries
mvn clean install -DskipTests              # Build without running tests
mvn test                                    # Run all tests
```

### Frontend (UI) Commands
```bash
cd openframe/services/openframe-frontend
npm install                                 # Install dependencies
npm run dev                                 # Start development server
npm run build                               # Build for production
npm run type-check                          # TypeScript type checking
```

### Rust Client Commands
```bash
cd client
cargo build                                 # Build the Rust client
cargo test                                  # Run Rust tests
cargo run                                   # Run the client locally
```

### Local Development
```bash
# Platform-specific startup scripts:
./scripts/run-mac.sh                        # macOS
./scripts/run-linux.sh                      # Linux
./scripts/run-windows.ps1
```

</details>
