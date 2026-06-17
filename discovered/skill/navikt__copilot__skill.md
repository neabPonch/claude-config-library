---
name: navikt__copilot__skill
source: https://github.com/navikt/copilot/blob/51be240b75252a7ab3155d46482c8229b68fb2eb/skills/kafka/SKILL.md
repo: navikt/copilot
kind: skill
stars: 47
last_pushed: 2026-06-15T13:20:37Z
license: mit
score: 9
domains: [backend, event-driven]
tags: [kafka, kotlin, event-driven, nais, rapids-rivers]
curated: 2026-06-15
curated_by: config-scout
---

# navikt/copilot — skill

**Why it's worth keeping:** The distinction between 'precondition' (silent filtering) and 'validate' (contract checking) is a sophisticated pattern worth stealing. It also includes highly practical 'TestRapid' templates and shell commands for environment verification.

**Summary:** Provides highly specialized operational and coding knowledge for the Rapids & Rivers event-driven framework on the Nais platform. It includes infrastructure manifests, specific Kotlin consumer patterns, and debugging commands.

**Source credibility:** High-quality organizational documentation from Navikt with recent maintenance activity.

**Recency:** Highly current; provides modern Kotlin patterns and infrastructure standards.

**Source:** [navikt/copilot/skills/kafka/SKILL.md](https://github.com/navikt/copilot/blob/51be240b75252a7ab3155d46482c8229b68fb2eb/skills/kafka/SKILL.md) · 47★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kafka
description: Rapids & Rivers, eventdrevet arkitektur, Kafka-mønstre og schema-design for Nav-applikasjoner
license: MIT
compatibility: Kotlin/JVM application with Kafka on Nais
metadata:
  domain: backend
  tags: kafka rapids-rivers events event-driven nais
---

# Kafka & Rapids & Rivers Skill

Patterns, templates, and procedures for building event-driven systems with Kafka on Nais. Covers Rapids & Rivers framework, event schema design, and consumer/producer patterns.

## When to Use

- Setting up Kafka in a Nais application
- Implementing a Rapids & Rivers consumer (River)
- Designing event schemas
- Testing event-driven code with TestRapid
- Troubleshooting Kafka connectivity or consumer lag

## Commands

```bash
# Check Kafka env vars are present (names only, not values)
kubectl exec -it <pod> -n <namespace> -- env | grep -o '^KAFKA[^=]*'

# Verify Kafka credentials are mounted
kubectl exec -it <pod> -n <namespace> -- ls -la /var/run/secrets/nais.io/kafka/

# View pod logs for Kafka events
kubectl logs -n <namespace> <pod> --tail=50 | grep -i "event\|kafka\|river"
```

## Setting Up Kafka

### Nais Manifest

```yaml
apiVersion: nais.io/v1alpha1
kind: Application
```

</details>
