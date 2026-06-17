---
name: RodrigoOkido__SwiftUI-BaseHelper
source: https://github.com/RodrigoOkido/SwiftUI-BaseHelper/blob/991824b7dcebe421a1b96b7c00f24a2ecc7e0037/CLAUDE.md
repo: RodrigoOkido/SwiftUI-BaseHelper
kind: claude-md
stars: 4
last_pushed: 2026-06-12T18:59:23Z
license: unknown
score: 9
domains: [ios-development, swiftui]
tags: [architecture-patterns, naming-conventions, design-system]
curated: 2026-06-15
curated_by: config-scout
---

# RodrigoOkido/SwiftUI-BaseHelper — claude-md

**Why it's worth keeping:** It includes explicit naming recipes (e.g., Remote/Mapper/Repository suffixes) and a detailed project layout that helps the AI navigate without constant file-system scanning. The 'Main Rules' section also provides strong guardrails against hardcoding design tokens or creating unprompted files.

**Summary:** This file establishes a strict architectural standard for SwiftUI development using MVVM and Clean Architecture. It provides specific naming conventions, directory mapping, and code templates to ensure consistency across feature implementations.

**Source credibility:** A high-quality personal developer tool with recent maintenance and clear architectural intent.

**Recency:** Highly current, utilizing modern Swift features like @Observable and specialized Xcode project group synchronization methods.

**Source:** [RodrigoOkido/SwiftUI-BaseHelper/CLAUDE.md](https://github.com/RodrigoOkido/SwiftUI-BaseHelper/blob/991824b7dcebe421a1b96b7c00f24a2ecc7e0037/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for AI assistants (and humans) working in the **SwiftUI-BaseHelper** repository. 
SwiftUI-BaseHelper is a SwiftUI project created by Rodrigo Okido, which aims to 
explore many concepts of the Apple SwiftUI framework. Explores navigation, design system 
components, view modifiers, and so on. This document captures the architecture, 
conventions, and working agreements established so far so that new changes stay consistent 
with the existing codebase. The GitHub profile of the author is `https://github.com/RodrigoOkido/`.

---

## 1. Main Rules
1. **Mirror the existing architecture.** This project intentionally follows the
   `SwiftUI-BaseHelper` reference architecture (MVVM + Clean layering, DI,
   router-based navigation). Before adding a screen, store, or service, look at
   how an existing equivalent is built and copy that shape. Deviate only when
   there is a concrete technical reason, and call it out. 
2. **Always build before declaring done.** Compile the app and run the test
   suite (see §10). UI changes should be verified in the simulator with a
   screenshot when practical.
3. **Use the DesignSystem.** Never hardcode spacing, sizes, colors, fonts, or
```

</details>
