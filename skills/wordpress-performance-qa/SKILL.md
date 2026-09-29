---
name: wordpress-performance-qa
description: Optimize and regression-test WordPress performance without breaking forms, commerce, analytics, SEO, or buyer journeys. Use for image conversion, cache or minification settings, asset unloading, Core Web Vitals investigation, Lighthouse testing, or rollback decisions.
---

# WordPress Performance QA

Optimize by measured bottleneck, one reversible layer at a time.

## Baseline

1. Select representative home, category, product, capability, article, contact, and inquiry pages.
2. Record plugins/theme/CDN/cache state, form and analytics behavior, and a backup/rollback point.
3. Run at least three comparable tests per page and use the median. Separate cold-cache and warm-cache observations.
4. Record mobile and desktop metrics plus server response/TTFB; a CDN miss may dominate frontend changes.

## Safe optimization order

1. Resize and convert oversized images; preserve quality, dimensions, alt text, responsive `srcset`, and LCP priority.
2. Enable browser/page caching with explicit exclusions for dynamic, cart, account, form-success, or personalized pages.
3. Minify HTML/CSS only after a restore point. Avoid combining or delaying JavaScript unless dependency tests prove it safe.
4. Unload plugin assets only on pages that do not need them; never disable a plugin globally to solve one-page overhead.
5. Purge only affected URLs when possible, then remeasure under the same conditions.

## Regression and stop gates

Test at 360, 390, 768, 1024, 1440, and 1920 px where practical. Verify menus, forms, validation, thank-you flow, tracking, canonical/meta/H1, structured data, images, console errors, and commerce/account paths. Roll back the last change when median performance regresses materially, a function breaks, tracking disappears, or an interaction cannot be isolated.

## Output

Return baseline, change log, median before/after table, regression evidence, unresolved root causes, and exact rollback instructions. Never present the best run as the result.
