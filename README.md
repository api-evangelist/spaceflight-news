# Spaceflight News (spaceflight-news)

The Spaceflight News API (SNAPI) by The Space Devs (TSD) is the most complete and up-to-date open spaceflight news API. It aggregates articles, blogs, and reports from 40+ news sites (NASA, ESA, SpaceX, Spaceflight Now, SpaceNews, Ars Technica, Reuters, and more) and exposes them through a public REST API (and a GraphQL endpoint). The project is open source under AGPL-3.0, runs on community Patreon funding, and is integrated with the Launch Library 2 API so any article can be linked to a specific launch or event.

**APIs.json:** [https://spaceflightnewsapi.net](https://spaceflightnewsapi.net)

## Tags

- News
- Space
- Spaceflight
- Aerospace
- Open Source
- Launches
- Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Spaceflight News API v4

REST API providing access to aggregated spaceflight news articles, blog posts, and official mission reports from 40+ news sites. Supports rich filtering (full-text search, news-site filters, date ranges, related Launch Library 2 launches/events), pagination, and ordering. A companion GraphQL endpoint is also exposed at /v4/graphql/.

- **Human URL:** [https://spaceflightnewsapi.net](https://spaceflightnewsapi.net)
- **Base URL:** `https://api.spaceflightnewsapi.net/v4`

#### Tags

- News
- Space
- Articles
- Blogs
- Reports

#### Properties

- [Documentation](https://api.spaceflightnewsapi.net/v4/docs/)
- [OpenAPI](openapi/spaceflight-news-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/spaceflight-news.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/spaceflight-news.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Swagger U I](https://api.spaceflightnewsapi.net/v4/docs/)
- [Graph Q L](https://api.spaceflightnewsapi.net/v4/graphql/)
- [Schema](https://api.spaceflightnewsapi.net/v4/schema/)
- [Repository](https://github.com/TheSpaceDevs/spaceflightnewsapi)
- [Source Code](https://github.com/TheSpaceDevs/spaceflightnewsapi)

### Launch Library 2 API

Sister API by The Space Devs, used by SNAPI to relate news articles to specific launches and events. Provides upcoming/previous launch data, events, agencies, astronauts, expeditions, spacecraft, launchers, and pads. SNAPI articles, blogs, and reports can be filtered by `launch` (UUID) or `event` (LL2 ID).

- **Human URL:** [https://thespacedevs.com/llapi](https://thespacedevs.com/llapi)
- **Base URL:** `https://ll.thespacedevs.com/2.3.0`

#### Tags

- Space
- Launches
- Events

#### Properties

- [Documentation](https://ll.thespacedevs.com/2.3.0/swagger/)
- [Tutorial](https://github.com/TheSpaceDevs/Tutorials)
- [Tools](https://github.com/TheSpaceDevs/launch-library-mcp)
- [Postman Collection](collections/spaceflight-news.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/spaceflight-news.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://spaceflightnewsapi.net)
- [Documentation](https://api.spaceflightnewsapi.net/v4/docs/)
- [Repository](https://github.com/TheSpaceDevs/spaceflightnewsapi)
- [GitHub Organization](https://github.com/TheSpaceDevs)
- [License](https://github.com/TheSpaceDevs/spaceflightnewsapi/blob/main/LICENSE)
- [Changelog](https://github.com/TheSpaceDevs/spaceflightnewsapi/releases)
- [Twitter](https://twitter.com/the_snapi)
- [Discord](https://discord.gg/p7ntkNA)
- [Patreon](https://www.patreon.com/TheSpaceDevs)
- [Email](derk@spaceflightnewsapi.net)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [Tutorials](https://github.com/TheSpaceDevs/Tutorials)
- [F A Q](https://github.com/TheSpaceDevs/Tutorials/blob/main/faqs/faq_SNAPI.md)
- [F A Q](https://github.com/TheSpaceDevs/Tutorials/blob/main/faqs/faq_TSD.md)
- [Tools](https://github.com/TheSpaceDevs/launch-library-mcp)
- [Tools](https://github.com/TheSpaceDevs/snapiwebsite)
- [Tools](https://github.com/TheSpaceDevs/serpy)
- [Spectral Rules](rules/spaceflight-news-rules.yml)
- [Vocabulary](vocabulary/spaceflight-news-vocabulary.yml)
- [JSON-LD](json-ld/spaceflight-news-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
