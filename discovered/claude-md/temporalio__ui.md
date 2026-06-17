---
name: temporalio__ui
source: https://github.com/temporalio/ui/blob/ccb4cb733e8285d34aa00bc9a7b52c8426ca1c0b/CLAUDE.md
repo: temporalio/ui
kind: claude-md
stars: 406
last_pushed: 2026-06-12T21:46:19Z
license: mit
score: 9
domains: [web-frontend]
tags: [svelte5, typescript, sveltekit]
curated: 2026-06-15
curated_by: config-scout
---

# temporalio/ui — claude-md

**Why it's worth keeping:** The inclusion of explicit Svelte 5 Runes examples is crucial to prevent LLMs from regressing to deprecated Svelte 4 syntax, while the import order and command mapping provide clear operational guardrails.

**Summary:** A high-quality configuration for a Svelte 5 and SvelteKit project that enforces strict coding standards and workflows.

**Source credibility:** High; Temporal is a major industry-standard engineering organization.

**Recency:** Very current; specifically addresses modern Svelte 5 patterns.

**Source:** [temporalio/ui/CLAUDE.md](https://github.com/temporalio/ui/blob/ccb4cb733e8285d34aa00bc9a7b52c8426ca1c0b/CLAUDE.md) · 406★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude AI Assistant Rules for Temporal UI

SvelteKit + Svelte 5 + TypeScript + TailwindCSS + Holocene design system

## Commands

```bash
pnpm lint              # Run all linters
pnpm check             # TypeScript type checking
pnpm test -- --run              # Run unit tests
```

## Svelte 5 Patterns

```typescript
// Props
let { class: className = '', adapter }: Props = $props();

// State
let count = $state(0);

// Computed
const doubled = $derived(count * 2);

// Effects
$effect(() => {
  console.log('Count:', count);
  return () => cleanup();
});

// SuperForms
const { form, errors, enhance } = $derived(
  superForm(data, {
    SPA: true,
    validators: zodClient(schema),
    onUpdate: async ({ form }) => {
      /* handle submit */
    },
  }),
);
```

## Import Order

1. Node.js built-ins
2. External libraries (with `svelte/**` first)
3. SvelteKit imports (`$app/**`, `$types`)
4. Internal imports (`$lib/**`)
5. Component imports (`$components/**/*.svelte`)
6. Relative imports (`./`, `../`)

## Workflow

1. **Always run linting**: Execute `pnpm lint` after making changes
2. **Type checking**: Run `pnpm check` to verify TypeScript compliance
3. **Test execution**: Run appr
```

</details>
