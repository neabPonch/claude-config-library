---
name: 808cadger__construction-safety-ai
source: https://github.com/808cadger/construction-safety-ai/blob/e79159dc93b449ccbfee8897fc95aba1f7106067/claude.md
repo: 808cadger/construction-safety-ai
kind: claude-md
stars: 1
last_pushed: 2026-05-11T01:19:15Z
license: apache-2.0
score: 7
domains: [computer-vision, devops]
tags: [yolov8, docker, python, safety]
curated: 2026-06-15
curated_by: config-scout
---

# 808cadger/construction-safety-ai — claude-md

**Why it's worth keeping:** The 'Claude Workflow' section provides high-value instructions including specific diagnostic questions to ask the user and a structured commit message convention linked to domain features.

**Summary:** Defines a computer vision safety pipeline and establishes an agent-centric debugging and commit workflow for Dockerized Python environments.

**Source credibility:** Single-star niche repository with personal developer focus.

**Recency:** Current; utilizes modern agentic workflows for containerized services.

**Source:** [808cadger/construction-safety-ai/claude.md](https://github.com/808cadger/construction-safety-ai/blob/e79159dc93b449ccbfee8897fc95aba1f7106067/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Construction Safety AI - PPE Detection & Alert System
Production-ready construction site monitoring: YOLOv8 PPE detection (hard hats/vests/gloves), real-time alerts, violation logs. Flask web app + Docker. Multi-camera scalable.

Repo: https://github.com/808cadger/construction-safety-ai. Dev: cadger808 (Pearl City, HI).

## Stack & Safety Pipeline
- Backend: Python/Flask (PPE detection API)
- Vision: YOLOv8 + OpenCV (hard hats, vests, gloves, glasses)
- Container: Docker + docker-compose.yml
- Deploy: Production-ready multi-camera
- Alerts: Email/SMS for violations
- CI: GitHub workflows

## Key Files & Pipeline
Dockerfile | docker-compose.yml | requirements.txt | README.md | setup.py

## Commands
# Dev
pip install -r requirements.txt
python app.py  # Flask dev server

# Production
docker-compose up -d
docker-compose logs -f

## Code Rules — PPE Detection Pipeline
- **Pipeline**: Camera feed → YOLOv8 detection → PPE compliance check → Alert if violation
- **PPE Types**: Hard hats, high-vis vests, gloves, safety glasses, harnesses
- **#ASSUMPTION**: Camera calibrated; TODO: auto-calibration
- **Scoring**: Confidence thresholds per PPE type (hard hat >0.85, vest >0.75)
- **Zones**:
```

</details>
