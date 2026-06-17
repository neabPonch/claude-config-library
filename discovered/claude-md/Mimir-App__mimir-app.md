---
name: Mimir-App__mimir-app
source: https://github.com/Mimir-App/mimir-app/blob/8b409ee3c9bcb6dee6cc262efb58527c52445615/CLAUDE.md
repo: Mimir-App/mimir-app
kind: claude-md
stars: 0
last_pushed: 2026-03-31T17:58:39Z
license: unknown
score: 8
domains: [desktop-app, systems-programming, ai-agents, multi-language]
tags: [tauri, rust, python, workflow-automation]
curated: 2026-06-17
curated_by: config-scout
---

# Mimir-App/mimir-app — claude-md

**Why it's worth keeping:** Uses custom slash command definitions to instruct the AI on operational workflows and implements a structured @.claude/context pattern for scalable documentation depth.

**Summary:** A sophisticated configuration for a multi-language project (Rust, Python, TS) that defines high-level agent workflows.

**Source credibility:** Low public reputation (0 stars), appearing to be an active early-stage specialized tool.

**Recency:** Current; utilizes modern stacks like Tauri 2 and contemporary development workflows.

**Source:** [Mimir-App/mimir-app/CLAUDE.md](https://github.com/Mimir-App/mimir-app/blob/8b409ee3c9bcb6dee6cc262efb58527c52445615/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Mimir

## Descripcion
Mimir es un asistente inteligente de imputacion de horas. Captura automaticamente la actividad del empleado mediante senales (cada 30s), genera bloques bajo demanda usando un agente Claude Code CLI que analiza senales + actividad VCS + calendario, y permite imputar horas a Odoo.

**Version actual: v0.8.0**

## Stack
- **Frontend**: Tauri 2 + Vue 3 + TypeScript + Vite
- **Backend desktop**: Rust (Tauri commands)
- **Capture daemon**: Python 3.10+ (asyncio + poller + tray), puerto 9476, systemd service
- **Server daemon**: Python 3.10+ (FastAPI + uvicorn), puerto 9477, child process de Tauri
- **Base de datos**: SQLite compartida (WAL) + JSON config (Tauri)

## Comandos

```bash
# Frontend + Tauri
npm install
npm run tauri dev    # Desarrollo con hot reload

# Daemon Python
cd daemon
python -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
python -m mimir_daemon      # Arranca daemon (capture + server)
pytest tests/ -v            # Tests del daemon (~195 tests)

# Build
bash scripts/build.sh capture   # Solo capture
bash scripts/build.sh server    # Solo server
bash scripts/build.sh daemon    # Ambos + instalador
bash scripts/build.sh
```

</details>
