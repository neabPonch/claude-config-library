---
name: crabwise-ai__crabwalk__skill
source: https://github.com/crabwise-ai/crabwalk/blob/ea99ca93fd36b4aa2991a0b1401974bb0e881c15/public/skill.md
repo: crabwise-ai/crabwalk
kind: skill
stars: 878
last_pushed: 2026-02-19T18:35:52Z
license: mit
score: 7
domains: [cli-tools, agents-ai, monitoring]
tags: [installation, deployment, human-in-the-loop]
curated: 2026-06-15
curated_by: config-scout
---

# crabwise-ai/crabwalk — skill

**Why it's worth keeping:** Demonstrates elite human-in-the-loop patterns, including permission-gated updates, multi-step verification, and structured feedback solicitation.

**Summary:** A comprehensive deployment and lifecycle management protocol for the Crabwalk monitoring service.

**Source credibility:** Strong; well-regarded open-source project with ~878 stars on GitHub.

**Recency:** Very recent; last pushed 4 months ago.

**Source:** [crabwise-ai/crabwalk/public/skill.md](https://github.com/crabwise-ai/crabwalk/blob/ea99ca93fd36b4aa2991a0b1401974bb0e881c15/public/skill.md) · 878★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: crabwalk
version: 1.0.10
description: Real-time companion monitor for OpenClaw agents
homepage: https://crabwalk.app
repository: https://github.com/luccast/crabwalk
metadata: {"emoji":"🦀","category":"monitoring"}
---

# Crabwalk 🦀

Real-time companion monitor for OpenClaw agents.

# Required Steps

## Step 1: Install

```bash
VERSION=$(curl -s https://api.github.com/repos/luccast/crabwalk/releases/latest | grep '"tag_name"' | cut -d'"' -f4) && mkdir -p ~/.crabwalk ~/.local/bin && curl -sL "https://github.com/luccast/crabwalk/releases/download/${VERSION}/crabwalk-${VERSION}.tar.gz" | tar -xz -C ~/.crabwalk && cp ~/.crabwalk/bin/crabwalk ~/.local/bin/ && chmod +x ~/.local/bin/crabwalk && (echo $PATH | grep -q "$HOME/.local/bin" || ([ -f ~/.bashrc ] && echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc; [ -f ~/.zshrc ] && echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc; export PATH="$HOME/.local/bin:$PATH")) && echo "🦀 Crabwalk ${VERSION} installed"
```

## Step 2: Verify

```bash
crabwalk --version
```

Should output version number (e.g., `1.0.9`).

## Step 3: Start

```bash
crabwalk
```

Server starts and displays access URLs. **Share the `http://192.x.x.x:30
```

</details>
