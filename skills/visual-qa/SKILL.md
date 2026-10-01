---
name: visual-qa
description: Use when validating screenshots, rendered web pages, landing pages, UI changes, responsive layouts, accessibility, visual regressions, or design fidelity. This is a normalized replacement for the requested `isual-qa`, treated as `visual-qa`.
metadata:
  source_status: "custom-gap-fill"
  requested_name: "isual-qa"
  aliases: "isual-qa, visual-qa-validator, ui-visual-review"
  related_skills: "agent-browser"
---

# Visual QA

Use this skill to inspect visual output from websites, apps, screenshots, mockups, or generated assets. The goal is to catch design, layout, accessibility, and conversion issues before the user ships a page.

## When to use

Use this skill when the user asks to:

- Review a website, landing page, screenshot, or UI implementation.
- Compare a rendered page against a design direction or reference.
- Check responsive behavior on desktop, tablet, and mobile.
- Find layout bugs such as overflow, clipping, overlapping elements, broken spacing, or unreadable text.
- Check visual hierarchy, CTA prominence, scannability, contrast, and accessibility basics.
- Validate generated images or OG/social cards before publishing.

## Required inputs

Ask for only the missing essentials:

- URL, screenshot, design file, or local app route.
- Intended device sizes or breakpoints.
- Target audience and primary conversion goal.
- Brand constraints if visual tone matters.

## Workflow

1. **Capture or inspect**
   - Use browser automation or screenshots when available.
   - Inspect at desktop, tablet, and mobile widths.
   - Capture above-the-fold and important conversion sections.

2. **Check layout integrity**
   - Look for broken grids, overflow, clipping, unexpected scrollbars, stretched images, misaligned cards, and inconsistent spacing.
   - Verify that sticky headers, modals, dropdowns, and forms do not obscure content.

3. **Check hierarchy and conversion clarity**
   - Confirm the primary CTA is visually dominant.
   - Confirm the headline, proof, benefits, and CTA form a clear path.
   - Flag competing CTAs, unclear section order, and low-contrast supporting copy.

4. **Check accessibility basics**
   - Contrast appears readable.
   - Focus states are visible.
   - Interactive controls look clickable.
   - Text is not embedded in images unless intentionally decorative.
   - Important images have alt-text expectations documented.

5. **Check responsive behavior**
   - Mobile navigation works.
   - Cards stack correctly.
   - Typography remains readable.
   - Forms remain usable on narrow screens.

## Output format

Return a prioritized QA report:

```markdown
# Visual QA Report

## Summary
- Overall status: Pass / Needs fixes / Blocked
- Primary risk: ...

## Critical Issues
| Issue | Evidence | Impact | Fix |
|---|---|---|---|

## High-Impact Improvements
| Improvement | Why it matters | Suggested change |
|---|---|---|

## Responsive Notes
- Desktop:
- Tablet:
- Mobile:

## Accessibility Notes
- Contrast:
- Focus:
- Semantics:

## Ship Recommendation
Proceed / Fix first / Re-test after changes
```

## Quality bar

Be concrete. Do not say “improve spacing” without pointing to the section and the exact visual problem. Prefer actionable fixes over general design advice.
