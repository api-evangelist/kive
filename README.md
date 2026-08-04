# Kive

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Kive is an AI product photography and campaign content platform for e-commerce brands, built by TO LABS AB and used by more than 10,000 brands. It generates product shots, lifestyle scenes, campaign imagery and product videos from a brand's own assets using a catalogue of curated visual presets ("studios"), paired with a creative asset library, AI search, boards, custom-trained subject models, bulk catalogue generation and AI editing tools.

Kive publishes **no public REST API**. Its programmable surface is an **OAuth-protected Model Context Protocol server** at `https://mcp.kive.ai/mcp`, which lets agents browse workspaces, saved products, trained models, studios and video presets, create products, generate images and videos, and edit outputs — all on the authorizing user's workspace permissions and credits.

- Website — https://www.kive.ai/
- MCP hub — https://kive.ai/mcp
- Documentation — https://kive.ai/docs
- Trust portal — https://trust.kive.ai/ (ISO/IEC 27001:2022)

Backed by: creandum, eqt-ventures

## Artifacts

| Artifact | Method |
|---|---|
| `mcp/kive-mcp.yml` | searched — published MCP server, OAuth metadata, documented capabilities |
| `authentication/kive-authentication.yml` | searched — OAuth 2.1 authorization code + PKCE |
| `scopes/kive-scopes.yml` | searched — `kive:mcp`, `offline_access` |
| `well-known/` | searched — RFC 8414 + RFC 9728 discovery documents (raw) |
| `llms/kive-llms.txt` | searched — verbatim from https://kive.ai/llms.txt |
| `conventions/kive-conventions.yml` | searched — credit model, async polling, no idempotency contract |
| `conformance/kive-conformance.yml` | searched — MCP, OAuth/RFC stack, ISO 27001 |
| `changelog/kive-changelog.yml` | searched — dated product-updates feed |
| `plans/kive-plans.yml` | searched — Free/Basic/Pro/Enterprise |
| `rate-limits/kive-rate-limits.yml` | searched — credit-based metering |
| `security/kive-trust-center.yml` | searched — ISO 27001 cert, 104 controls |
| `security/kive-vulnerability-disclosure.yml` | searched — security@kive.ai via trust portal |
| `security/kive-domain-security.yml` | probed — TLS 1.3, HSTS, SPF, DMARC reject |

Not applicable / not published: OpenAPI, AsyncAPI, webhooks, SDKs/packages, CLI, sandbox, status page, deprecation policy, security.txt.
