---
name: cyberia-to__cyb__claude
source: https://github.com/cyberia-to/cyb/blob/53bef66eeb69a8301af631ed2f3a55da5a48a721/cyb-boot/CLAUDE.md
repo: cyberia-to/cyb
kind: claude-md
stars: 175
last_pushed: 2026-06-09T11:13:32Z
license: unknown
score: 8
domains: [cli-tools, systems-programming, security]
tags: [installer, bootstrapping, rust, distribution]
curated: 2026-06-15
curated_by: config-scout
---

# cyberia-to/cyb — claude-md

**Why it's worth keeping:** Uses a strict 'Rules' section to prevent AI from making catastrophic deployment errors (like uploading internal artifacts to GitHub). The structure effectively communicates architectural boundaries between the installer and the main app.

**Summary:** Defines the high-stakes bootstrapping process and distribution constraints for the cyb ecosystem.

**Source credibility:** The repo shows active maintenance and highly specific, non-generic technical implementation details.

**Recency:** Very current; uses modern technologies like iroh, CIDs, and AES-256-GCM.

**Source:** [cyberia-to/cyb/cyb-boot/CLAUDE.md](https://github.com/cyberia-to/cyb/blob/53bef66eeb69a8301af631ed2f3a55da5a48a721/cyb-boot/CLAUDE.md) · 175★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# cyb-boot — project rules

## What cyb-boot IS

A thin installer (~3MB) that bootstraps the cyb desktop app from the content-addressed network. It is NOT the app itself.

Target flow (from design doc):
1. Import wallet from boot.dat (mnemonic + referrer)
2. Connect to iroh bootstrap nodes
3. Fetch version registry particle (hardcoded CID)
4. Resolve latest cyb CID for user's platform from registry
5. Download cyb binary by CID (hash-verified by iroh)
6. Install cyb
7. Launch cyb → first network sync registers referral as cyberlink

Current implementation is simplified — uses HTTP download from GitHub instead of iroh. See README.md "Current vs Target" table.

## Key concepts

- **Two apps**: cyb-boot (installer) downloads and installs cyb (the actual app), then exits
- **Version registry**: a particle in the knowledge graph at a known CID, maps platforms to cyb binary CIDs
- **Referral embedding**: server patches a 64-byte slot in the pre-built binary with the referrer address (no recompilation)
- **macOS notarization**: .app bundle must be pre-signed+notarized in CI. Server cannot modify the binary — only appends boot.dat alongside in the zip
- **boot.dat**: AES-256-GCM encrypted
```

</details>
