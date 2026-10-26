# aceRNA Technologies

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

**aceRNA Technologies Co., Ltd.** (株式会社アクセルナ / aceRNA Technologies) is a Japanese
biotechnology venture founded in April 2018 to commercialize the RNA design technology known as the
**RNA Switch**, developed in the synthetic RNA biology laboratory of Prof. Hirohide Saito at Kyoto
University. An RNA Switch is embedded into a messenger RNA so that expression of the therapeutic
transgene is gated by the activity of a specific microRNA inside the cell — letting a treatment act
only on the cell type and cell state that is actually diseased. The company applies the platform
across mRNA medicines, cell therapy and gene therapy, and works with partner companies on joint
development. It is headquartered at the University of Tokyo Entrepreneur Plaza in Tokyo.

## API surface

**aceRNA runs no developer programme.** There is no API reference, developer portal, OpenAPI,
GraphQL SDL, AsyncAPI, SDK, CLI, webhook catalogue, pricing page or status page anywhere on
`acernatec.com`. `/openapi.json`, `/swagger.json`, `/graphql`, `/api-docs`, `/docs` and the whole
`/.well-known/` prefix all miss, and no `api.` / `developer.` / `docs.` subdomain is published.

Two machine-readable surfaces **are** served on the domain, and both are captured here verbatim:

| Surface | URL | Status |
|---|---|---|
| `llms.txt` | https://www.acernatec.com/llms.txt | 200 — real llms.txt, in Japanese |
| Site MCP endpoint | https://www.acernatec.com/_api/mcp | 200 — `tools/list` returns 9 tools with JSON Schema inputs |

Both are **generated by the Wix platform**, which hosts the site — they are not authored by aceRNA
and there is no aceRNA-built API behind them. The MCP endpoint exposes generic Wix site tools
(business details, in-site search, site API doc search, anonymous visitor-token issuance and a Wix
REST bridge) over the site's public marketing content. Read them as *"the host platform is
agent-aware"*, not *"the company runs an API programme"*.

## Artifacts

- `mcp/acerna-mcp.yml` + `mcp/acerna-tools-list.json` — the live `tools/list` response, verbatim
- `llms/acerna-llms.txt` — the served `llms.txt`, verbatim
- `authentication/acerna-authentication.yml` — the auth model the MCP endpoint actually enforces
- `conformance/acerna-conformance.yml` — what the host does and does not conform to, with evidence
- `well-known/acerna-well-known.yml` — negative probe record for the `/.well-known/` surface
- `security/acerna-domain-security.yml` — TLS/HSTS/DNSSEC/CAA/SPF/DMARC probe
- `plans/acerna-plans-pricing.yml`, `rate-limits/acerna-rate-limits.yml` — honest zeros

Sources: https://www.acernatec.com/ · https://www.acernatec.com/en ·
harvest listing https://equityzen.com/company/acerna
