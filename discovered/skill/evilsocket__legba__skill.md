---
name: evilsocket__legba__skill
source: https://github.com/evilsocket/legba/blob/74d1178deb4ad2007dfce7ecf2186b3390c7668f/skills/legba/SKILL.md
repo: evilsocket/legba
kind: skill
stars: 1897
last_pushed: 2026-05-20T12:49:30Z
license: other
score: 9
domains: [security, cli-tools]
tags: [bruteforce, enumeration, network-security]
curated: 2026-06-15
curated_by: config-scout
---

# evilsocket/legba — skill

**Why it's worth keeping:** It includes a critical meta-instruction to fetch documentation before generating specific plugin commands and provides granular details on complex credential expressions like templates and globs.

**Summary:** A highly structured skill file for the legba multi-protocol security tool, covering credential expression syntax and plugin usage.

**Source credibility:** High; specialized security tool with nearly 2k stars and active maintenance.

**Recency:** Current; specifically supports modern MCP (Model Context Protocol) standards.

**Source:** [evilsocket/legba/skills/legba/SKILL.md](https://github.com/evilsocket/legba/blob/74d1178deb4ad2007dfce7ecf2186b3390c7668f/skills/legba/SKILL.md) · 1897★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: legba
description: Use this skill when the user wants to brute-force credentials, spray passwords, or enumerate services/subdomains against any network protocol (HTTP, SSH, FTP, SMB, RDP, databases, mail protocols, DNS, etc.) using legba. Also use it when the user asks how to use legba, how to write a recipe, how to configure the REST API or MCP server, or asks for help constructing a legba command.
---

# legba

legba is a fast, multi-protocol credential bruteforcer, password sprayer, and enumerator written in Rust on top of the Tokio async runtime. It is a modern replacement for THC-Hydra, Medusa, Ncrack, and Patator — benchmarked at 4.5× faster on HTTP basic auth, 55× faster on SSH, 3.8× on MySQL vs. Hydra on identical hardware. It ships as a single static binary with no native dependencies and supports 30+ protocol plugins.

Full documentation: https://legba.evilsocket.net/
GitHub: https://github.com/evilsocket/legba

## Installation

```bash
# Precompiled binary (Linux/macOS) — recommended
# Download the latest release from https://github.com/evilsocket/legba/releases

# Homebrew (macOS / Linux)
brew tap evilsocket/legba https://github.com/evilsocket/legba
brew insta
```

</details>
