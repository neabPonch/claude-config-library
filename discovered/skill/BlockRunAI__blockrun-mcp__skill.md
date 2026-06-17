---
name: BlockRunAI__blockrun-mcp__skill
source: https://github.com/BlockRunAI/blockrun-mcp/blob/a183e21766425924f7e48ead7ac9d77913194174/skills/modal/SKILL.md
repo: BlockRunAI/blockrun-mcp
kind: skill
stars: 466
last_pushed: 2026-06-14T03:31:57Z
license: mit
score: 9
domains: [agents-ai, cloud-compute, security, dev-tools]
tags: [remote-execution, gpu, sandbox, modal, ephemeral]
curated: 2026-06-16
curated_by: config-scout
---

# BlockRunAI/blockrun-mcp — skill

**Why it's worth keeping:** Includes critical 'When NOT to Use' guardrails and provides highly structured worked examples that model the specific lifecycle needed for remote compute.

**Summary:** Provides a comprehensive lifecycle for managing ephemeral remote containers with GPU support via Modal. It covers sandbox creation, execution, and termination.

**Source credibility:** Strong; part of an active AI infrastructure repo (BlockRunAI) with recent activity.

**Recency:** Current; uses modern patterns for agentic tool-calling and container orchestration.

**Source:** [BlockRunAI/blockrun-mcp/skills/modal/SKILL.md](https://github.com/BlockRunAI/blockrun-mcp/blob/a183e21766425924f7e48ead7ac9d77913194174/skills/modal/SKILL.md) · 466★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: modal
description: Use when the user needs to run isolated code remotely — a disposable container, optional GPU access (T4 → H100), or a safer place for untrusted / heavy code. Prefer local execution for normal repo work; use Modal sandboxes for isolation, hardware access, or one-shot heavy compute.
triggers:
  - "modal sandbox"
  - "remote python"
  - "sandbox execution"
  - "isolated code run"
  - "gpu sandbox"
  - "h100"
  - "a100"
  - "remote container"
  - "ephemeral container"
  - "run untrusted code"
---

# Modal Sandboxes

Disposable remote containers (with optional GPU) via Modal, paid per call in USDC. No Modal account, no GPU procurement — pay only for what runs.

## How to Call from MCP

```ts
// 1. Create
blockrun_modal({ path: "sandbox/create", body: {
  image: "python:3.11",
  gpu: "A100",
  timeout: 600,
  setup_commands: ["pip install torch transformers"]
}})
// returns { sandbox_id, ... }

// 2. Exec
blockrun_modal({ path: "sandbox/exec", body: {
  sandbox_id: "sb_abc...",
  command: ["python", "-c", "import torch; print(torch.cuda.get_device_name(0))"]
}})

// 3. Terminate
blockrun_modal({ path: "sandbox/terminate", body: { sandbox_id: "sb_abc..." } })
```

</details>
