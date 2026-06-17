---
name: mentilead__shopify-app-skill__shopify-app-skill
source: https://github.com/mentilead/shopify-app-skill/blob/f2cd56ef17b030d9d2504416989c5da6dc38115c/shopify-app-skill.md
repo: mentilead/shopify-app-skill
kind: skill
stars: 3
last_pushed: 2026-03-08T16:47:25Z
license: mit
score: 9
domains: [web-development, ecommerce, cloud-infrastructure]
tags: [shopify, react-router, aws, fullstack]
curated: 2026-06-15
curated_by: config-scout
---

# mentilead/shopify-app-skill — skill

**Why it's worth keeping:** The 'Critical Gotchas' section provides highly specific, pattern-based solutions for complex issues like iframe breakout navigation, loader race conditions, and Cloud-Front CSRF failures.

**Summary:** A specialized skill profile for building embedded Shopify apps using React Router v7 and AWS infrastructure.

**Source credibility:** While the star count is low, the technical depth of the failure patterns indicates genuine production experience.

**Recency:** Very current; includes React Router v7 and modern Shopify API patterns.

**Source:** [mentilead/shopify-app-skill/shopify-app-skill.md](https://github.com/mentilead/shopify-app-skill/blob/f2cd56ef17b030d9d2504416989c5da6dc38115c/shopify-app-skill.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Shopify App Development Skill

## Activation & Scope

This skill applies when building **embedded Shopify apps** using:
- React Router v7 (Shopify Remix template / `@shopify/shopify-app-react-router`)
- Shopify Polaris UI components
- Shopify GraphQL Admin API
- DynamoDB (single-table design)
- AWS Lambda + API Gateway v2 + CloudFront
- AWS CDK for infrastructure

Use this as an actionable reference for architecture decisions, code patterns, and gotchas. Every pattern here is production-tested.

---

## CRITICAL GOTCHAS (Top 10)

Read this section first. These are the highest-value lessons — each one cost hours to debug.

### 1. Never Use Polaris `url` Prop for Internal Navigation

Polaris `<Link url="...">` and `<Button url="...">` render plain `<a>` tags. Inside Shopify's embedded app iframe, these navigate to the raw app URL (CloudFront/tunnel domain), breaking out of the admin iframe.

```tsx
// WRONG — breaks out of iframe
<Button url="/app/pricing">Upgrade</Button>
<Link url="/app/settings">Settings</Link>

// CORRECT — stays in iframe
const navigate = useNavigate();
<Button onClick={() => navigate('/app/pricing')}>Upgrade</Button>

// OK — external URLs are fine with url p
```

</details>
