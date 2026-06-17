---
name: bauerpawel__Portainer_templates_v3_converter
source: https://github.com/bauerpawel/Portainer_templates_v3_converter/blob/fbfa05bb38410f2f1fef37d4834fc781cd042cc3/CLAUDE.MD
repo: bauerpawel/Portainer_templates_v3_converter
kind: claude-md
stars: 3
last_pushed: 2026-06-15T07:08:59Z
license: apache-2.0
score: 9
domains: [cli-tools, devops, data-transformation]
tags: [python, json-processing, automation]
curated: 2026-06-15
curated_by: config-scout
---

# bauerpawel/Portainer_templates_v3_converter — claude-md

**Why it's worth keeping:** The 'Format Differences' section provides explicit before/after examples which are crucial for preventing hallucinations during code modification tasks. It also details the specific algorithmic steps of the 'Main Conversion Flow'.

**Summary:** Provides exhaustive domain-specific context for a data transformation tool, including exact JSON schema changes and internal conversion logic.

**Source credibility:** Solid utility repository with active maintenance history and clear documentation.

**Recency:** Highly relevant; includes modern Python standards and current development workflows.

**Source:** [bauerpawel/Portainer_templates_v3_converter/CLAUDE.MD](https://github.com/bauerpawel/Portainer_templates_v3_converter/blob/fbfa05bb38410f2f1fef37d4834fc781cd042cc3/CLAUDE.MD) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.MD - Project Context for Claude Code

## Project Overview

**Portainer Templates Converter v2 → v3** is a Python application that automatically converts Portainer application templates from v2 format to v3 format, which is compatible with the latest versions of Portainer.io.

### Key Purpose
Convert Docker/Swarm app templates to the new Portainer v3 format which requires:
- Adding unique `id` fields
- Adding `labels` arrays
- Removing deprecated `restart_policy` and `platform` fields
- Validating against official JSON Schema

### Languages & Technologies
- **Primary**: Python 3.6+
- **Key Libraries**: `requests`, `jsonschema`
- **Format**: JSON template processing
- **Domain**: Docker, Portainer, containerization

## Project Structure

```
.
├── portainer_converter.py      # Main application (PortainerTemplateConverter class)
├── test_converter.py           # Unit tests for the converter
├── schema_v3.json              # Official Portainer v3 JSON Schema for validation
├── templates_v3_converted.json # Output file (generated after conversion)
├── requirements.txt            # Python dependencies
├── README.md                   # Documentation (Polish)
├── README.en.md
```

</details>
