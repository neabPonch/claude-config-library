---
name: mrgeoffrich__mini-infra
source: https://github.com/mrgeoffrich/mini-infra/blob/6c8f34646d901e610a033e3a39cff93429e259c3/CLAUDE.md
repo: mrgeoffrich/mini-infra
kind: claude-md
stars: 3
last_pushed: 2026-06-12T22:22:05Z
license: mit
score: 9
domains: [devops, cli-tools, containerization, infrastructure]
tags: [git-worktree, vm-orchestration, environment-discovery, pnpm]
curated: 2026-06-15
curated_by: config-scout
---

# mrgeoffrich/mini-infra — claude-md

**Why it's worth keeping:** The use of 'environment-details.xml' as a single source of truth for dynamic port discovery is an elite pattern for AI agents. The explicit instructions on workspace-specific constraints (pnpm vs npm) prevent common dependency errors.

**Summary:** A highly technical guide for managing a complex development environment using git worktrees and isolated VMs. It details exact CLI commands for spinning up/tearing down environments and resolving dynamic service ports.

**Source credibility:** High; the repo is actively maintained and features a highly sophisticated, engineered developer experience.

**Recency:** Very current; it utilizes modern toolchains like pnpm and specifically references Claude Code's 'skill' architecture.

**Source:** [mrgeoffrich/mini-infra/CLAUDE.md](https://github.com/mrgeoffrich/mini-infra/blob/6c8f34646d901e610a033e3a39cff93429e259c3/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Mini Infra - Claude Code Context

Important: When making changes, if we are on main branch, switch to a branch. All changes should not go into main unless the user specifically mentions they want the changes on main.

All changes should be submitted as PRs when they are ready.

## Planning Guidelines

After the first round of exploration and planning try to do more exploration for flow on effects.

When designing the solution make sure you pick a DRY and well though out solution to reduce duplication and keep the code base maintainable.

## Worktree Development Workflow

For parallel dev work, each git worktree runs its own fully isolated Mini Infra instance on its own VM. This is the default flow — use it instead of fighting over a single dev daemon when you have multiple WIPs in flight. The VM driver is auto-selected per platform: **Colima** on macOS, **WSL2** on Windows. Override via the `MINI_INFRA_DRIVER` env var (`colima` or `wsl`).

The whole flow is driven by a single CLI — `pnpm worktree-env <command>` — defined in [deployment/development/worktree-env.ts](deployment/development/worktree-env.ts). The same commands work on macOS, Linux, and Windows; there are no platform-s
```

</details>
