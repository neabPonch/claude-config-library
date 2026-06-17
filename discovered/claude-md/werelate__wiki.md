---
name: werelate__wiki
source: https://github.com/werelate/wiki/blob/8d0fb9bd046925b82a86315c904e5452fcd0cf61/CLAUDE.md
repo: werelate/wiki
kind: claude-md
stars: 11
last_pushed: 2026-05-22T17:54:25Z
license: gpl-2.0
score: 9
domains: [web-backend, php, media-wiki]
tags: [architecture-map, domain-specific, knowledge-base]
curated: 2026-06-15
curated_by: config-scout
---

# werelate/wiki — claude-md

**Why it's worth keeping:** It explicitly defines 'hidden' system behaviors like the Propagation Pattern and provides exhaustive lookup tables for namespace constants/IDs, which is critical for navigating custom-extended legacy frameworks.

**Summary:** Acts as a comprehensive technical manual that maps complex genealogical logic to specific PHP classes, namespaces, and MediaWiki lifecycle hooks.

**Source credibility:** Small-scale open-source project with regular maintenance history.

**Recency:** Highly relevant; technical architecture documentation remains useful regardless of specific LLM version updates.

**Source:** [werelate/wiki/CLAUDE.md](https://github.com/werelate/wiki/blob/8d0fb9bd046925b82a86315c904e5452fcd0cf61/CLAUDE.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

WeRelate.org is a genealogical wiki built on MediaWiki. The codebase extends MediaWiki with custom structured namespaces for genealogical data (Person, Family, Place, Source, etc.) and specialized functionality for family tree visualization, GEDCOM import/export, and genealogical data management.

## Setup and Installation

### Database Setup
```bash
# Download and import skeleton database
wget http://public.werelate.org.s3.amazonaws.com/wikidb.sql
mysql -u [user] -p [database_name] < wikidb.sql
```

### Simple Setup
```bash
cp htaccess.sample .htaccess
# Edit environment variables in .htaccess
```

### Full Setup
1. Copy files to a `w` directory under your htdocs root
2. Create Apache site file from `conf/apache2.sample`
3. Copy to `apache2/sites-available/[sitename]`
4. Fill in/modify values based on your environment
5. Enable the site: `a2ensite [sitename]`

### Running Jobs
Background jobs are disabled in the web context (`$wgJobRunRate = 0`). Run jobs manually:
```bash
php maintenance/runJobs.php
```

## Architecture

### Core MediaWiki
- **
```

</details>
