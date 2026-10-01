---
name: agent-browser
description: Use a browser automation workflow to open pages, interact with websites, inspect UI state, capture screenshots, test forms, check accessibility trees, and extract web content.
metadata:
  source_status: "normalized-from-public-description"
  mapped_from: "agent-browser, agent-browser-2"
  aliases: "browser-automation, web-ui-testing"
  related_skills: "visual-qa, seo-expert, cro-expert"
---

# Agent Browser

Use this skill when the task requires actually interacting with a website or web app instead of only reasoning from text.

## When to use

Use for:

- Opening URLs and inspecting rendered pages.
- Clicking, typing, submitting forms, and testing flows.
- Capturing screenshots for visual QA.
- Checking mobile/desktop responsive behavior.
- Extracting content, links, metadata, headings, forms, CTAs, and structured page data.
- Testing login, checkout, signup, lead-gen, search, filter, navigation, and modal flows.
- Verifying whether UI changes are actually visible in the browser.

## Workflow

1. **Define the mission**
   - What needs to be verified or extracted?
   - What pages or user journeys matter?

2. **Open and observe**
   - Load the page.
   - Record title, URL, load errors, console-visible failures if available, and page state.

3. **Interact**
   - Click navigation, CTAs, filters, tabs, menus, forms, and modals.
   - Use realistic user data when testing forms.
   - Avoid destructive actions unless explicitly authorized.

4. **Capture evidence**
   - Screenshot important states.
   - Extract visible text, key DOM landmarks, metadata, and accessibility information when available.

5. **Report findings**
   - Separate confirmed observations from assumptions.
   - Include reproduction steps for bugs.

## Output format

```markdown
# Browser Inspection Report

## Scope
- URL(s):
- Device/viewport:
- Flow tested:

## Observations
| Area | Finding | Evidence | Severity |
|---|---|---|---|

## Reproduction Steps
1.
2.
3.

## Suggested Fixes
| Issue | Fix | Owner |
|---|---|---|
```

## Guardrails

- Do not submit payment, delete data, publish content, or send real emails unless the user explicitly asks.
- Use test data for forms.
- Respect robots, rate limits, and authentication boundaries.
