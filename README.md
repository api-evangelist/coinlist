# CoinList

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

CoinList is a fintech platform for the token economy - it runs compliant token sales, tokenized equities, trading, staking, and wallet services for crypto projects and investors. Its developer surface is Passage (the "Frontline API"), a partner API that lets third parties embed CoinList-managed token sales and tokenized equities directly inside their own apps: OAuth 2.0 (PKCE) partner and user authentication, Sumsub KYC token issuance, tax-document signing, offers, eligibility requirements, participations, wallet ownership proof and allow-listing, and on-chain swap/token reads. Passage runs the regulated infrastructure and back office; the partner focuses on the product. Shipped with a React SDK (@coinlist-co/react) of UI components, hooks, and server helpers. Added to the API Evangelist network from the electric-capital and polychain portfolios and enriched from CoinList's public developer surface.

**Areas:** Company · Fintech · Cryptocurrency · Token Sales · Tokenized Equities · KYC · Authentication · Blockchain · Digital Assets · Embedded Finance

## CoinList on APIs.io

Everything profiled for CoinList is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/coinlist/](https://apis.io/providers/coinlist/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [CoinList KYC API](https://apis.io/apis/coinlist/coinlist-kyc-api/) — The KYC API from CoinList — 1 operation(s) for kyc.
- [CoinList Offers API](https://apis.io/apis/coinlist/coinlist-offers-api/) — The Offers API from CoinList — 4 operation(s) for offers.
- [CoinList Participations API](https://apis.io/apis/coinlist/coinlist-participations-api/) — The Participations API from CoinList — 2 operation(s) for participations.
- [CoinList Pii API](https://apis.io/apis/coinlist/coinlist-pii-api/) — The Pii API from CoinList — 1 operation(s) for pii.
- [CoinList Requirements API](https://apis.io/apis/coinlist/coinlist-requirements-api/) — The Requirements API from CoinList — 2 operation(s) for requirements.
- [CoinList Swap API](https://apis.io/apis/coinlist/coinlist-swap-api/) — The Swap API from CoinList — 3 operation(s) for swap.
- [CoinList Token API](https://apis.io/apis/coinlist/coinlist-token-api/) — The Token API from CoinList — 2 operation(s) for token.
- [CoinList Wallet API](https://apis.io/apis/coinlist/coinlist-wallet-api/) — The Wallet API from CoinList — 1 operation(s) for wallet.
- [CoinList Wallet Ownership API](https://apis.io/apis/coinlist/coinlist-wallet-ownership-api/) — The Wallet Ownership API from CoinList — 1 operation(s) for wallet ownership.
- [CoinList O Auth API](https://apis.io/apis/coinlist/coinlist-oauth-api/) — The OAuth API from CoinList — 3 operation(s) for oauth.
- [CoinList document submissions API](https://apis.io/apis/coinlist/coinlist-document-submissions-api/) — The document submissions API from CoinList — 1 operation(s) for document submissions.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (2)

Multi-step workflows that chain operations into a business task.

- [CoinList Passage - Invest flow](https://apis.io/arazzos/coinlist/coinlist-invest-flow/)
- [CoinList Passage - KYC and document onboarding](https://apis.io/arazzos/coinlist/coinlist-kyc-onboarding/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [coinlist-passage](https://apis.io/servers/coinlist/coinlist-passage/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Coinlist Agentic Access](https://apis.io/agentic-access/coinlist/coinlist-agentic-access/)

#### Collections (11)

Postman and Open Collection request collections.

- [Frontline DocumentSubmissions API](https://apis.io/collections/coinlist/open-coinlist-documentsubmissions-api/)
- [Frontline DocumentSubmissions KYC API](https://apis.io/collections/coinlist/open-coinlist-kyc-api/)
- [Frontline DocumentSubmissions OAuth API](https://apis.io/collections/coinlist/open-coinlist-oauth-api/)
- [Frontline DocumentSubmissions Offers API](https://apis.io/collections/coinlist/open-coinlist-offers-api/)
- [Frontline DocumentSubmissions Participations API](https://apis.io/collections/coinlist/open-coinlist-participations-api/)
- [Frontline DocumentSubmissions Pii API](https://apis.io/collections/coinlist/open-coinlist-pii-api/)
- [Frontline DocumentSubmissions Requirements API](https://apis.io/collections/coinlist/open-coinlist-requirements-api/)
- [Frontline DocumentSubmissions Swap API](https://apis.io/collections/coinlist/open-coinlist-swap-api/)
- [Frontline DocumentSubmissions Token API](https://apis.io/collections/coinlist/open-coinlist-token-api/)
- [Frontline DocumentSubmissions Wallet API](https://apis.io/collections/coinlist/open-coinlist-wallet-api/)
- [Frontline DocumentSubmissions Wallet Ownership API](https://apis.io/collections/coinlist/open-coinlist-wallet-ownership-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Coinlist Passage Overlay](https://apis.io/overlays/coinlist/coinlist-passage-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Coinlist Authentication](https://apis.io/security/coinlist/coinlist-authentication/)
- [Coinlist Domain Security](https://apis.io/security/coinlist/coinlist-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Coinlist Scopes](https://apis.io/scopes/coinlist/coinlist-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://coinlist.co/)
- [Documentation](https://docs.passage.coinlist.co/)
- [Getting started](https://docs.passage.coinlist.co/sdk/quickstart)
- [API reference](https://docs.passage.coinlist.co/api-reference)
- [Support](https://support.coinlist.co/)
- [Blog](https://blog.coinlist.co)
- [Terms of service](https://coinlist.co/terms)
- [Privacy policy](https://coinlist.co/privacy)
- [GitHub](https://github.com/coinlist)
- [Status](https://status.coinlist.co)

## API Evangelist rating

**Kin Score 43.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 43.6 |
| Contract governance | 4.5 |
| Operational transparency | 34.2 |
| Developer ergonomics | 66.1 |
| Access clarity | 27.6 |

**Agent readiness 35.2** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | paginated |
| Operation Distinctiveness | distinct |

**Regulatory alignment 32.4** — Securities & Market Data

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/coinlist/](https://apis.io/providers/coinlist/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for CoinList: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/coinlist/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
