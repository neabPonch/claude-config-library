---
name: Djtv1304__ambacar-backend-notifications
source: https://github.com/Djtv1304/ambacar-backend-notifications/blob/2e6a9a9a4c74720a339986f8e13f32b1e8ba03ea/Claude.md
repo: Djtv1304/ambacar-backend-notifications
kind: claude-md
stars: 0
last_pushed: 2026-01-28T05:36:05Z
license: unknown
score: 9
domains: [backend-api, microservices, django]
tags: [architectural-decisions, orchestration, technical-specification]
curated: 2026-06-15
curated_by: config-scout
---

# Djtv1304/ambacar-backend-notifications — claude-md

**Why it's worth keeping:** It uses 'Decision Records' to explain the rationale behind patterns (like Slugs vs UUIDs) and provides explicit execution flows that allow an AI to understand business intent rather than just code structure.

**Summary:** A highly detailed architectural specification for a Django microservice covering domain logic, service orchestration, and infrastructure decisions.

**Source credibility:** Low social proof (0 stars), but high-density technical documentation suggests a real production environment.

**Recency:** Very current, featuring specific 2026 timelines/decisions and modern stack requirements.

**Source:** [Djtv1304/ambacar-backend-notifications/Claude.md](https://github.com/Djtv1304/ambacar-backend-notifications/blob/2e6a9a9a4c74720a339986f8e13f32b1e8ba03ea/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Context - Ambacar Notification Service

> Contexto técnico y decisiones arquitectónicas del microservicio de notificaciones multi-canal para talleres automotrices Ambacar.

---

## Resumen del Proyecto

**Ambacar Notification Service** es un microservicio Django que orquesta notificaciones multi-canal (Email, WhatsApp, Push) para el flujo de servicio automotriz de talleres Ambacar.

**Problema que resuelve:**
- Envío automático de notificaciones a clientes y staff según la fase del servicio
- Soporte para múltiples canales con fallback automático
- Configuración personalizable por tipo de servicio y taller
- Sistema de preferencias de cliente para priorizar canales

**Stack Principal:**
- Django 5.x + DRF + drf-spectacular
- PostgreSQL (Supabase)
- Celery 5.3+ (Redis broker)
- Adaptadores: SMTP, Evolution API (WhatsApp), py-webpush

---

## Arquitectura

### Patrón: Hexagonal (Ports & Adapters)

```
Core Domain (apps/core/)
├── Ports: NotificationGateway, TemplateRenderer
├── Constants: NotificationChannel, NotificationStatus, EventType
└── Authentication: InternalAPIAuthentication (service-to-service)

Notifications (apps/notifications/)
├── Models: ServicePhase, ServiceT
```

</details>
