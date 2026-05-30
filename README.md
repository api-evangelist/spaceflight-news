# Spaceflight News (spaceflight-news)

The Spaceflight News API (SNAPI) by The Space Devs (TSD) is the most complete and up-to-date open spaceflight news API. It aggregates articles, blogs, and reports from 40+ news sites (NASA, ESA, SpaceX, Spaceflight Now, SpaceNews, Ars Technica, Reuters, and more) and exposes them through a public REST API (and a GraphQL endpoint). The project is open source under AGPL-3.0, runs on community Patreon funding, and is integrated with the Launch Library 2 API so any article can be linked to a specific launch or event.

**URL:** [Visit APIs.json URL](https://spaceflightnewsapi.net)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - News, Space, Spaceflight, Aerospace, Open Source, Launches, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## Type

- **x-type:** opensource
- **x-license:** AGPL-3.0
- **x-governance:** community
- **x-funding:** Patreon
- **x-source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: News

## APIs

### Spaceflight News API v4

REST API providing access to aggregated spaceflight news articles, blog posts, and official mission reports from 40+ news sites. Supports rich filtering (full-text search, news-site filters, date ranges, related Launch Library 2 launches/events), pagination, and ordering. A companion GraphQL endpoint is also exposed at /v4/graphql/.

**Human URL:** [https://spaceflightnewsapi.net](https://spaceflightnewsapi.net)

**Base URL:** `https://api.spaceflightnewsapi.net/v4`

**Version:** 4.30.2

#### Tags:

 - News, Space, Articles, Blogs, Reports

#### Properties

- [Documentation](https://api.spaceflightnewsapi.net/v4/docs/)
- [OpenAPI](openapi/spaceflight-news-openapi.yml)
- [SwaggerUI](https://api.spaceflightnewsapi.net/v4/docs/)
- [GraphQL Endpoint](https://api.spaceflightnewsapi.net/v4/graphql/)
- [OpenAPI Schema (Live)](https://api.spaceflightnewsapi.net/v4/schema/)
- [Repository](https://github.com/TheSpaceDevs/spaceflightnewsapi)
- [SourceCode](https://github.com/TheSpaceDevs/spaceflightnewsapi)
- [NaftikoCapability — Articles](capabilities/spaceflight-news-articles.yaml)
- [NaftikoCapability — Blogs](capabilities/spaceflight-news-blogs.yaml)
- [NaftikoCapability — Reports](capabilities/spaceflight-news-reports.yaml)
- [NaftikoCapability — Info](capabilities/spaceflight-news-info.yaml)

### Launch Library 2 API

Sister API by The Space Devs, used by SNAPI to relate news articles to specific launches and events. Provides upcoming/previous launch data, events, agencies, astronauts, expeditions, spacecraft, launchers, and pads. SNAPI articles, blogs, and reports can be filtered by `launch` (UUID) or `event` (LL2 ID).

**Human URL:** [https://thespacedevs.com/llapi](https://thespacedevs.com/llapi)

**Base URL:** `https://ll.thespacedevs.com/2.3.0`

#### Tags:

 - Space, Launches, Events

#### Properties

- [Documentation](https://ll.thespacedevs.com/2.3.0/swagger/)
- [Launch Library 2 Tutorial](https://github.com/TheSpaceDevs/Tutorials)
- [Launch Library MCP Server](https://github.com/TheSpaceDevs/launch-library-mcp)

## Common Properties

- [Website](https://spaceflightnewsapi.net)
- [Documentation](https://api.spaceflightnewsapi.net/v4/docs/)
- [Repository](https://github.com/TheSpaceDevs/spaceflightnewsapi)
- [GitHubOrganization](https://github.com/TheSpaceDevs)
- [License — AGPL-3.0](https://github.com/TheSpaceDevs/spaceflightnewsapi/blob/main/LICENSE)
- [ChangeLog](https://github.com/TheSpaceDevs/spaceflightnewsapi/releases)
- [Twitter](https://twitter.com/the_snapi)
- [Discord](https://discord.gg/p7ntkNA)
- [Patreon (Funding)](https://www.patreon.com/TheSpaceDevs)
- [Email — derk@spaceflightnewsapi.net](mailto:derk@spaceflightnewsapi.net)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [TheSpaceDevs Tutorials & FAQs](https://github.com/TheSpaceDevs/Tutorials)
- [SNAPI FAQ](https://github.com/TheSpaceDevs/Tutorials/blob/main/faqs/faq_SNAPI.md)
- [TSD FAQ](https://github.com/TheSpaceDevs/Tutorials/blob/main/faqs/faq_TSD.md)
- [Launch Library MCP Server](https://github.com/TheSpaceDevs/launch-library-mcp)
- [SNAPI Website (snapiwebsite)](https://github.com/TheSpaceDevs/snapiwebsite)
- [Serpy (Serialization Library)](https://github.com/TheSpaceDevs/serpy)
- [SpectralRules](rules/spaceflight-news-rules.yml)
- [Vocabulary](vocabulary/spaceflight-news-vocabulary.yml)
- [JSONLD](json-ld/spaceflight-news-context.jsonld)

## Features

| Name | Description |
|------|-------------|
| News Aggregation | Aggregates spaceflight news from 40+ sites (NASA, ESA, SpaceX, ULA, Spaceflight Now, SpaceNews, Ars Technica, Reuters, and more) into a single API. |
| Three Content Types | Separate endpoints for articles (news), blogs (op-eds and longform), and reports (official mission/program reports). |
| Full-Text Search | Search articles by title, summary, or arbitrary keyword across all three content types. |
| Launch Library 2 Integration | Every article can be linked to a Launch Library 2 launch (UUID) or event (LL2 ID), enabling related-news widgets in launch tracking apps. |
| Rich Filtering | Filter by news site (inclusion/exclusion lists), published-at/updated-at date ranges, has_launch, has_event, is_featured. |
| Ordering and Pagination | Order by published_at or updated_at (ascending or descending) with offset/limit pagination. |
| GraphQL Endpoint | Companion GraphQL endpoint at /v4/graphql/ for clients that want to shape their own responses. |
| Free and Open | Free to use, no authentication required, open source under AGPL-3.0, funded through Patreon. |

## Use Cases

| Name | Description |
|------|-------------|
| Launch Tracker Companion Feed | Embed a "related news" feed alongside upcoming launches in a launch tracking app, using the LL2 launch UUID to filter SNAPI articles. |
| Space Industry Newsletter | Pull recent articles, dedupe by news site, and publish a daily/weekly newsletter rollup. |
| Voice Assistant Briefing | Power a daily spaceflight briefing skill that reads out the latest featured articles from a curated set of news sites. |
| Research and Analysis | Build a corpus of spaceflight news for NLP/research projects (topic modeling, sentiment analysis, mission coverage analysis). |
| Mission Operator Dashboard | Surface official mission reports alongside live telemetry/operations dashboards for situational awareness. |
| Educational Apps | Power student-facing apps that pair upcoming launches with explanatory articles and blog posts. |

## Integrations

| Name | Description |
|------|-------------|
| Launch Library 2 API | Sister TSD API; articles/blogs/reports can be linked to LL2 launch UUIDs and event IDs. |
| Patreon | Funding model — the API is community-funded via Patreon contributions to The Space Devs. |
| Discord | Support and feedback channel via the TSD Discord server (#feedback-and-help forum). |
| GitHub Issues | Bug reports and feature requests handled via GitHub Issues on TheSpaceDevs/spaceflightnewsapi. |

## Solutions

| Name | Description |
|------|-------------|
| Spaceflight News Apps | Mobile and web apps that aggregate and display spaceflight news from many publishers without each app maintaining its own scrapers. |
| Mission Coverage Dashboards | Dashboards that combine launches, events, and news coverage in one view. |
| Newsroom Tooling | Editorial dashboards for spaceflight journalists tracking what competitor outlets are publishing on a given mission. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Spaceflight News API v4](openapi/spaceflight-news-openapi.yml) — 7 operations across 4 tags (Articles, Blogs, Reports, Info); 11 component schemas; 25 reusable parameters.

### JSON Schema

- [Article](json-schema/spaceflight-news-article-schema.json)
- [Author](json-schema/spaceflight-news-author-schema.json)
- [Blog](json-schema/spaceflight-news-blog-schema.json)
- [Event](json-schema/spaceflight-news-event-schema.json)
- [Info](json-schema/spaceflight-news-info-schema.json)
- [Launch](json-schema/spaceflight-news-launch-schema.json)
- [PaginatedArticleList](json-schema/spaceflight-news-paginated-article-list-schema.json)
- [PaginatedBlogList](json-schema/spaceflight-news-paginated-blog-list-schema.json)
- [PaginatedReportList](json-schema/spaceflight-news-paginated-report-list-schema.json)
- [Report](json-schema/spaceflight-news-report-schema.json)
- [Socials](json-schema/spaceflight-news-socials-schema.json)

### JSON Structure

- [Article](json-structure/spaceflight-news-article-structure.json)
- [Author](json-structure/spaceflight-news-author-structure.json)
- [Blog](json-structure/spaceflight-news-blog-structure.json)
- [Event](json-structure/spaceflight-news-event-structure.json)
- [Info](json-structure/spaceflight-news-info-structure.json)
- [Launch](json-structure/spaceflight-news-launch-structure.json)
- [PaginatedArticleList](json-structure/spaceflight-news-paginated-article-list-structure.json)
- [PaginatedBlogList](json-structure/spaceflight-news-paginated-blog-list-structure.json)
- [PaginatedReportList](json-structure/spaceflight-news-paginated-report-list-structure.json)
- [Report](json-structure/spaceflight-news-report-structure.json)
- [Socials](json-structure/spaceflight-news-socials-structure.json)

### JSON-LD

- [Spaceflight News Context](json-ld/spaceflight-news-context.jsonld) — 11 type declarations + property terms with XSD datatypes and schema.org alignments.

### Examples

- [Article](examples/spaceflight-news-article-example.json)
- [Author](examples/spaceflight-news-author-example.json)
- [Blog](examples/spaceflight-news-blog-example.json)
- [Event](examples/spaceflight-news-event-example.json)
- [Info](examples/spaceflight-news-info-example.json)
- [Launch](examples/spaceflight-news-launch-example.json)
- [PaginatedArticleList](examples/spaceflight-news-paginated-article-list-example.json)
- [PaginatedBlogList](examples/spaceflight-news-paginated-blog-list-example.json)
- [PaginatedReportList](examples/spaceflight-news-paginated-report-list-example.json)
- [Report](examples/spaceflight-news-report-example.json)
- [Socials](examples/spaceflight-news-socials-example.json)

## Capabilities

Naftiko capabilities for each Spaceflight News API business surface. Each file is self-contained with an inline `consumes` block and both REST + MCP adapters.

### Spaceflight News API v4

| Workflow | Operations | REST | MCP Tools | Persona |
|----------|-----------|------|-----------|---------|
| [Articles](capabilities/spaceflight-news-articles.yaml) | listArticles, retrieveArticle | 2 | 2 | News Reader / Launch Tracker Developer |
| [Blogs](capabilities/spaceflight-news-blogs.yaml) | listBlogs, retrieveBlog | 2 | 2 | News Reader / Editorial Curator |
| [Reports](capabilities/spaceflight-news-reports.yaml) | listReports, retrieveReport | 2 | 2 | Mission Operator / Researcher |
| [Info](capabilities/spaceflight-news-info.yaml) | retrieveInfo | 1 | 1 | Integrator |

## Vocabulary

- [Spaceflight News Vocabulary](vocabulary/spaceflight-news-vocabulary.yml) — Unified taxonomy mapping 4 resources, 2 actions, 4 workflows, and 6 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Spaceflight News Spectral Rules](rules/spaceflight-news-rules.yml) — 35+ rules across 13 categories enforcing SNAPI API conventions (snake_case parameters/properties, kebab-case paths, trailing slashes, HTTPS-only servers, camelCase operationIds, Title Case tags, "Spaceflight News" summary prefix, and more).

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
