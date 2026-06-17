---
name: tinykit-studio__tinykit
source: https://github.com/tinykit-studio/tinykit/blob/617db3416af227451e18de1f84394888679cf766/claude.md
repo: tinykit-studio/tinykit
kind: claude-md
stars: 500
last_pushed: 2026-01-09T05:55:36Z
license: mit
score: 9
domains: [web-frontend, fullstack-development]
tags: [svelte-5, runes, syntax-enforcement, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# tinykit-studio/tinykit — claude-md

**Why it's worth keeping:** Uses highly effective 'Wrong vs Right' diffs for breaking syntax changes and prescribes specific MCP tool usage to ensure code correctness.

**Summary:** Enforces strict Svelte 5 rune syntax and provides a comprehensive architectural blueprint including database schemas and routing logic.

**Source credibility:** High; comes from a popular (500 stars) and active open-source project.

**Recency:** Very current, specifically addressing Svelte 5 which is the modern standard.

**Source:** [tinykit-studio/tinykit/claude.md](https://github.com/tinykit-studio/tinykit/blob/617db3416af227451e18de1f84394888679cf766/claude.md) · 500★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# tinykit - Claude Code Documentation

## ⚠️ CRITICAL: SVELTE 5 ONLY

**THIS PROJECT USES SVELTE 5 WITH RUNES. YOU MUST ALWAYS:**

1. **Use `$state()` for reactive variables** - NOT `let foo = 'bar'`

   ```svelte
   ❌ WRONG: let count = 0
   ✅ RIGHT: let count = $state(0)
   ```

2. **Use `$props()` for component props** - NOT `export let`

   ```svelte
   ❌ WRONG: export let title = ''
   ✅ RIGHT: let { title = '' } = $props()
   ```

3. **Use `watch` from runed for watching prop changes** - NOT `$effect()`

   ```svelte
   ❌ WRONG: $effect(() => { if (target_field) doSomething() })
   ✅ RIGHT: watch(() => target_field, (value) => { if (value) doSomething() })
   ```

   - Import: `import { watch } from "runed"`
   - Use `watch` when reacting to specific prop/state changes
   - Use `$effect()` only for setup/cleanup side effects (e.g., event listeners)

4. **Use `$derived()` for computed values** - NOT `$:` assignments

   ```svelte
   ❌ WRONG: $: doubled = count * 2
   ✅ RIGHT: let doubled = $derived(count * 2)
   ```

5. **Use `onclick={handler}` NOT `on:click={handler}`**

   ```svelte
   ❌ WRONG: <button on:click={handler}>Click</button>
   ✅ RIGHT: <button onclick={handler}>
```

</details>
