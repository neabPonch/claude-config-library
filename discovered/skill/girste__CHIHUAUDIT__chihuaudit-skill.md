---
name: girste__CHIHUAUDIT__chihuaudit-skill
source: https://github.com/girste/CHIHUAUDIT/blob/34f1f39956fbf77bff64df16d87445e87a8dd306/docs/skill/chihuaudit-skill.md
repo: girste/CHIHUAUDIT
kind: skill
stars: 51
last_pushed: 2026-02-07T18:04:49Z
license: mit
score: 8
domains: [security, devops, cli-tools]
tags: [system-audit, linux-security, infrastructure]
curated: 2026-06-16
curated_by: config-scout
---

# girste/CHIHUAUDIT — skill

**Why it's worth keeping:** Includes advanced agentic patterns like multi-stage/tiered execution (Basic vs. Deep Dive) and provides practical sysadmin implementation details like specific sudoers configurations.

**Summary:** A high-density system audit protocol that enables Claude to perform professional Linux security and health assessments via structured shell execution.

**Source credibility:** Moderate community interest with 51 stars on GitHub.

**Recency:** Very current, updated within the last 4 months.

**Source:** [girste/CHIHUAUDIT/docs/skill/chihuaudit-skill.md](https://github.com/girste/CHIHUAUDIT/blob/34f1f39956fbf77bff64df16d87445e87a8dd306/docs/skill/chihuaudit-skill.md) · 51★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Chihuaudit Claude Skill - Complete System Audit

**Skill Type**: Autonomous system security and health audit with zero user interaction required.

**Compatibility**: Tested with Claude Sonnet 4.5, Opus 4.5, and Haiku 4.5 models.

## Purpose

Execute a comprehensive, read-only Linux system audit that replicates the functionality of the Chihuaudit binary tool through native shell commands. This skill enables Claude to perform professional-grade infrastructure assessments without requiring any binary installation or dependencies.

**Key Features**:
- 🔒 **100% Read-Only** - Zero system modifications, completely safe for production
- ⚡ **Parallel Execution** - Optimized batch commands for sub-60-second completion
- 🎯 **Precise Detection** - Intelligent command existence checks and graceful degradation
- 📊 **Structured Output** - Clear categorization with visual indicators (✅ ⚠️ ❌)
- 🔄 **Consistent Results** - Battle-tested across 1+ years of production use

## What it checks

### 🔒 Security (Basic)
- Firewall status and rules (ufw/iptables)
- SSH configuration (port, auth methods, allowed users)
- Fail2ban status and active jails
- TLS/SSL certificates (Let's Encrypt, Caddy, Certbot)
```

</details>
