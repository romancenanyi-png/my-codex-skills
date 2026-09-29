---
name: b2b-outreach-experiments
description: Design and review small, reply-focused B2B cold-outreach experiments from already verified prospects. Use for A-grade pilot selection, decision-maker personalization, email validation, deliverability readiness, single-variable tests, follow-up, reply classification, and stop or scale decisions. Do not use to scrape contacts or mass-send.
---

# B2B Outreach Experiments

Start with a 15-prospect pilot. Scale only after human replies and business-quality signals prove the route.

## Preconditions

- Each prospect passed a channel-specific verification skill and has source URLs.
- A public, attributable contact exists; named decision makers outrank generic inboxes.
- Sending domain authentication and mailbox reputation are checked where possible: SPF, DKIM, DMARC, recent bounces, and reply history.
- The user has separated research, draft approval, and send authority.

## Experiment design

1. Freeze one country, buyer type, product/use case, offer, CTA, and message structure.
2. State one observed business fact and one relevant buyer risk; do not manufacture personalization.
3. Keep the email concise, commonly 65–95 words, with one lightweight question.
4. Change one variable per cohort: subject, first line, proof, CTA, or sender—not all at once.
5. Validate syntax and domain; reject malformed, placeholder, guessed, support/help, opt-out, and hard-bounced addresses.
6. Send only after explicit approval. Verify exact Sent state and log timestamp/version.
7. Follow up once after 3–5 business days unless there is a reply, bounce, opt-out, or different agreed timing.

## Evaluation

Classify human positive, human neutral, objection, referral, auto-reply, bounce, opt-out, and no response. If a complete pilot produces zero human replies, stop scaling and change one upstream variable—list quality, decision-maker quality, sender trust, offer, or copy—then run a new pilot.

## Output

Return pilot hypothesis, prospect inclusion evidence, approved message versions, deliverability checks, send log, response table, learning, and `stop/iterate/scale` decision. Opens alone are not proof of interest.
