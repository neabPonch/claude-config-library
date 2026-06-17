---
name: j-klawson__security-gym
source: https://github.com/j-klawson/security-gym/blob/320da052480e8dd0ec985dcb99b0ab1e2f19ab94/CLAUDE.md
repo: j-klawson/security-gym
kind: claude-md
stars: 3
last_pushed: 2026-06-07T18:07:47Z
license: apache-2.0
score: 9
domains: [security, reinforcement-learning, data-engineering]
tags: [cybersecurity, gymnasium, ebpf, rl-environment]
curated: 2026-06-15
curated_by: config-scout
---

# j-klawson/security-gym — claude-md

**Why it's worth keeping:** It explains complex stateful logic—like the asymmetric reward mechanics and parser registration patterns—that an AI could easily break without this context. It also provides specific command-line workflows for running experiments and validation.

**Summary:** An exceptionally dense architectural map detailing how security logs are parsed, stored, and converted into reinforcement learning observations.

**Source credibility:** High; comes from a well-structured research project with recent activity.

**Recency:** Current; uses modern Python packaging and Gymnasium standards.

**Source:** [j-klawson/security-gym/CLAUDE.md](https://github.com/j-klawson/security-gym/blob/320da052480e8dd0ec985dcb99b0ab1e2f19ab94/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# security-gym

Gymnasium-compatible environment that replays labeled Linux log streams for continual learning research.

See `ROADMAP.md` for project phases and `TODO.md` for current action items.

## Architecture

- `src/security_gym/` — installable package (`pip install -e .`)
- `attacks/` — attack scripts for data generation (NOT pip-installed)
- `campaigns/` — YAML campaign configs for Isildur (ssh_brute_only, log4shell_only, recon_only, recon_ssh_log4shell, credential_stuffing_only, post_auth_only, full_killchain, redis_exploit_only, redis_killchain)
- `configs/` — YAML composition configs for StreamComposer (stream_7d_brute_only, stream_30d_heavy, stream_90d_mixed, stream_365d_realistic)
- `server/` — target VM provisioning docs, Docker Compose for vulnerable services, and eBPF collector daemon
- `data/` — runtime data directory (gitignored)
- `tests/` — pytest test suite

## Key Patterns

- **Parsers**: decorator-based registry (`@ParserRegistry.register('auth_log')`); six parsers: `auth_log`, `syslog`, `web_access`, `web_error`, `journal`, `ebpf`. Shared syslog header in `_syslog_header.py` with `parse_syslog_header()` supporting both BSD (`Feb 22 00:55:01`) and RFC 3339 (
```

</details>
