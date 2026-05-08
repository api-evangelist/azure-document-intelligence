# Azure AI Document Intelligence (azure-document-intelligence)

Azure AI Document Intelligence (formerly Form Recognizer) is Microsoft's cloud document understanding service. It exposes prebuilt models for invoices, receipts, IDs, business cards, tax forms and contracts, plus a layout/OCR Read model and a Custom-model framework for fine-tuned extraction.

**APIs.json:** [apis.yml](apis.yml)

## APIs
- **Document Intelligence REST API** — `https://<your-resource>.cognitiveservices.azure.com` — Read, Layout, Prebuilt models, Custom Classifiers and Extractors. Subscription-key or Microsoft Entra ID auth. [Docs](https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/) · [API reference](https://learn.microsoft.com/en-us/rest/api/aiservices/document-models/) · [OpenAPI](openapi/azure-document-intelligence-openapi.json).

## OpenAPI (fetched 2026-05-08)
`openapi/azure-document-intelligence-openapi.json` — Microsoft's Swagger 2.0 v2024-11-30 GA spec, source <https://github.com/Azure/azure-rest-api-specs/tree/main/specification/ai/data-plane/DocumentIntelligence>.

## Tags
AI, Document AI, Azure, IDP, OCR, Microsoft, REST

## Common Properties
- [Service page](https://azure.microsoft.com/en-us/products/ai-services/ai-document-intelligence) · [Docs](https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/) · [Pricing](https://azure.microsoft.com/en-us/pricing/details/document-intelligence/)
- [Source](https://github.com/Azure/azure-rest-api-specs/tree/main/specification/ai/data-plane/DocumentIntelligence)
- [Plans](plans/azure-document-intelligence-plans-pricing.yml) — reconciled
- [Rate Limits](rate-limits/azure-document-intelligence-rate-limits.yml) — reconciled
- [FinOps](finops/azure-document-intelligence-finops.yml) — reconciled, FOCUS-aligned

## Plans (reconciled)
- **Free (F0)** — 500 pages/mo.
- **Standard (S0)** — Read $1.50/1K pages (drops to $0.60/1K above 1M); Prebuilt $10/1K; Custom Classification $3/1K; Custom Extraction (incl. Custom Generative) $30/1K; Add-Ons $6/1K; Query Fields $10/1K; training $3/h after first 10h free.
- **Commitment Tiers** — e.g. Custom 20K pages $540/mo … 500K pages $10.5K/mo; Prebuilt 20K $190/mo … 500K $4K/mo; Read 500K $375/mo … 8M $4.2K/mo.

## Rate Limits (reconciled)
- F0: 1 TPS · S0: 15 TPS (raisable on request).
- Document caps (S0): 500 MB / 2,000 pages.
- 429 with `Retry-After`.

## Timestamps
- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## Maintainers
- **Kin Lane** — kin@apievangelist.com
