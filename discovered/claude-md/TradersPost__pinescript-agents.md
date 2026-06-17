---
name: TradersPost__pinescript-agents
source: https://github.com/TradersPost/pinescript-agents/blob/e78730d468db9eaa70186eb82c7cbd020b271e50/CLAUDE.md
repo: TradersPost/pinescript-agents
kind: claude-md
stars: 110
last_pushed: 2026-06-04T21:25:32Z
license: unknown
score: 9
domains: [trading-finance, domain-specific-languages, cli-tools, agents-ai]
tags: [pinescript, proactive-agent, syntax-guardrails, workflow-automation]
curated: 2026-06-16
curated_by: config-scout
---

# TradersPost/pinescript-agents — claude-md

**Why it's worth keeping:** It uses 'state-aware prompting' (checking file existence to decide greetings) and defines strict syntactic guardrails for domain-specific errors. The deterministic instruction to run tools immediately upon pattern detection (YouTube URLs) minimizes friction.

**Summary:** A high-agency configuration that transforms Claude into a proactive specialist with stateful onboarding and automated tool workflows.

**Source credibility:** High; the repo is highly specialized with significant community traction (110 stars).

**Recency:** Very current; reflects modern agentic patterns such as proactive initialization and tool-driven workflows.

**Source:** [TradersPost/pinescript-agents/CLAUDE.md](https://github.com/TradersPost/pinescript-agents/blob/e78730d468db9eaa70186eb82c7cbd020b271e50/CLAUDE.md) · 110★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Pine Script Development Assistant - Claude Code Instructions

## Overview
You are now equipped with specialized Pine Script development capabilities. This project provides you with comprehensive Pine Script v6 knowledge, specialized skills, and a template library to help users create professional TradingView indicators and strategies.

## ⚠️ CRITICAL: Pine Script Syntax Rules

### Line Continuation - NEVER Split These Across Lines:
Pine Script does NOT support arbitrary line breaks. These cause "end of line without line continuation" errors:

**WRONG:**
```pinescript
titleText = regressionMode == "Static" ? "Static Regression" :
            regressionMode == "Live" ? "Live Regression" :
            "Regression Statistics"
```

**CORRECT - Keep on one line:**
```pinescript
titleText = regressionMode == "Static" ? "Static Regression" : regressionMode == "Live" ? "Live Regression" : "Regression Statistics"
```

**Rule**: Ternary operators (`? :`), logical expressions (`and`, `or`), and arithmetic spanning lines MUST have continuation lines indented MORE than the starting line, OR be kept on a single line. When in doubt, use single lines for complex expressions.

See: `docs/pinescrip
```

</details>
