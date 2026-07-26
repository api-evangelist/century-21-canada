# Century 21 Canada (century-21-canada)

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
