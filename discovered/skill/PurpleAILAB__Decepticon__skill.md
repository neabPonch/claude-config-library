---
name: PurpleAILAB__Decepticon__skill
source: https://github.com/PurpleAILAB/Decepticon/blob/821f11c0d7b1380b957ec7e71f4f9e5d2e0e63dd/packages/decepticon/decepticon/skills/standard/analyst/prototype-pollution/SKILL.md
repo: PurpleAILAB/Decepticon
kind: skill
stars: 4389
last_pushed: 2026-06-16T16:28:28Z
license: apache-2.0
score: 9
domains: [security, web-exploitation, javascript, backend]
tags: [prototype-pollution, rce, red-team, node-js]
curated: 2026-06-17
curated_by: config-scout
---

# PurpleAILAB/Decepticon — skill

**Why it's worth keeping:** It includes specific grep/jq commands for dependency auditing, identifies critical 'gadget' patterns like child_process.spawn, and provides success signals crucial for autonomous verification.

**Summary:** This skill provides a specialized playbook for hunting JavaScript prototype pollution by mapping vulnerable libraries, audit workflows, and exploitation gadgets. It enables an agent to move from vulnerability discovery to high-impact proof-of-concept.

**Source credibility:** High; the Decepticon repo is a well-regarded red-teaming toolset with significant community traction.

**Recency:** Highly current, referencing 2023-2026 vulnerability meta-trends and modern Node.js patterns.

**Source:** [PurpleAILAB/Decepticon/packages/decepticon/decepticon/skills/standard/analyst/prototype-pollution/SKILL.md](https://github.com/PurpleAILAB/Decepticon/blob/821f11c0d7b1380b957ec7e71f4f9e5d2e0e63dd/packages/decepticon/decepticon/skills/standard/analyst/prototype-pollution/SKILL.md) · 4389★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: prototype-pollution
description: Hunt JavaScript prototype pollution (CWE-1321) — the 2023-2026 meta-vulnerability that chains into RCE, auth bypass, and SSRF on most Node.js stacks.
metadata:
  subdomain: web-exploitation
  when_to_use: "javascript prototype pollution cwe-1321 node js __proto__ constructor chain rce auth bypass ssrf gadget"
---

# Prototype Pollution Playbook

Prototype pollution is the JavaScript equivalent of a universal gadget:
plant a property on `Object.prototype` and it appears on every object in
the runtime. Worthless in isolation, deadly in chain (`__proto__.isAdmin
= true` → auth bypass; `__proto__.shell = "/bin/bash"` → RCE via `spawn`).

## 1. Sinks — the libraries that still introduce sinks

Keep a running list per engagement. These continue to ship sinks in 2026:

- **Deep-merge:** `lodash.merge`, `deepmerge` (pre-fix), `merge-deep`, `deepExtend`, `hoek.merge`, `mixme`
- **Deep-clone:** `lodash.defaultsDeep`, `lodash.zipObjectDeep`, `set-value` (pre-3.0.3)
- **URL-to-obj:** `qs`, `express-fileupload`, `jquery.extend(true, ...)`
- **Config loaders:** `node-config` recursive merge, `dotenv-extended`, `rc`
- **Template engines:** Handlebars hel
```

</details>
