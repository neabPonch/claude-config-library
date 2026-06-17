---
name: Jupiter41__arthur-airport__kafka-skill
source: https://github.com/Jupiter41/arthur-airport/blob/33f9105cc98955a06b2080d388f0514e8eca2475/docs/skills/kafka.SKILL.md
repo: Jupiter41/arthur-airport
kind: skill
stars: 9
last_pushed: 2026-06-08T08:22:10Z
license: other
score: 9
domains: [backend-api, distributed-systems, data-streaming]
tags: [kafka, python, asyncio, event-driven]
curated: 2026-06-16
curated_by: config-scout
---

# Jupiter41/arthur-airport — skill

**Why it's worth keeping:** Includes essential implementation details like the 'sim_time' vs 'produced_at' distinction, async consumer loop safety (run_in_executor), and explicit idempotency patterns.

**Summary:** A highly structured skill file defining an event-driven architecture using Kafka, Python, and asyncio for a simulation environment.

**Source credibility:** High-fidelity technical specification from a specialized digital twin project with recent activity.

**Recency:** Modern; utilizes contemporary Python features like structural pattern matching.

**Source:** [Jupiter41/arthur-airport/docs/skills/kafka.SKILL.md](https://github.com/Jupiter41/arthur-airport/blob/33f9105cc98955a06b2080d388f0514e8eca2475/docs/skills/kafka.SKILL.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SKILL — Kafka
## Topics · Schemas · Producer/Consumer patterns

---

## Topic catalogue

| Topic | Producer | Key | Partitions |
|---|---|---|---|
| `sim.clock` | sim-orchestrator | — | 1 |
| `flights.schedule` | sim-orchestrator | `flight_id` | 1 |
| `flights.events` | flight-service | `flight_id` | 6 |
| `passengers.events` | passenger-service | `passenger_id` | 6 |
| `baggage.events` | baggage-service | `baggage_tag` | 6 |
| `weather.events` | weather-service | — | 1 |
| `incidents.events` | incident-service | `incident_id` | 3 |
| `incidents.alerts` | incident-service | `incident_id` | 3 |
| `incidents.inject` | api-gateway (manual) | — | 1 |

Consumer groups: `flight-svc`, `pax-svc`, `bag-svc`, `weather-svc`, `inc-svc`, `api-gateway`

Full event schemas → `docs/architecture/EVENT_BUS.md`

---

## Event envelope (every message on every topic)

```python
{
    "event_id": "uuid-v4",           # unique per event — use for dedup
    "event_type": "FlightStatusChanged",
    "schema_version": "1.0",
    "produced_at": "ISO8601",        # wall clock — do not use for business logic
    "sim_time": "ISO8601",           # simulation time — ALWAYS use this
    "producer": "flight-servi
```

</details>
