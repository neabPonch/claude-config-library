---
name: Emifacio__gymAppBack
source: https://github.com/Emifacio/gymAppBack/blob/4c892cdce6bbca0005d67e541624a4e03cebd200/skill.md
repo: Emifacio/gymAppBack
kind: skill
stars: 25
last_pushed: 2026-06-04T14:22:11Z
license: mit
score: 7
domains: [devops, backend-api]
tags: [fastapi, railway, docker, celery]
curated: 2026-06-15
curated_by: config-scout
---

# Emifacio/gymAppBack — skill

**Why it's worth keeping:** Uses a rigorous 'Validate -> Configure -> Deploy -> Verify -> Debug' pattern; emphasizes critical PaaS requirements like dynamic port handling via $PORT.

**Summary:** Provides a structured DevOps workflow for deploying a FastAPI stack (including Celery/Redis) to the Railway platform.

**Source credibility:** Low star count, but highly specific and practical repository purpose.

**Recency:** Highly current, utilizing modern Python/FastAPI patterns.

**Source:** [Emifacio/gymAppBack/skill.md](https://github.com/Emifacio/gymAppBack/blob/4c892cdce6bbca0005d67e541624a4e03cebd200/skill.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Untitled

# Agent Skill: Deploy FastAPI Backend to Railway

You are an expert DevOps engineer.

Your task is to **prepare and deploy a FastAPI backend to Railway successfully**.

The backend uses the following stack:

```
Python
FastAPI
PostgreSQL
Redis
Celery
```

The goal is to ensure the project **deploys successfully on Railway without build failures**.

---

# Step 1 — Validate Project Structure

Ensure the repository follows this structure:

```
project-root/
│
├ app/
│   ├ main.py
│   ├ api/
│   ├ services/
│   ├ repositories/
│   └ models/
│
├ requirements.txt
├ Dockerfile
├ .env.example
├ README.md
└ railway.json (optional)
```

The FastAPI application must be defined in:

```
app/main.py
```

Example:

```
fromfastapiimportFastAPI

app=FastAPI()

@app.get("/")
defhealth():
return {"status":"ok"}
```

---

# Step 2 — Validate Dependencies

Ensure `requirements.txt` includes at least:

```
fastapi
uvicorn[standard]
sqlalchemy
psycopg2-binary
redis
celery
python-dotenv
alembic
pydantic
```

If Celery or Redis are used, include them as dependencies.

---

# Step 3 — Configure Server Start Command

Railway requires the application to listen on the **PORT environment variable
```

</details>
