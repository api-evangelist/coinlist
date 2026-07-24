---
name: Complete the Passage invest flow
description: Prove wallet ownership, allow-list the wallet for an offer, check on-chain balance/allowance, and create a participation for a signed-in user.
api: openapi/coinlist-passage-openapi-original.json
operations: [getPartnerOffer, getTokenBalance, getTokenAllowance, createWalletOwnershipChallenge, allowWallet, createPartnerParticipation, getPartnerParticipation]
---

# Complete the Passage invest flow

Drives the full investment path from a chosen offer option to a tracked participation. Requires a user-scoped (`authorization_code` + PKCE) access token.

## Steps
1. **Load the offer** — `GET /v1/offers/{id}` (`getPartnerOffer`) to get the option, chain, and token contract the user will pay with.
2. **Read on-chain state** — `GET /v1/token/balance` (`getTokenBalance`) and `GET /v1/token/allowance` (`getTokenAllowance`) to confirm the connected wallet can fund the purchase and whether an ERC-20 approval is still needed.
3. **Prove wallet ownership** — `POST /v1/wallet-ownership` (`createWalletOwnershipChallenge`) to issue a challenge the user signs.
4. **Allow the wallet** — `POST /v1/offers/{offer_id}/allow-wallet` (`allowWallet`) to authorize the proven wallet on the offer.
5. **Create the participation** — `POST /v1/participations` (`createPartnerParticipation`) with the offer option and wallet.
6. **Track it** — `GET /v1/participations/{id}` (`getPartnerParticipation`) to poll status.

## Rules
- Auth: user-scoped Bearer token; partner-only tokens are rejected on user endpoints.
- No `Idempotency-Key` support — guard client-side against double-submits before `createPartnerParticipation`.
- Errors use `{ type, message, code, errors, event_id }`; on `invalid_request_error` inspect the `errors` field-map.
