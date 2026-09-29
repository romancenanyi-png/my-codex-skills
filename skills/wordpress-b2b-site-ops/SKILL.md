---
name: wordpress-b2b-site-ops
description: Plan, edit, and QA inquiry-focused WordPress B2B manufacturing sites. Use for site architecture, buyer paths, page modules, service/product/FAQ content, forms, responsive behavior, scoped changes, launch checklists, or rollback plans. Do not use for keyword strategy or performance tuning alone.
---

# WordPress B2B Site Ops

Build a site that lets a buyer answer four questions quickly: what is supplied, who it is for, what proof exists, and how to request a quote.

## Required inputs

- Business facts: products, buyer types, markets, capabilities, MOQ, lead time, certifications, and unsupported claims.
- Existing URLs, CMS/theme/builder, plugins, forms, analytics, and backup access.
- Desired conversion action and pages in scope.

If a fact is missing, mark it `unknown`; never invent it.

## Workflow

1. Freeze scope. Record live URLs, screenshots, key forms, plugins, analytics, and rollback point.
2. Map buyer journeys. Connect home → product/category → capability → proof/FAQ → inquiry.
3. Assign one purpose to each URL. Preserve useful URLs unless migration is explicitly approved.
4. Write visible modules: buyer problem, product fit, capability boundary, process, proof, FAQ, and one primary CTA.
5. Keep business rules identical across product, service, FAQ, form, and structured data.
6. Implement the smallest scoped change. Use page-specific selectors and avoid unrelated plugin/theme changes.
7. Test form success/failure, notifications, analytics, navigation, internal links, and mobile behavior.
8. Compare before/after and record changed files/settings, unresolved risks, and rollback steps.

## Hard gates

- No unsupported capacity, certification, delivery, sustainability, customer, or quality claims.
- No removal of working forms, analytics, canonical URLs, or core plugins without approval.
- One visible H1 per page; one clear primary CTA; no dead-end buyer path.
- Test representative widths from 360 px through desktop; do not claim mobile QA from one screenshot.

## Output and validation

Return scope, buyer journey, URL/page matrix, module copy, implementation list, QA evidence, open issues, and rollback plan. Verify every claim, click every changed path, submit test forms where authorized, and confirm the live page matches the approved scope.
