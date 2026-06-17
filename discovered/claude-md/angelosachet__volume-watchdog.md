---
name: angelosachet__volume-watchdog
source: https://github.com/angelosachet/volume-watchdog/blob/5eb3fb68446a66e25b54a50fd5faf793a504879e/claude.md
repo: angelosachet/volume-watchdog
kind: claude-md
stars: 0
last_pushed: 2026-05-11T17:44:39Z
license: unknown
score: 7
domains: [backend-api, devops-tools, monitoring]
tags: [fastapi, docker, system-monitoring]
curated: 2026-06-15
curated_by: config-scout
---

# angelosachet/volume-watchdog — claude-md

**Why it's worth keeping:** Provides explicit logic breakdowns for complex tasks (like the URL extraction process) and precise environment variable/schema mappings that minimize agent guesswork.

**Summary:** A highly detailed technical specification for a FastAPI service that monitors Docker volume usage and file distributions.

**Source credibility:** Low social proof; likely a personal or small-scale utility project.

**Recency:** Current, utilizing modern Python standards like Pydantic and FastAPI.

**Source:** [angelosachet/volume-watchdog/claude.md](https://github.com/angelosachet/volume-watchdog/blob/5eb3fb68446a66e25b54a50fd5faf793a504879e/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Como este sistema funciona

Este projeto e uma API **FastAPI** para monitorar uso de disco de instalacoes (volumes Docker) e guardar historico no Postgres.

## Fluxo principal

1. Na inicializacao, a API executa `init_db()` e garante schema.
2. Em `POST /collect`, o coletor:
   - procura instalacoes com pasta `volumes/` dentro de `ROOT_PATHS` ate `SCAN_DEPTH`
   - mede cada volume com `du -sb`
   - calcula uso por tipo de arquivo (fotos, videos, audios, textos, outros)
   - tenta extrair `BACKEND_URL` de `docker-compose.yml`/`.env`
3. Persiste um novo `run_id` com dados agregados e detalhados no banco.

## Endpoints principais

- `GET /health`
- `POST /collect`
- `GET /runs`
- `GET /usage/latest`
- `GET /usage/latest/summary`
- `GET /usage/latest/file-types`
- `GET /usage/latest/file-types/by-url?url=...`

## Componentes

- `app/collector.py`: descoberta de instalacoes e coleta.
- `app/main.py`: API e consultas.
- `app/database.py`: conexao e criacao de tabelas.
- `scripts/run_api.py` e `scripts/run_collection.py`: execucao via script/cron.

## Estrutura

```
size-manager/
├── app/
│   ├── main.py        # rotas FastAPI
│   ├── collector.py   # descoberta + medicao + categorizaca
```

</details>
