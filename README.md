# Parseflow (parseflow)

Document parsing, extraction, and search API. Parse PDFs, DOCX, TXT, and raw text into structured chunks, extraction fields, and search-ready data — with deterministic and BYOK-LLM modes, async jobs with webhook delivery, batch processing, and a built-in keyword search index.

**APIs.yml:** [apis.yml](apis.yml)

## Type
- **x-type:** company
- **submitted via:** [api-search/network#35](https://github.com/api-search/network/issues/35)

## APIs
- **Parseflow API** — `https://parseflow-api.thankfulisland-fec0f8f2.westus2.azurecontainerapps.io` — process, analyze, batch, async jobs, document indexing + search, usage/quota, billing webhooks. [OpenAPI](openapi/parseflow-openapi.json) · [Docs](https://docs.parseflow.tech/docs/api-reference) · [Postman](https://documenter.getpostman.com/view/54564964/2sBXwmPsb9)

## Artifacts

| Artifact | Path |
|---|---|
| OpenAPI 3.1 (upstream mirror) | [openapi/parseflow-openapi.json](openapi/parseflow-openapi.json) |
| Naftiko capabilities | [capabilities/](capabilities/) (`process-document`, `analyze-document`, `batch-process`, `async-jobs`, `index-and-search`, `usage-and-quota` + shared API binding) |
| JSON Schema | [json-schema/](json-schema/) (process request/response, batch request, job status, indexed document, search response, usage) |
| JSON-LD context | [json-ld/parseflow-context.jsonld](json-ld/parseflow-context.jsonld) |
| Examples | [examples/](examples/) (`process`, `async-job`, `search`, `batch`) |
| Spectral ruleset | [rules/parseflow-rules.yml](rules/parseflow-rules.yml) |
| Vocabulary | [vocabulary/parseflow-vocabulary.yml](vocabulary/parseflow-vocabulary.yml) |
| Plans (API Commons 0.1) | [plans/parseflow-plans-pricing.yml](plans/parseflow-plans-pricing.yml) |
| Rate Limits (API Commons 0.1) | [rate-limits/parseflow-rate-limits.yml](rate-limits/parseflow-rate-limits.yml) |
| FinOps (FOCUS 1.3) | [finops/parseflow-finops.yml](finops/parseflow-finops.yml) |

## Plans (summary)

| Plan | Price | Monthly cap | Per-minute | Upload | Notes |
|---|---|---|---|---|---|
| Starter | $10/mo | 500 req (rolling 30d) | 20 rpm | 10 MB | Hard-capped — 429 `MONTHLY_USAGE_EXCEEDED` on overflow |
| Growth | $15/mo | 1,000 req (rolling 30d) | 20 rpm | 10 MB | Same enforcement as Starter |
| BYOK advanced lane | included | n/a | 5 rpm | 10 MB | `mode=byok_assisted`; model inference billed on caller's provider key |

Source: [docs.parseflow.tech/docs/pricing](https://docs.parseflow.tech/docs/pricing) · [docs.parseflow.tech/docs/limits](https://docs.parseflow.tech/docs/limits) · [docs.parseflow.tech/docs/billing](https://docs.parseflow.tech/docs/billing). Billing is processed by Whop; API keys carry the `pfk_` prefix and are sent as `X-API-Key`.

## Tags
Document Parsing, PDF, OCR, Text Extraction, Document AI, Search, BYOK, Async Jobs, Webhooks, REST

## Common Properties
- [Website](https://docs.parseflow.tech/)
- [Getting Started](https://docs.parseflow.tech/docs/getting-started)
- [API Reference](https://docs.parseflow.tech/docs/api-reference)
- [Pricing](https://docs.parseflow.tech/docs/pricing)
- [Limits](https://docs.parseflow.tech/docs/limits)
- [Billing](https://docs.parseflow.tech/docs/billing)
- [Postman](https://documenter.getpostman.com/view/54564964/2sBXwmPsb9)

## Timestamps
- **Created:** 2026-05-27
- **Modified:** 2026-05-27

## Maintainers
- **Kin Lane** — kin@apievangelist.com
