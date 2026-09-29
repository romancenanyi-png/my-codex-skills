---
name: b2b-inquiry-response-ops
description: Triage, draft, approve, send, and verify B2B inquiry email through gated queues for new inquiries, existing customers awaiting replies, and seven-day no-response follow-up. Use for inbox operations requiring human approval and evidence-based learning. Do not use for bulk cold outreach.
---

# B2B Inquiry Response Ops

Protect response quality by completing one queue before opening the next.

## Queue order

1. **A — New inbound inquiries:** answer the current question and obtain the minimum missing information.
2. **B — Existing customers awaiting reply/new project:** resolve the active blocker; do not restart completed discovery.
3. **C — Seven-day follow-up:** only messages actually sent at least 168 hours ago with no human reply.

Process at most five threads per review batch. Do not enter B until A is sent or explicitly deferred; do not enter C until B is closed for the run.

## Per-thread cycle

1. Read the complete thread and attachment metadata; distinguish human reply, bounce, auto-acknowledgement, and platform notification.
2. Build a fact card: customer need, supplied facts, open blocker, promises already made, and prohibited assumptions.
3. Draft a natural reply focused on the next decision. Ask only questions that change quoting, sampling, production, or delivery.
4. Present the draft for approval. Version approved edits; never send a superseded draft.
5. Send only with explicit authority, then verify the exact message appears in Sent. Unknown send state blocks retry until checked.
6. Update state with evidence and the next follow-up date.

## Seven-day exclusions

Exclude bounces, opt-outs, drafts never sent, threads waiting on the sender's quote/PI/sample/action, known channel migration, future-dated promises, and any thread with a later human reply.

## Output and learning

Return queue, thread summary, proposed reply, missing facts, risk flags, approval version, send evidence, and next action. Keep customer data in the authorized workspace. Record lessons only from explicit correction, verified outcome, or repeated evidence; never loop blind retries.
