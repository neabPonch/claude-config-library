---
name: KDZMEDIABOT__KDZMEDIABOT__claude
source: https://github.com/KDZMEDIABOT/KDZMEDIABOT/blob/2ee1ddfb520516f649dba1a69165bebb9b813834/KDZJAVACORE/CLAUDE.md
repo: KDZMEDIABOT/KDZMEDIABOT
kind: claude-md
stars: 4
last_pushed: 2026-06-14T17:23:08Z
license: mit
score: 9
domains: [devops, infrastructure, deployment, backend-api]
tags: [environment-context, strict-constraints, operational-runbooks]
curated: 2026-06-15
curated_by: config-scout
---

# KDZMEDIABOT/KDZMEDIABOT — claude-md

**Why it's worth keeping:** The 'Beware' section provides high-value negative constraints to prevent environmental errors, and the inclusion of exact SSH/Docker debugging commands is a top-tier pattern.

**Summary:** Extremely detailed operational context including network topology for 'rig1.lan', service dependencies, and remote monitoring commands.

**Source credibility:** Active repository with recent activity and niche specialization.

**Recency:** Highly current; reflects modern DevOps and containerized deployment workflows.

**Source:** [KDZMEDIABOT/KDZMEDIABOT/KDZJAVACORE/CLAUDE.md](https://github.com/KDZMEDIABOT/KDZMEDIABOT/blob/2ee1ddfb520516f649dba1a69165bebb9b813834/KDZJAVACORE/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI Content Generator System

## Production Environment (rig1.lan)

Current production deployment is on `rig1.lan`:
- **Frontend**: http://rig1.lan:8088 (nginx serving SPA)
- **Auth Service**: http://rig1.lan:3002 (Node.js/Passport.js sidecar)
- **Backend**: http://rig1.lan:8443 (Spring Boot Java, deployed outside Docker via `tools/redeploy_backend_prod_nodockerjava.sh`)
- **PostgreSQL**: rig1.lan:5432 (port 15432 externally exposed)
- **Redis**: rig1.lan:6379 (used for session storage)

### Critical Production Configuration (`.env.prod`)

```bash
# URLs must use rig1.lan, NOT localhost
AUTH_SERVICE_FRONTEND_URL=http://rig1.lan:8088
AUTH_SERVICE_PUBLIC_URL=http://rig1.lan:3002
FRONTEND_URL=http://rig1.lan:8088
SERVER_PROFILE=prod
AUTH_SERVICE_SESSION_SECRET=<strong-random-secret>
AUTH_SERVICE_HTTPD_PORT=3002
AUTH_SESSION_STORE=redis
AUTH_SERVICE_REDIS_URL=redis://redis:6379
AUTH_SERVICE_REDIS_PREFIX=aisystem:auth:sess:
```

### Production Container Status

```bash
# Check running containers
sudo ssh -o PasswordAuthentication=false -i /home/rig1_ubuntu16_root root@rig1.lan -c "docker ps --format 'table {{.Names}}\t{{.Status}}\t{{.Ports}}'"

# View auth service logs
sudo ssh -o Pass
```

</details>
