---
name: javi2327pr-hue__skills-seguridad__sa21-skill
source: https://github.com/javi2327pr-hue/skills-seguridad/blob/473a40fd3dba50a947ca4f6e2b3d923ffcbb3c1e/sa21-SKILL.md
repo: javi2327pr-hue/skills-seguridad
kind: skill
stars: 0
last_pushed: 2026-05-19T04:31:39Z
license: unknown
score: 8
domains: [security, agents-ai, cli-tools]
tags: [security-audit, autonomous-agent, risk-assessment]
curated: 2026-06-16
curated_by: config-scout
---

# javi2327pr-hue/skills-seguridad — skill

**Why it's worth keeping:** The exhaustive list of trigger phrases for proactive activation and the platform-aware logic (Full vs. Chat mode) are elite agentic design patterns.

**Summary:** An autonomous security agent that detects when a user is about to introduce new skills and performs a multi-category risk analysis.

**Source credibility:** Low repository reputation, but content demonstrates advanced reasoning and structured prompting techniques.

**Recency:** Highly current; specifically tailored to the skill/agent ecosystem of modern AI CLI tools.

**Source:** [javi2327pr-hue/skills-seguridad/sa21-SKILL.md](https://github.com/javi2327pr-hue/skills-seguridad/blob/473a40fd3dba50a947ca4f6e2b3d923ffcbb3c1e/sa21-SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: security-audit
version: "2.1"
description: >
  Activa SecurityAudit SIEMPRE que el usuario quiera verificar la seguridad
  de un skill antes de instalarlo. Úsalo ante CUALQUIERA de estas señales:
  el usuario pega texto que empieza con "---" y tiene "name:", el usuario
  adjunta un archivo .skill o .md, el usuario dice "audita este skill",
  "es seguro este skill", "puedo instalar esto", "revisa la seguridad de",
  "analiza este skill", "verifica que no sea malicioso", "escanea mis
  skills", "revisa todos mis skills instalados", "confías en este skill",
  "qué hace exactamente este skill", "me mandaron este skill", "encontré
  este skill en GitHub", "skill de la comunidad", "antes de usar este
  skill", "este skill es confiable", "quiero instalar este skill de
  terceros". También actívalo si el usuario da una URL de GitHub/repositorio
  y pregunta si puede instalar lo que hay ahí. Este skill opera de forma
  completamente autónoma — tiene su propio loop de decisión, worker de
  análisis y base de patrones de riesgo. NO esperes que el usuario pida
  explícitamente una "auditoría" — si hay un skill de por medio y hay duda
  sobre su seguridad, actívate.
---

# SecurityAud
```

</details>
