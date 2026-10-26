# Century 21 Canada (century-21-canada)

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

CENTURY 21 Canada Limited Partnership is the Canadian master franchisor of the CENTURY 21® real estate brand, headquartered at 1285 West Pender Street in Vancouver, British Columbia. The master licence for Canada was secured in Vancouver in 1976 — the first international franchise of the CENTURY 21 System — and the network today spans roughly 400 independently owned and operated offices from coast to coast. Century 21 Canada sits in the brokerage/franchisor layer of the Canadian real estate value chain: it consumes member-owned MLS® listing data distributed nationally by the Canadian Real Estate Association (CREA) through REALTOR.ca and the Data Distribution Facility (DDF®), rather than originating or redistributing that data as a product of its own.

Its API posture is empty, and this profile records that honestly. As of a 2026-07-26 probe there is no developer portal, no API documentation, no published base URL, no SDK, no webhooks, no Postman collection, and no machine-readable contract of any kind on century21.ca or c21.ca.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/century-21-canada/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/century-21-canada/refs/heads/main/apis.yml)

## Tags

- Real Estate
- Canada
- Brokerage
- Franchising
- Property Listings
- MLS
- Residential Real Estate
- Commercial Real Estate
- PropTech

## Timestamps

- **Created:** 2026-07-26
- **Modified:** 2026-07-26

## APIs

No public APIs are published by Century 21 Canada. See `review.yml` for the full probe record.

## RESO Posture

No RESO reference found. There is no RESO Web API certification, no RESO Data Dictionary certification or version claim, no OData service root, no `$metadata` document, and no Universal Property Identifier (UPI) usage anywhere in the public surface. This is the expected Canadian answer: RESO certification is a US MLS-layer artifact, while Canadian listing distribution runs through CREA's single national DDF®, which CREA describes as normalized to the RESO Data Dictionary. A brokerage franchisor is a downstream consumer of that pool, not a certified data provider.

## Access Gate

`none-published` — there is nothing for a developer to sign up for, apply to, license, or join, because no API exists. The real gate sits one layer up at CREA: REALTOR®/board membership plus data-feed credentials, or a board IDX/VOW data licence agreement. Century 21 Canada's own gated surfaces are people-gates, not API gates — `my.hub21.ca` and `engage.hub21.ca` both redirect (HTTP 302) to a MoxiWorks member login.

## Open Data

None. No dataset, bulk download, or unlicensed feed is published. The terms of use restrict MLS content to authorized use and prohibit scraping and derivative works.

## Auth Model

No API authentication model is published. `/.well-known/openid-configuration` returned HTTP 403 on both century21.ca and www.c21.ca. Human authentication for agents and franchisees is a MoxiWorks session login.

## Platform Vendor

The Century 21 Canada terms of use name **MoxiWorks LLC** as the site operator. The consumer site, property search, listing hosts, agent hub (hub21.ca), CMA tooling, and lead pipeline are all MoxiWorks platform surfaces. Any API capability in that stack belongs to MoxiWorks, not to Century 21 Canada.

## A Note on Wildcard DNS

`*.century21.ca` and `*.c21.ca` are wildcarded onto `eboat.moxiworks.com`, so `developer.`, `developers.`, `api.` and `docs.` all return HTTP 200 without a developer portal existing. A control probe against a nonsense subdomain reproduced the same 200. The one distinct host, `api.c21.ca`, is a 2019-vintage Microsoft-IIS placeholder returning the three characters `API`.

## Common Properties

- [Website](https://www.c21.ca/)
- [Blog](https://www.c21.ca/blog)
- [Blog RSS](https://www.c21.ca/feed)
- [Press Releases](https://www.c21.ca/category/press-releases)
- [Terms of Service](https://www.c21.ca/terms-of-use)
- [Privacy Policy](https://www.c21.ca/privacy-policy)
- [Sitemap](https://www.c21.ca/sitemap.xml)
- [Property Search](https://www.c21.ca/search/)
- [Office Directory](https://www.c21.ca/directory)
- [Franchise Sales](https://century21franchise.ca/)
- [Member Portal](https://my.hub21.ca/)
- [Facebook](https://www.facebook.com/CENTURY21Canada)
- [Instagram](https://www.instagram.com/century21canada/)
- [YouTube](https://www.youtube.com/channel/UCK9uFomKQuOUR8sSKHe7yWQ)

## Maintainers

- Kin Lane — kin@apievangelist.com
