---
name: tramlinehq__store-quirks__skill
source: https://github.com/tramlinehq/store-quirks/blob/5b1f9fa9950902fd4b628c3afda72e28200ca800/store-quirks/SKILL.md
repo: tramlinehq/store-quirks
kind: skill
stars: 259
last_pushed: 2026-02-11T11:23:22Z
license: cc0-1.0
score: 8
domains: [mobile-dev, devops]
tags: [app-store, deployment, versioning]
curated: 2026-06-15
curated_by: config-scout
---

# tramlinehq/store-quirks — skill

**Why it's worth keeping:** The comparison table provides high-density, structured facts that prevent common deployment hallucinations, while the 'Usage' section establishes a clear reasoning protocol for the agent.

**Summary:** A domain-specific reference guide detailing technical discrepancies between Apple App Store and Google Play Store release management behaviors.

**Source credibility:** Strong; 259 stars indicates high community validation of its specific niche knowledge.

**Recency:** Highly current; last updated 4 months ago.

**Source:** [tramlinehq/store-quirks/store-quirks/SKILL.md](https://github.com/tramlinehq/store-quirks/blob/5b1f9fa9950902fd4b628c3afda72e28200ca800/store-quirks/SKILL.md) · 259★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: store-quirks
description: Reference guide for mobile app store quirks and undocumented behaviors across Apple App Store and Google Play Store. Use when the user asks about app store release management, phased/staged rollouts, version codes, version names, build versioning, TestFlight, App Bundle Explorer, App Store Connect API behavior, canceling submissions, removing apps from sale, or any question about how Apple App Store or Google Play Store handles releases, builds, and updates. Also use when comparing behavior between the two stores.
---

# Mobile App Store Quirks

A compiled reference of answers for common and rare situations when releasing and managing app updates across Apple App Store and Google Play Store.

## Key Differences Between Stores

| Behavior | Apple App Store | Google Play Store |
|----------|----------------|-------------------|
| New users during rollout | Always get latest build | Participate in rollout % bucket |
| Rollout user selection | New random sample each release | Sticky user group from previous release |
| Rollout time limit | 30 days max | Indefinite |
| Update build during rollout | Not possible | Yes, creates new release |
| Version N
```

</details>
