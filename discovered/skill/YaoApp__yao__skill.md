---
name: YaoApp__yao__skill
source: https://github.com/YaoApp/yao/blob/1824e3d1015fbb043535f4997610552b6d8dbf82/tools/secret/SKILL.md
repo: YaoApp/yao
kind: skill
stars: 7543
last_pushed: 2026-06-10T09:37:29Z
license: other
score: 8
domains: [security, cli-tools, agents-ai]
tags: [secrets-management, security-protocols, tool-documentation]
curated: 2026-06-15
curated_by: config-scout
---

# YaoApp/yao — skill

**Why it's worth keeping:** The 'Security Rules' section is a gold-standard template for preventing data leakage in agentic workflows. It also provides multi-language implementation patterns that reduce ambiguity for the LLM.

**Summary:** Provides a structured framework for an agent to interact with a secure secret management CLI tool.

**Source credibility:** High; YaoApp is a highly-starred, actively maintained project.

**Recency:** Current; aligns with modern security requirements for AI agent tool-calling.

**Source:** [YaoApp/yao/tools/secret/SKILL.md](https://github.com/YaoApp/yao/blob/1824e3d1015fbb043535f4997610552b6d8dbf82/tools/secret/SKILL.md) · 7543★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Secret Management

Agents can read user-configured secrets at runtime using the `tai tool` CLI.
Secrets are encrypted at rest (AES-256-GCM) and decrypted only when read.

## Available Tools

| Tool | Description |
|------|-------------|
| `secret_list` | List secret names and descriptions (no values) |
| `secret_read` | Read a single secret value by name |

## Usage

### Bash

```bash
# List available secrets
tai tool secret_list

# Read a secret
TOKEN=$(tai tool secret_read '{"name": "GITHUB_TOKEN"}' | jq -r '.value')
git clone "https://${TOKEN}@github.com/org/repo.git"
```

### Node.js

```javascript
const { execSync } = require("child_process");

function readSecret(name) {
  const raw = execSync(
    `tai tool secret_read '${JSON.stringify({ name })}'`,
    { encoding: "utf-8" }
  );
  return JSON.parse(raw).value;
}

const token = readSecret("GITHUB_TOKEN");
```

### Python

```python
import json
import subprocess

def read_secret(name: str) -> str:
    result = subprocess.run(
        ["tai", "tool", "secret_read", json.dumps({"name": name})],
        capture_output=True, text=True, check=True,
    )
    return json.loads(result.stdout)["value"]

token = read_secret("GITHUB
```

</details>
