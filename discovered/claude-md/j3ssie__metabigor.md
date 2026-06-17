---
name: j3ssie__metabigor
source: https://github.com/j3ssie/metabigor/blob/c47664e8d3ac96e3d723f7f5501d242245ee5f63/CLAUDE.md
repo: j3ssie/metabigor
kind: claude-md
stars: 1543
last_pushed: 2026-02-15T15:22:05Z
license: mit
score: 9
domains: [cli-tools, security]
tags: [go, osnt, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# j3ssie/metabigor — claude-md

**Why it's worth keeping:** The 'Important Context for AI Assistants' section is exceptional, explicitly detailing non-obvious constraints like stdin piping requirements, specific error-handling patterns, and concurrency limits to prevent regressions.

**Summary:** A comprehensive blueprint for a Go-based CLI tool that covers architecture, data flow, and rigorous development workflows.

**Source credibility:** High; comes from a popular OSINT project with significant GitHub stars (1.5k+).

**Recency:** Very current; mentions Go 1.24 and was updated recently.

**Source:** [j3ssie/metabigor/CLAUDE.md](https://github.com/j3ssie/metabigor/blob/c47664e8d3ac96e3d723f7f5501d242245ee5f63/CLAUDE.md) · 1543★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Metabigor - CLAUDE.md

**Project**: Metabigor - OSINT intelligence tool without API key hassle
**Version**: v2.1.0
**Language**: Go 1.24.0
**Author**: [@j3ssie](https://twitter.com/j3ssie)
**License**: MIT

## Project Overview

Metabigor is a command-line OSINT (Open Source Intelligence) tool designed to perform network reconnaissance and intelligence gathering without requiring API keys. It's part of the Osmedeus Engine ecosystem and focuses on seven core capabilities:

1. **Network Discovery** (`net`) - Find IP ranges (CIDRs) from ASN, organization, domain, or IP
2. **Certificate Transparency** (`cert`) - Discover subdomains via crt.sh certificate logs
3. **IP Enrichment** (`ip`) - Get port/service/vulnerability data via Shodan InternetDB (free)
4. **GitHub Code Search** (`github`) - Find secrets and credentials in public repos via grep.app
5. **IP Clustering** (`ipc`) - Group IPs by ASN for infrastructure mapping
6. **Related Domains** (`related`) - Discover related domains via cert logs, WHOIS, analytics
7. **CDN/WAF Detection** (`cdn`) - Identify if IPs are behind CDN or WAF providers

## Architecture

### Directory Structure

```
metabigor/
├── cmd/metabigor/          # Mai
```

</details>
