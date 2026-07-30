# Kive

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
