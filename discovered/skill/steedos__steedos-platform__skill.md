---
name: steedos__steedos-platform__skill
source: https://github.com/steedos/steedos-platform/blob/53d1c566063e2c90d72d4b67cc31950a52d5a653/skills/steedos-server-internals/SKILL.md
repo: steedos/steedos-platform
kind: skill
stars: 1561
last_pushed: 2026-06-12T17:32:17Z
license: agpl-3.0
score: 9
domains: [backend-architecture, microservices, real-time-systems]
tags: [nestjs, moleculer, event-driven, architectural-map]
curated: 2026-06-15
curated_by: config-scout
---

# steedos/steedos-platform — skill

**Why it's worth keeping:** The use of 'TRIGGER' and 'SKIP' directives is a top-tier technique for controlling agent scope. It also maps critical event-driven flows between microservices, WebSockets, and the database.

**Summary:** Provides a high-density architectural mental model for a complex NestJS and Moleculer hybrid microservice environment.

**Source credibility:** High; part of an established open-source enterprise platform with significant GitHub traction.

**Recency:** Very current, referencing NestJS 11 and modern architectural patterns.

**Source:** [steedos/steedos-platform/skills/steedos-server-internals/SKILL.md](https://github.com/steedos/steedos-platform/blob/53d1c566063e2c90d72d4b67cc31950a52d5a653/skills/steedos-server-internals/SKILL.md) · 1561★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: steedos-server-internals
description: |
  Steedos Server internal architecture: NestJS 11 + Moleculer 0.14 hybrid.
  TRIGGER: NestJS module organization; Moleculer broker (namespace, transporter,
  cacher, serializer); AppMoleculer events ($packages.changed, $metadata.*,
  @objectRecordEvent); Socket.IO AppGateway, WebSocket rooms; bootstrap sequence,
  middleware, guards, dependency injection; broker.call, broker.emit;
  edition system, @builder6/* ecosystem.
  SKIP: use REST API → steedos-server-api or steedos-builder6-api;
  configure server → steedos-configuration; Builder6 internals →
  steedos-builder6-internals; overview → steedos-getting-started.
---

# Steedos Server Architecture | Steedos 服务端架构

## Overview | 概述

Steedos Server (`builder6/server`) is a NestJS + Moleculer hybrid backend. NestJS handles HTTP/REST, Moleculer handles microservice orchestration, and Socket.IO provides real-time communication.

## Technology Stack | 技术栈

- **HTTP Framework**: NestJS 11 (Express adapter)
- **Microservices**: Moleculer 0.14
- **Real-time**: Socket.IO via `@nestjs/websockets`
- **Database**: MongoDB 3.7 via `@steedos/objectql`
- **Session Store**: Redis via `connect-redi
```

</details>
