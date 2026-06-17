---
name: vyskoczilova__woocommerce-payforpayment
source: https://github.com/vyskoczilova/woocommerce-payforpayment/blob/59e137ba5250c8237e6c7744edb4e9389a7b1e5b/CLAUDE.md
repo: vyskoczilova/woocommerce-payforpayment
kind: claude-md
stars: 13
last_pushed: 2026-03-18T13:19:22Z
license: unknown
score: 9
domains: [wordpress, ecommerce, php]
tags: [logic-flow, hook-registry, architectural-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# vyskoczilova/woocommerce-payforpayment — claude-md

**Why it's worth keeping:** Uses specific line number pointers to ground the LLM in critical math logic and includes a comprehensive list of available hooks/filters essential for WordPress development.

**Summary:** Provides an exceptionally detailed map of core business logic flows, including exact file locations and code line references.

**Source credibility:** A real-world WooCommerce plugin with active maintenance (3 months ago).

**Recency:** Highly current, utilizing modern WordPress/WooCommerce compatibility standards.

**Source:** [vyskoczilova/woocommerce-payforpayment/CLAUDE.md](https://github.com/vyskoczilova/woocommerce-payforpayment/blob/59e137ba5250c8237e6c7744edb4e9389a7b1e5b/CLAUDE.md) · 13★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Pay for Payment for WooCommerce is a WordPress plugin that adds individual charges (fixed and/or percentage-based) for each payment method in WooCommerce. The plugin calculates percentage fees first, then adds fixed fees on top.

**Key Constraints:**
- Not currently compatible with WooCommerce Block Checkout (shortcode checkout required)
- Not compatible with WooCommerce Stripe Payment Gateway (React-based)
- Minimum WooCommerce version: 2.6 (WC 3.2+ recommended)
- HPOS (High-Performance Order Storage) compatible
- PHP 8.0+ supported

## Architecture

### Plugin Structure

The plugin follows a class-based singleton pattern with the following core components:

**Main Entry Point:** `woocommerce-payforpayment.php`
- Checks for WooCommerce dependency
- Initializes core class and integrations
- Declares HPOS compatibility

**Core Classes (in `/inc/`):**

1. **`Pay4Pay` (class-pay4pay.php)** - Main plugin logic
   - Singleton pattern (`Pay4Pay::instance()`)
   - Handles fee calculation in `calculate_pay4payment()` at line 94
   - Fee calculation base
```

</details>
