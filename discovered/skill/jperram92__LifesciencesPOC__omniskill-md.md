---
name: jperram92__LifesciencesPOC__omniskill-md
source: https://github.com/jperram92/LifesciencesPOC/blob/58d4d269c580e3335650181fafb6629e18128bb4/OmniSkill.MD
repo: jperram92/LifesciencesPOC
kind: skill
stars: 0
last_pushed: 2026-04-21T20:59:46Z
license: unknown
score: 9
domains: [salesforce, devops]
tags: [omnistudio, xml-automation, config-management]
curated: 2026-06-15
curated_by: config-scout
---

# jperram92/LifesciencesPOC — skill

**Why it's worth keeping:** It utilizes a 'Clone Strategy' directive to prevent property hallucination and includes exact, high-fidelity `propertySetConfig` blocks required by the engine.

**Summary:** Provides strict technical constraints and JSON templates for creating/modifying Salesforce OmniScript XML files to ensure Designer UI compatibility.

**Source credibility:** Low public reputation (0 stars), but the extreme technical specificity suggests it is derived from specialized enterprise assets.

**Recency:** Very current, based on a push from 2 months ago.

**Source:** [jperram92/LifesciencesPOC/OmniSkill.MD](https://github.com/jperram92/LifesciencesPOC/blob/58d4d269c580e3335650181fafb6629e18128bb4/OmniSkill.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sf-omniscript
description: >
Comprehensive guide for creating and maintaining OmniStudio OmniScripts (.os-meta.xml files).
TRIGGER when: user creates new OmniScript versions, edits .os-meta.xml files, fixes Designer UI
crashes, adds steps/elements to an OmniScript, deploys/retrieves OmniScripts, or works with
the omniScripts/ folder.
DO NOT TRIGGER when: OmniStudio DataRaptors/Integration Procedures (use sf-metadata), LWC OmniOut
components (use sf-lwc), or Apex invoked from OmniScript (use sf-apex).
license: MIT
metadata:
version: "1.3.0"
author: "HLS Assets Team"
sf-omniscript
This skill ensures that all OmniStudio OmniScript components created or modified in this repository are syntactically complete, UI-compatible, and consistently named.
1. Directory Structure
Flat Folder Structure (Recommended):
All OmniScript files should reside in the root of the `omniScripts/` directory.
Path: `force-app/main/default/omniScripts/<filename>.os-meta.xml`
Legacy Subfolder Structure:
Avoid using subfolders (e.g., `omniScripts/HLS_ReferralForm_English/`) unless explicitly requested for legacy migration purposes. If a retrieval results in a flat file, keep it flat.
2. Naming Convention
```

</details>
