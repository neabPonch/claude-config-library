---
name: digitalsparky__jekyll-minifier
source: https://github.com/digitalsparky/jekyll-minifier/blob/5422b3570321668b419ec8271391a029f385c390/CLAUDE.md
repo: digitalsparky/jekyll-minifier
kind: claude-md
stars: 260
last_pushed: 2025-09-12T18:14:09Z
license: gpl-3.0
score: 8
domains: [ruby, cli-tools, web-infrastructure]
tags: [architecture-heavy, dockerized, contextual]
curated: 2026-06-15
curated_by: config-scout
---

# digitalsparky/jekyll-minifier — claude-md

**Why it's worth keeping:** The 'Release Status' section provides immediate project state/delta context, while the Architecture section explains crucial side-effect mechanisms like how it hooks into Jekyll core classes.

**Summary:** Provides technical depth on integration patterns (monkey patching) and complete command sets for both local and Docker development.

**Source credibility:** Decent niche popularity (260 stars) with recent maintenance history.

**Recency:** Current; includes modern Docker workflows and environment-specific execution paths.

**Source:** [digitalsparky/jekyll-minifier/CLAUDE.md](https://github.com/digitalsparky/jekyll-minifier/blob/5422b3570321668b419ec8271391a029f385c390/CLAUDE.md) · 260★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Jekyll Minifier is a Ruby gem that provides minification for Jekyll sites. It compresses HTML, XML, CSS, JSON and JavaScript files both inline and as separate files using terser, cssminify2, json-minify and htmlcompressor. The gem only runs when `JEKYLL_ENV="production"` is set.

## Release Status (v0.2.1)

**READY FOR RELEASE** - Security vulnerability patched:
- ✅ **SECURITY FIX**: ReDoS vulnerability in preserve_patterns completely resolved
- ✅ Comprehensive ReDoS protection with pattern validation and timeout guards
- ✅ 100% backward compatibility maintained - all existing configs work unchanged
- ✅ Extensive security test suite: 90/90 tests passing (74 original + 16 security)
- ✅ Graceful degradation - dangerous patterns filtered with warnings, builds continue
- ✅ Performance impact minimal - security checks complete in microseconds
- ✅ Comprehensive security documentation added (SECURITY.md)

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Build the gem
gem build jekyll-minifier.gemspec

# Run
```

</details>
