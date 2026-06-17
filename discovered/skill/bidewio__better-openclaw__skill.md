---
name: bidewio__better-openclaw__skill
source: https://github.com/bidewio/better-openclaw/blob/983125bfe00f076d9a2862ce0fbb9ad7b2cdfa65/skills/rabbitmq-queue/SKILL.md
repo: bidewio/better-openclaw
kind: skill
stars: 55
last_pushed: 2026-06-15T02:02:20Z
license: other
score: 7
domains: [backend, devops, messaging]
tags: [rabbitmq, api-interaction, microservices]
curated: 2026-06-15
curated_by: config-scout
---

# bidewio/better-openclaw — skill

**Why it's worth keeping:** The inclusion of ready-to-use REST API commands allows an agent to perform system observability and debugging without needing specific AMQP clients installed.

**Summary:** Provides actionable curl commands to interact with the RabbitMQ Management API for inspection and message publishing.

**Source credibility:** Decent; 55 stars suggests a useful utility tool rather than a major enterprise standard.

**Recency:** 

**Source:** [bidewio/better-openclaw/skills/rabbitmq-queue/SKILL.md](https://github.com/bidewio/better-openclaw/blob/983125bfe00f076d9a2862ce0fbb9ad7b2cdfa65/skills/rabbitmq-queue/SKILL.md) · 55★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rabbitmq-queue
description: Message broker and queuing with RabbitMQ
version: 1.0.0
tags: [messaging, queue, broker, microservices]
---

# RabbitMQ – Message Broker

RabbitMQ is the most widely deployed open-source message broker
supporting AMQP, MQTT, and STOMP protocols.

- **GitHub**: github.com/rabbitmq/rabbitmq-server (13 000+ ⭐)
- **License**: MPL-2.0
- **Security**: VMware/Broadcom-backed. Enterprise-grade. No malware.

## Environment Variables

| Variable | Description |
|---|---|
| `{{RABBITMQ_URL}}` | Management API URL |
| `{{RABBITMQ_USER}}` | Username |
| `{{RABBITMQ_PASSWORD}}` | Password |

## Usage Examples

### List queues

```bash
curl -s -u "{{RABBITMQ_USER}}:{{RABBITMQ_PASSWORD}}" \
  "{{RABBITMQ_URL}}/api/queues"
```

### Publish a message

```bash
curl -s -X POST -u "{{RABBITMQ_USER}}:{{RABBITMQ_PASSWORD}}" \
  "{{RABBITMQ_URL}}/api/exchanges/%2f/amq.default/publish" \
  -H "Content-Type: application/json" \
  -d '{"properties":{},"routing_key":"my_queue","payload":"Hello","payload_encoding":"string"}'
```

## AI Agent Tips

- Supports multiple protocols: AMQP 0-9-1, MQTT, STOMP.
- Management plugin provides REST API and web dashboard.
- Dead letter
```

</details>
