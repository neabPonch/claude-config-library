---
name: ashmitahaldar__the-last-cartographer
source: https://github.com/ashmitahaldar/the-last-cartographer/blob/8f15d993927abcd8bf31f48bf57b2908f3e5cabe/CLAUDE.md
repo: ashmitahaldar/the-last-cartographer
kind: claude-md
stars: 0
last_pushed: 2026-05-09T15:03:05Z
license: unknown
score: 9
domains: [game-dev, ai-agents, backend-api]
tags: [roadmap, prompt-engineering, state-management, hackathon]
curated: 2026-06-15
curated_by: config-scout
---

# ashmitahaldar/the-last-cartographer — claude-md

**Why it's worth keeping:** The inclusion of 'Coding agent prompts' within the roadmap is a masterstroke, and providing explicit data schemas (like the NPC state) prevents hallucinated logic.

**Summary:** A highly tactical roadmap that uses a checklist to track build phases and provides specific prompts for the agent to execute each task.

**Source credibility:** Low social proof (0 stars), but contains high-density, complex technical detail characteristic of an actual project.

**Recency:** Extremely current; highly optimized for agentic workflows used today.

**Source:** [ashmitahaldar/the-last-cartographer/CLAUDE.md](https://github.com/ashmitahaldar/the-last-cartographer/blob/8f15d993927abcd8bf31f48bf57b2908f3e5cabe/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — The Last Cartographer

### AI NPC Visual Novel | Hackathon Project

---

## Current Build Phase

**Phase 0 — Pre-Hackathon Setup**

- [ ] Ren'Py project initialized ✓
- [ ] Backend folder scaffolded
- [ ] API keys in `.env.local`
- [ ] Vercel project created and connected
- [ ] Mara reference art generated for Fal
- [ ] Story bible written ✓ (see `mara_story_bible.md`)

> **Update this section as phases complete.** Coding agents should read this first to know where work left off.

Phase 1 — Hour 0–1 | Skeleton
Goal: Ren'Py game runs, backend responds with dummy data

Scaffold Next.js backend with npx create-next-app
Create /api/chat route that returns hardcoded JSON
Build Ren'Py skeleton: title screen → town scene → input box → display response
Confirm Ren'Py requests.post() reaches Vercel endpoint
Deploy backend to Vercel

Coding agent prompt:

"Create a Next.js 14 App Router API route at /api/chat that accepts POST with {input, npc_state, history} and returns a hardcoded JSON object matching this schema: [paste schema]. Include CORS headers."

Phase 2 — Hour 1–2 | Live Gemini Integration
Goal: Real NPC responses printing to screen

Wire Gemini 1.5 Pro into /api/chat
```

</details>
