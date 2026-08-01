---
name: Steadily agency quote to offer
description: As an appointed independent agency, create a draft quote in your rater, price and underwrite it, then generate a firm offer through the Steadily Rater Quotes API.
api: openapi/steadily-rater-quotes-openapi-original.json
operations: [who_am_i, Agent Bearer Token, quote_create, quote_update, price_quote, underwriting_info, offer_quote, get_offer, get_policy]
---

# Steadily — Agency draft quote to firm offer

Use this skill when an agency appointed with Steadily creates quotes directly from
its rater and turns them into firm offers and policies.

## Auth
- Base URL: `https://api.steadily.com`, all paths under `/v1`.
- Authenticate with your `X-Steadily-ApiKey`.
- For agent-scoped calls, mint a bearer token with `Agent Bearer Token`
  (`POST /v1/account/agency/token`) and send it as `Authorization: Bearer <token>`.
- Confirm the key/referral identity any time with `who_am_i`
  (`GET /v1/account/info`).

## Steps
1. **Create a draft quote** — `quote_create` (`POST /v1/agency/draft_quote`) with
   the property and coverage inputs. Capture the returned `quote_id` (e.g.
   `qte_100259208`).
2. **Refine** — `quote_update` (`PUT /v1/agency/draft_quote/{quote_id}`) to adjust
   inputs; read it back with `quote_info` (`GET /v1/agency/draft_quote/{quote_id}`).
3. **Price** — `price_quote` (`GET /v1/agency/draft_quote/{quote_id}/price`).
4. **Underwrite** — `underwriting_info`
   (`GET /v1/agency/draft_quote/{quote_id}/underwrite`) to retrieve underwriting
   detail.
5. **Make an offer** — `offer_quote` (`POST /v1/agency/quote_offer`) to generate a
   firm offer; read it with `get_offer` (`GET /v1/agency/quote_offer/{offer_id}`).
6. **Retrieve the policy** — once bound, `get_policy`
   (`GET /v1/agency/policy/{policy_id}`).

## Conventions
- JSON in / JSON out; validation errors are HTTP 422 with a `detail[]` array.
- List endpoints paginate with `limit` + `starting_after_id`.
- Entity graph: quote → offer → policy (see `data-model/steadily-data-model.yml`).
