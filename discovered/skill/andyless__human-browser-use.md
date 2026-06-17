---
name: andyless__human-browser-use
source: https://github.com/andyless/human-browser-use/blob/c493412e4f0923369f6526ebde942d0f46ad8a59/skill.md
repo: andyless/human-browser-use
kind: skill
stars: 2
last_pushed: 2026-03-14T09:44:40Z
license: mit
score: 8
domains: [agents-ai, web-automation, security]
tags: [browser-use, stealth, humanization]
curated: 2026-06-14
curated_by: config-scout
---

# andyless/human-browser-use — skill

**Why it's worth keeping:** It provides specific, actionable parameters like lognormal typing delays, overshoot probabilities, and inertia scrolling to bypass sophisticated bot detection.

**Summary:** A specialized wrapper for browser-use that injects human-like mouse trajectories, typing rhythms, and anti-bot stealth behaviors.

**Source credibility:** Low star count suggests a niche/new tool, but the technical specificity indicates high-quality automation engineering.

**Recency:** Very recent (3 months ago), making it highly relevant to current agentic browser frameworks.

**Source:** [andyless/human-browser-use/skill.md](https://github.com/andyless/human-browser-use/blob/c493412e4f0923369f6526ebde942d0f46ad8a59/skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# human-browser-use Skill

> Human-like browser automation extension for [browser-use](https://github.com/browser-use/browser-use).

## When to use

Use `human-browser-use` instead of raw `browser-use` when:
- The target site has anti-bot detection (Cloudflare, reCAPTCHA, DataDome, etc.)
- You need mouse movements to look like a real person
- You need typing to have natural rhythm and occasional typos
- You need to hide automation fingerprints (`navigator.webdriver`, WebGL, etc.)

## Installation

```bash
pip install human-browser-use
```

## CLI (preferred for quick tasks)

```bash
hbu open https://example.com       # Navigate
hbu state                           # See elements
hbu click 5                         # Click (human-like trajectory)
hbu type "Hello"                    # Type (human-like dynamics)
hbu screenshot page.png             # Screenshot
hbu close                           # Close
```

All browser-use CLI commands work with `hbu`. The browser stays alive between commands.

## Python API

```python
import asyncio
from human_browser_use import HumanBrowserSession, HumanBrowserProfile, HumanBehaviorConfig

async def main():
    session = HumanBrowserSession(
```

</details>
