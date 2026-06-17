---
name: AnandPilania__eloquentjs__realtime-skill
source: https://github.com/AnandPilania/eloquentjs/blob/f301b946c59fb2b5d70aa19d8d6e931787b1dc56/agent-files/skills/realtime-skill.md
repo: AnandPilania/eloquentjs
kind: skill
stars: 72
last_pushed: 2026-05-05T07:48:47Z
license: unknown
score: 9
domains: [backend-api, realtime]
tags: [websocket, broadcasting, eloquentjs]
curated: 2026-06-15
curated_by: config-scout
---

# AnandPilania/eloquentjs — skill

**Why it's worth keeping:** It offers clear end-to-end code examples for both server-side triggers—including automated model hooks—and client-side listeners. The pattern for securing private channels via auth handlers is highly specific and implementation-ready.

**Summary:** Provides complete instructions for implementing WebSocket-based real-time functionality using @eloquentjs/realtime. It covers model lifecycle broadcasting, private channel authorization, and client-side subscription patterns.

**Source credibility:** Solid; 72 stars on a specialized monorepo with recent activity.

**Recency:** Current; utilizes modern JavaScript/ESM standards relevant to contemporary development environments.

**Source:** [AnandPilania/eloquentjs/agent-files/skills/realtime-skill.md](https://github.com/AnandPilania/eloquentjs/blob/f301b946c59fb2b5d70aa19d8d6e931787b1dc56/agent-files/skills/realtime-skill.md) · 72★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# EloquentJS Realtime Skill

## When to use this skill
Use when adding WebSocket-based real-time functionality to an EloquentJS project using `@eloquentjs/realtime`.

---

## Installation

```bash
npm install @eloquentjs/core @eloquentjs/realtime ws
```

---

## Server Setup

```js
import { createRealtimeServer } from '@eloquentjs/realtime'

const rt = createRealtimeServer({
  port:         6001,        // WebSocket port (default: 6001)
  appKey:       'my-app-key',
  appSecret:    'my-secret', // for private channel auth
  pingInterval: 30_000,      // heartbeat interval in ms
})

// Always close cleanly on shutdown — clears ping timer
process.on('SIGTERM', () => rt.close())
process.on('SIGINT',  () => rt.close())
```

---

## Broadcasting Model Events

```js
// Auto-broadcast all lifecycle events for a model
rt.broadcastFrom(User)
// Broadcasts on channels: 'users'
// Events: 'created', 'updated', 'deleted'

// Custom channel name
rt.broadcastFrom(Post, { channel: 'blog-posts' })

// Filter which events to broadcast
rt.broadcastFrom(Order, {
  events: ['created', 'updated'],
})

// Transform the payload before broadcasting
rt.broadcastFrom(User, {
  transform: (user) => ({
    id
```

</details>
