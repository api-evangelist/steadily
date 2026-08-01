---
name: Steadily partner estimate and refer a lead
description: Get a landlord-insurance estimate for a rental property and refer the prospect to Steadily as a partner (property manager, lender, or marketplace).
api: openapi/steadily-estimate-api-openapi-original.json
operations: [instant_estimate, quote_estimate, refer_lead, get_lead, partner_summary]
---

# Steadily — Estimate and refer a lead

Use this skill to produce a landlord-insurance estimate for a rental property and
hand the prospect to Steadily through the Partner (Estimate) API.

## Auth
- Base URL: `https://api.steadily.com`, all paths under `/v1`.
- Send your API key as the `X-Steadily-ApiKey` header (or query param). Some
  operations also accept the `X-Steadily-SecretKey`.
- Request keys from `partnerships-team@steadily.com`.

## Steps
1. **Instant estimate** — call `instant_estimate` (`POST /v1/quote/instant-estimate`)
   for a fast ballpark premium in seconds, or `quote_estimate`
   (`POST /v1/quote/estimate`) for a fuller estimate. Pass the property details.
2. **Refer the lead** — when the prospect wants to proceed, call `refer_lead`
   (`POST /v1/quote/submit`) to submit the lead to Steadily. Capture the returned
   `entity_id`.
3. **Check status** — call `get_lead` (`GET /v1/quote/estimate/{entity_id}`) to
   retrieve the current state of that referral.
4. **Reconcile** — periodically call `partner_summary` (`GET /v1/report/summary`)
   to reconcile leads, accounts, and bound policies for your partnership.

## Conventions
- Requests and responses are `application/json`.
- List/report endpoints paginate with `limit` + `starting_after_id` and return a
  `next` cursor.
- Validation failures return HTTP 422 with a `detail[]` array of `{loc, msg, type}`
  (see `errors/steadily-problem-types.yml`).
- No idempotency-key contract is documented — do not blindly retry `refer_lead`.
