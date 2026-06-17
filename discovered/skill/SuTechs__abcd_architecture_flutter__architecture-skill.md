---
name: SuTechs__abcd_architecture_flutter__architecture-skill
source: https://github.com/SuTechs/abcd_architecture_flutter/blob/0059ae0bea0ede738e6ebe7235bb9f09225c3814/architecture_skill.md
repo: SuTechs/abcd_architecture_flutter
kind: skill
stars: 163
last_pushed: 2026-05-08T06:42:08Z
license: mit
score: 9
domains: [mobile-development, software-architecture]
tags: [flutter, agent-instructions, unidirectional-data-flow]
curated: 2026-06-15
curated_by: config-scout
---

# SuTechs/abcd_architecture_flutter — skill

**Why it's worth keeping:** Uses highly effective 'Do/Do Not' sections to prevent pattern drift and includes specific discovery instructions (like using `rg`) for the agent's pre-implementation phase.

**Summary:** Establishes strict layer boundaries and operational constraints specifically designed to guide AI agents in maintaining architectural integrity within a Flutter project.

**Source credibility:** Good; 163 stars indicates community validation and recent activity shows it is a living standard.

**Recency:** Very current; utilizes modern Flutter stack components like Riverpod and Freezed.

**Source:** [SuTechs/abcd_architecture_flutter/architecture_skill.md](https://github.com/SuTechs/abcd_architecture_flutter/blob/0059ae0bea0ede738e6ebe7235bb9f09225c3814/architecture_skill.md) · 163★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ABCD Architecture Guidelines for AI Agents

Provide this document as context to AI agents modifying, generating, or reviewing code within this repository. 

ABCD Architecture enforces a strict unidirectional data flow designed for scalability and maintainability. It is a foundational architecture, not a specific application template. (Note: Todo is only a reference feature).

## Architectural Flow

Implement features adhering to the following strict boundary flow:

```text
Display -> Command -> API -> Command -> Bloc -> Display
```

### Layer Definitions

- **API (`lib/data/api/`)**: Interfaces with external services and defines backend contracts.
- **Bloc (`lib/data/bloc/`)**: Manages application and feature state.
- **Command (`lib/data/command/`)**: Orchestrates user actions, side effects, and state mutations.
- **Display (`lib/screens/`)**: Renders Flutter UI components.

### Supporting Structures

- **Models (`lib/data/data/`)**: Immutable `Freezed` data classes.
- **Shared Widgets (`lib/widgets/`)**: Reusable UI components.
- **Application Shell (`lib/app/`)**: Routing, configuration, and theme definitions.

Do not introduce external architectural patterns (e.g., Clean Arch
```

</details>
