---
name: Onboard a user through KYC and tax documents
description: Start a Sumsub KYC session, pre-fill tax forms from stored PII, and create a document signing submission for a Passage user.
api: openapi/coinlist-passage-openapi-original.json
operations: [createKycToken, getPii, createDocumentSubmission]
---

# Onboard a Passage user (KYC + documents)

Completes the identity and tax-document requirements that gate participation. All calls need a user-scoped (`authorization_code` + PKCE) access token.

## Steps
1. **Start KYC** — `POST /v1/kyc-token` (`createKycToken`) to mint a short-lived Sumsub WebSDK access token, then launch the Sumsub verification flow client-side.
2. **Pre-fill PII** — `GET /v1/pii` (`getPii`) to retrieve the user's legal name, country of citizenship, tax ID, and address (null when unavailable) to pre-fill forms.
3. **Sign documents** — `POST /v1/documents/{document_type}/submission` (`createDocumentSubmission`) for a document type such as a W-8BEN; the signing link is emailed to the user. Re-posting resends / re-signs where the document state allows.

## Rules
- Partner-only (`client_credentials`) tokens are rejected by `createKycToken` — a user-scoped token is required.
- PII is forwarded to Passport, never stored by the partner; handle it transiently.
- Errors use the `{ type, message, code, errors, event_id }` envelope (see `errors/coinlist-problem-types.yml`).
