---
name: Hiksang__perpdex
source: https://github.com/Hiksang/perpdex/blob/0ac95e151bd83fcdceed0fdecad93f0dbdbe555e/claude.md
repo: Hiksang/perpdex
kind: claude-md
stars: 0
last_pushed: 2026-01-13T08:20:58Z
license: apache-2.0
score: 9
domains: [fintech, crypto, fullstack]
tags: [realtime-data, arbitrage]
curated: 2026-06-15
curated_by: config-scout
---

# Hiksang/perpdex — claude-md

**Why it's worth keeping:** Uses a 'Claude Skills' mapping technique to organize documentation paths and provides granular WebSocket/API details to eliminate guesswork.

**Summary:** A high-density technical manual for a real-time arbitrage platform that maps complex exchange integrations and API structures.

**Source credibility:** Low social proof but contains professional-grade, high-density project intelligence.

**Recency:** Extremely current, referencing modern tech like React 19 and Tailwind 4.

**Source:** [Hiksang/perpdex/claude.md](https://github.com/Hiksang/perpdex/blob/0ac95e151bd83fcdceed0fdecad93f0dbdbe555e/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PerpDEX - Funding Rate Arbitrage Platform

## Project Overview
DEX 및 CEX 간 펀딩레이트와 가격 차이를 활용한 차익거래 플랫폼. 5개의 DEX(Hyperliquid, Pacifica, Lighter, Extended, Variational)와 5개의 CEX(Binance, OKX, Bybit, Gate.io, Bitget)에서 실시간 펀딩레이트 및 가격을 수집하고 차익거래 기회를 탐지한다.

## Tech Stack

### Backend
- **Framework**: FastAPI (Python 3.11+)
- **Database**: PostgreSQL (asyncpg, SQLAlchemy 2.0)
- **Cache**: Redis
- **Migration**: Alembic

### Frontend
- **Framework**: Next.js 16 (React 19)
- **Styling**: Tailwind CSS 4
- **Charts**: Recharts, Lightweight Charts
- **State**: TanStack React Query
- **WebSocket**: Native WebSocket (실시간 데이터 스트리밍)
- **HTTP**: Axios

## Project Structure
```
perpdex/
├── src/                    # Python 백엔드
│   ├── api/                # FastAPI 라우터
│   ├── adapters/           # DEX/CEX 어댑터
│   │   ├── base.py         # 베이스 어댑터
│   │   ├── hyperliquid.py
│   │   ├── pacifica.py
│   │   ├── lighter.py
│   │   ├── extended.py
│   │   ├── variational.py
│   │   └── cex/            # CEX 어댑터
│   │       ├── base.py
│   │       ├── binance.py
│   │       ├── okx.py
│   │       ├── bybit.py
│   │       ├── gateio.py
│   │       └── bitget.py
│   ├── core/               # 모델, 스키마, 예외
│
```

</details>
