---
name: dart-lang__site-www__skill
source: https://github.com/dart-lang/site-www/blob/5cc8bf11fca25a00d13cf6bc197f8ab30dc089ac/.agents/skills/update-whats-new/SKILL.md
repo: dart-lang/site-www
kind: skill
stars: 1034
last_pushed: 2026-06-15T22:41:15Z
license: other
score: 9
domains: [documentation, git-automation, content-management]
tags: [changelog, markdown, automated-updates]
curated: 2026-06-16
curated_by: config-scout
---

# dart-lang/site-www — skill

**Why it's worth keeping:** It utilizes high-quality negative constraints (Do NOT include) with concrete examples to filter noise, and provides precise structural instructions for complex Markdown linking patterns.

**Summary:** Automates the update of a 'What's New' documentation page by analyzing git commits between release dates and applying specific formatting rules.

**Source credibility:** High; maintained by the official Dart/Google team in a highly active repository.

**Recency:** Current; follows modern git-driven documentation workflows suitable for agentic automation.

**Source:** [dart-lang/site-www/.agents/skills/update-whats-new/SKILL.md](https://github.com/dart-lang/site-www/blob/5cc8bf11fca25a00d13cf6bc197f8ab30dc089ac/.agents/skills/update-whats-new/SKILL.md) · 1034★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: update-whats-new
description: Update the whats-new page with changes to the website since the previous release.
---

# Update what's new page

Use this skill when a new Dart release has occurred and
you need to update `src/content/resources/whats-new.md`
to describe the changes to the website
since the previous release.

## Steps

1.  **Identify the previous release date**

    Read `src/content/resources/whats-new.md`
    and locate the topmost release section.
    Find the "Released on" date for that release.
    This is your starting point.

2.  **Retrieve recent Git commits**

    Retrieve the git commits made to the repository
    since the previous release date identified in step 1.
    For example:
    `git log --after="<previous_release_date>" --oneline`.

3.  **Analyze commits for meaningful changes**

    Review the content of each commit since that date.
    Identify changes that are significant to developers or users.
    Look for:

    -   New glossary terms.
    -   Large or significant page updates.
    -   New pages.
    -   Deprecated or removed pages.
    -   New tutorials or guide enhancements.

    > [!IMPORTANT]
    > When analyzing changes for the
```

</details>
