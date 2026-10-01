---
name: b2b-website-architecture
description: Plan B2B website structure, navigation, URL patterns, conversion paths, page hierarchy, SEO hubs, industry pages, solution pages, comparison pages, resource centers, and internal linking.
metadata:
  source_status: "mapped-from-public-skill"
  mapped_from: "site-architecture"
  source_url: "https://github.com/LeoYeAI/openclaw-marketing-skills/blob/main/skills/site-architecture/SKILL.md"
  related_skills: "b2b-seo-geo-ops, wordpress-b2b-site-ops"
---

# B2B Website Architecture

Use this skill to design the structure of a B2B website so that buyers can understand the product, find relevant use cases, verify the supplier, and convert.

## Required inputs

- ICP and buying committee.
- Product/service families and capability boundaries.
- Primary market, language, conversion action, and sales motion.
- Verified proof, missing evidence, and claims that must not be published.
- Existing URLs and migration constraints when redesigning a live site.

Mark missing facts as `unknown`; do not fill them with plausible copy.

## Workflow

1. Define the primary buyer, business outcome, market, language, and conversion.
2. Map the buying journey: discovery → fit → evidence → evaluation → inquiry.
3. Inventory existing or required pages. Give each URL one primary intent and conversion role.
4. Design a small Phase 1 sitemap before adding long-tail pages.
5. Specify header, footer, breadcrumbs, hubs, contextual links, and orphan-page prevention.
6. Connect product/solution pages to capabilities, proof, buyer guides, FAQs, and inquiry pages.
7. Plan redirects and canonical URLs when URLs change.
8. Separate launch requirements from later expansion.

## Manufacturing / export model

```text
Homepage (/)
├── Products (/products)
│   └── Product category (/products/{category})
├── Services / Capabilities (/services)
│   ├── OEM (/services/oem)
│   └── ODM (/services/odm)
├── Materials / Quality / Process
├── About / Factory / Certifications
├── Resources (/resources)
│   └── Buyer guide (/guides/{topic})
├── FAQ (/faq)
└── Contact / Request a Quote
```

Adapt this model to the business. Do not create empty pages merely to match the tree.

## Decision rules

- Prefer a relevant existing page over a new competing URL.
- Do not use the sitemap as a substitute for crawlable internal links.
- Keep URLs stable unless the benefit justifies migration risk.
- Give informational content a path to a relevant commercial page and inquiry action.
- Do not mix consumer shopping paths into an inquiry-led B2B journey unless explicitly required.
- Preserve useful live URLs and working conversion paths during redesigns.

## Output

Return:

1. Business context and assumptions.
2. Buyer journey.
3. Phase 1 and Phase 2 sitemap.
4. URL map with page, parent, intent, evidence, CTA, and status (`keep/update/create/merge/redirect`).
5. Navigation and breadcrumb specification.
6. Internal linking and conversion-path map.
7. Redirect/canonical plan where relevant.
8. Missing inputs and validation checklist.
