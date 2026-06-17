---
name: SebastianHoyoss__UNbytecitoDataHack
source: https://github.com/SebastianHoyoss/UNbytecitoDataHack/blob/8e58cead776c4026d1e333e2b0d4240ce94bbe65/CLAUDE.md
repo: SebastianHoyoss/UNbytecitoDataHack
kind: claude-md
stars: 1
last_pushed: 2026-04-23T16:44:20Z
license: unknown
score: 9
domains: [agents-ai, rag, python]
tags: [multi-agent, rag, arxiv, streamlit]
curated: 2026-06-15
curated_by: config-scout
---

# SebastianHoyoss/UNbytecitoDataHack — claude-md

**Why it's worth keeping:** Excellent use of 'Design Decisions' to explain technical trade-offs (like the double-call JSON pattern) and provides explicit data schemas/prompting strategies crucial for AI context.

**Summary:** Highly detailed documentation for a multi-agent RAG system that maps out specific architectural flows and agent responsibilities.

**Source credibility:** Low star count, but highly structured content suggests a high-quality hackathon project.

**Recency:** Very current; reflects modern RAG and multi-agent development patterns.

**Source:** [SebastianHoyoss/UNbytecitoDataHack/CLAUDE.md](https://github.com/SebastianHoyoss/UNbytecitoDataHack/blob/8e58cead776c4026d1e333e2b0d4240ce94bbe65/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Reto 3: Asistente Inteligente para Artículos de Investigación

## Qué es este proyecto

MVP multiagente que permite al usuario escribir un tema o pregunta de investigación y recibe:
- Papers relevantes de ArXiv resumidos individualmente
- Análisis comparativo entre los papers seleccionados
- Síntesis del estado del arte alineada con la pregunta de investigación
- Chat RAG sobre cualquier paper encontrado (vectorizado en Pinecone), en español o inglés

---

## Cómo ejecutar

```bash
# Activar entorno virtual
source .venv/Scripts/activate   # Git Bash
# o
.venv\Scripts\activate           # cmd/PowerShell

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar app
streamlit run app.py
```

Requiere archivo `.env` en la raíz con:
```
GROQ_API_KEY=tu_api_key
GROQ_API_KEY_2=tu_segunda_api_key   # opcional, para rotación automática
PINECONE_API_KEY=tu_api_key
PINECONE_INDEX=papers-rag
```

---

## Estructura de archivos

```
├── app.py                      ← Interfaz Streamlit
├── agents/
│   ├── buscador.py             ← Busca papers en ArXiv (optimiza query con Groq antes)
│   ├── resumidor.py            ← Resume cada paper individualmente con Groq
│   ├── com
```

</details>
