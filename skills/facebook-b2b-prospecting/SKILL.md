---
name: facebook-b2b-prospecting
description: Discover, verify, score, and deduplicate B2B buyer prospects from public Facebook pages and official business sources. Use for buyer research, public email or WhatsApp verification, page-activity checks, exclusion logging, and research-only prospect tables. Do not guess contacts or send outreach without separate authority.
---

# Facebook B2B Prospecting

Research in two passes: broad discovery, then strict verification.

## Search design

Use narrow combinations of product + buyer type + city/country, such as distributor, wholesaler, corporate-gift supplier, travel retailer, outdoor retailer, school supplier, beauty distributor, or promotional-products company. Avoid generic industry searches that flood results with consumers and competitors.

## Verification chain

1. Open the public Facebook page and record page URL, business category, location, recent activity date, and product-fit evidence.
2. Follow the official website link or independently verify the matching domain.
3. Confirm buyer role and signs of repeat inventory, wholesale, distribution, private label, or bulk procurement.
4. Record only a publicly displayed official email. A phone is not WhatsApp unless an explicit WhatsApp link/button or business source confirms it.
5. Search for a public decision maker in procurement, sourcing, product, merchandising, partnerships, or ownership.
6. Dedupe by normalized company, domain, page, first email, phone/WhatsApp, decision maker, and prior-contact history.

## Hard rejects

Reject private/personal profiles, inactive pages without a current business site, repair/consignment/resale-only services, consumers, irrelevant packaging/printers, support/help-only contacts, placeholder or guessed emails, opt-outs, and prior hard bounces.

## Output schema

Return `Company`, `Buyer_Type`, `Country_City`, `Facebook_URL`, `Website`, `Recent_Activity`, `Fit_Evidence`, `Contact_Name_Role`, `Email`, `WhatsApp`, `Contact_Source`, `Score`, `Grade`, `Exclusion_Reason`, and `Checked_At`. Separate fact from inference and preserve public source URLs.

This skill ends at research unless the user separately authorizes drafting or sending.
