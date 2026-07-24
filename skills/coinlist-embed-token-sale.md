---
name: Embed a CoinList token sale offer
description: List the Passage offers available to the signed-in user, load full offer details, and read the eligibility requirements before showing an invest button.
api: openapi/coinlist-passage-openapi-original.json
operations: [listPartnerOffers, getPartnerOffer, listOfferRequirements, listOfferRequirementStatuses]
---

# Embed a CoinList (Passage) token sale offer

Passage lets a partner surface CoinList-managed token sales / tokenized-equity offers inside their own app. Authenticate first (OAuth 2.0 Bearer — see `authentication/coinlist-authentication.yml`).

## Steps
1. **List offers** — `GET /v1/offers` (`listPartnerOffers`). Paginate with `limit` + `starting_after`/`starting_before`; the response is `{ object: "list", data: [Offer] }`.
2. **Load details** — `GET /v1/offers/{id}` (`getPartnerOffer`) for the chosen offer id to render sale details and options.
3. **Read requirements** — `GET /v1/offers/{offer_id}/requirements` (`listOfferRequirements`) to learn what each option needs (KYC, jurisdiction, wallet, documents).
4. **Check status** — `GET /v1/offers/{offer_id}/requirements/statuses` (`listOfferRequirementStatuses`) to know which requirements the current user has already satisfied; only enable "Invest" when the option is eligible.

## Rules
- Auth: partner-scoped calls use the `client_credentials` grant; user-scoped calls (requirements/participations) need an `authorization_code` (PKCE) token.
- Errors return the custom envelope `{ type, message, code, errors, event_id }` (see `errors/coinlist-problem-types.yml`); surface `message` and log `event_id`.
- No idempotency key is supported; these are read operations.
