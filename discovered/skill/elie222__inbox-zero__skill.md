---
name: elie222__inbox-zero__skill
source: https://github.com/elie222/inbox-zero/blob/fc2f59402d46427fb441eb94e109fd159d528d92/.claude/skills/ui-components/SKILL.md
repo: elie222/inbox-zero
kind: skill
stars: 11273
last_pushed: 2026-06-14T19:55:28Z
license: other
score: 7
domains: [web-frontend, ui-ux]
tags: [shadcn, tailwind, swr, react]
curated: 2026-06-15
curated_by: config-scout
---

# elie222/inbox-zero — skill

**Why it's worth keeping:** Includes specific CLI commands for component installation and repeatable code patterns for loading states and form inputs.

**Summary:** Provides strict technical guidelines for UI development using Shadcn, Tailwind, and SWR data fetching.

**Source credibility:** High; sourced from a highly-starred (11k+) open-source project.

**Recency:** 

**Source:** [elie222/inbox-zero/.claude/skills/ui-components/SKILL.md](https://github.com/elie222/inbox-zero/blob/fc2f59402d46427fb441eb94e109fd159d528d92/.claude/skills/ui-components/SKILL.md) · 11273★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ui-components
description: UI component and styling guidelines using Shadcn UI, Radix UI, and Tailwind
---
# UI Components and Styling

## UI Framework
- Use Shadcn UI and Tailwind for components and styling
- Implement responsive design with Tailwind CSS using a mobile-first approach
- Use `next/image` package for images

## Install new Shadcn components

```sh
pnpm dlx shadcn@latest add COMPONENT
```

Example:

```sh
pnpm dlx shadcn@latest add progress
```

## Data Fetching with SWR
For API get requests to server use the `swr` package:

```typescript
const searchParams = useSearchParams();
const page = searchParams.get("page") || "1";
const { data, isLoading, error } = useSWR<PlanHistoryResponse>(
  `/api/user/planned/history?page=${page}`
);
```

## Loading Components
Use the `LoadingContent` component to handle loading states:

```tsx
<Card>
  <LoadingContent loading={isLoading} error={error}>
    {data && <MyComponent data={data} />}
  </LoadingContent>
</Card>
```

## Form Components
### Text Inputs
```tsx
<Input
  type="email"
  name="email"
  label="Email"
  registerProps={register("email", { required: true })}
  error={errors.email}
/>
```

### Text Area
```tsx
<
```

</details>
