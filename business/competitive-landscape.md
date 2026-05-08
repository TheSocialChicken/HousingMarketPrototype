# Competitive Landscape
> AI-Powered Construction Procurement | Last updated: 2026-05-08
>
> Sources: Crunchbase, Capterra, vendor sites, Contrary Research, PR Newswire

---

## Positioning Statement

We occupy a specific intersection that no current competitor covers: **construction-specific AI procurement, deployed locally, fine-tuned per client, with explainable output suitable for public-sector audit requirements, targeting the Dutch and EU market.**

The market is crowded with generic procurement suites and a handful of construction-specific cloud tools — but the combination of local deployment, per-client fine-tuning, and construction domain specialisation is an open space.

---

## Competitive Map

| Category | Players | Our overlap | Our advantage |
|---|---|---|---|
| **Generic enterprise procurement suites** | SAP Ariba, Coupa, Ivalua, GEP SMART | Procurement automation | Local deployment, construction domain, per-client model, SME-accessible |
| **Construction project management with procurement** | Procore, Autodesk Construction Cloud | Construction sector | AI-first, fine-tuning, local model, not bundled with broader PM tool |
| **Construction materials procurement (cloud)** | Kojo, Parspec, Field Materials, Constrafor | Construction materials + AI matching | Local deployment, EU/NL market, per-client fine-tuning, explainability |
| **Dutch/EU public procurement platforms** | Mercell (Negometrix), TenderNed | Dutch public sector, compliance | AI decision layer on top of what they only manage as a process |
| **AI procurement automation (horizontal)** | Fairmarkit, Levelpath, Zip HQ | AI + automation | Construction domain, local deployment, fine-tuned model |

---

## Player Profiles

---

### 1. SAP Ariba / Coupa / Ivalua / GEP SMART
> Enterprise procurement suites with AI features

**What they do:** Full source-to-pay suites covering sourcing, supplier management, contracts, and spend analytics. AI features focus on spend classification, supplier risk scoring, and contract analytics.

**Deployment:** Cloud-only. SAP Ariba has on-premise legacy roots but current offering is SaaS.

**Construction specialisation:** None. Generic horizontal procurement.

**AI approach:** Rule-based analytics and AI-assisted search, not fine-tuned per client. No per-client model training.

**Target market:** Enterprise (500+ employees), typically €100K+ ACV contracts.

**Why they're not our real competitor:**
- Cloud-only: disqualified for clients with data sovereignty requirements (municipalities, large infrastructure orgs)
- Priced and scoped for enterprise procurement departments, not construction site procurement managers
- No construction material domain knowledge — materials, specifications, certifications are handled generically
- No fine-tuning means no improvement over time on the client's specific supplier and material base

**Threat level:** LOW for Segment A (construction companies). MEDIUM for Segment B (municipalities) — SAP/Coupa are present in large municipal IT stacks.

---

### 2. Procore
> Construction project management platform with materials/procurement module

**What they do:** Comprehensive construction project management — budgets, documents, schedules, RFIs, submittals. Launched a Materials module for procurement-to-installation tracking.

**Deployment:** Cloud-only (SaaS).

**Construction specialisation:** HIGH — Procore is purpose-built for construction. Strong brand in the sector.

**AI approach:** Submittal workflow automation, document extraction. Limited AI-driven supplier comparison or recommendation.

**Target market:** General contractors, mid-to-large construction companies. US-dominant, growing in EU.

**Why they're not our real competitor:**
- Procurement is a module within a broader platform — clients who already use Procore are locked into its procurement workflow, not looking for a separate AI layer
- No supplier matching or specification-to-material AI recommendation engine
- No fine-tuning on client data
- Cloud-only — not viable for sovereign deployments

**Threat level:** MEDIUM — Procore is the most likely platform to add an AI procurement assistant. If Procore builds or acquires a matching engine, it becomes a serious threat to Segment A clients who are already in their ecosystem. Watch.

**Opportunity:** Procore does not serve the AI recommendation / fine-tuning use case. An integration or co-existence model is possible — our AI layer on top of their data.

---

### 3. Parspec
> Closest direct AI competitor — construction materials specification matching

**What they do:** AI-powered platform that extracts product requirements from engineering drawings and specifications, then matches them to compliant products from a database of 6M+ products across 4,000+ manufacturer catalogues. Generates instant quotes and submittal packages. Raised **$20M Series A** (Threshold Ventures, 2024). 4× revenue growth, 288 customers.

**Deployment:** Cloud-only (SaaS).

**Construction specialisation:** HIGH — purpose-built for construction procurement. Started with MEP (mechanical, electrical, plumbing); expanding to other trades.

**AI approach:** LLM + ML for specification extraction and product matching. Not fine-tuned per client — matches against a shared product catalogue, not the client's own historical procurement data.

**Target market:** US-centric. Electrical/MEP distributors and contractors. Limited EU presence as of 2026.

**Why this is the most important competitor to track:**
- Parspec is doing the closest thing to what we're building: AI-powered spec-to-product matching in construction
- Well-funded, validated, and growing
- Their model is cloud and catalogue-based — our model is local and client-data-based

**Where we differ:**
| Parspec | Us |
|---|---|
| Cloud-only | Local / on-premise |
| Shared product catalogue (6M items) | Fine-tuned on client's own procurement history |
| US market, MEP/electrical focus | EU/NL market, broad construction materials |
| No per-client training | Model improves with the client's own data |
| No audit trail for public sector | Explainable AI, audit-ready output |
| Not municipality-suitable | Designed for municipalities and compliance |

**Threat level:** HIGH if they enter the EU market. Currently LOW in NL due to geography and product focus.

---

### 4. Kojo
> Construction materials procurement and management

**What they do:** Cloud platform for materials management — purchase orders, delivery tracking, invoice matching, inventory. Focused on field purchasing workflows for contractors.

**Deployment:** Cloud-only.

**Construction specialisation:** HIGH — procurement and materials management purpose-built for construction.

**AI approach:** Workflow automation and spend visibility, not AI-driven specification matching or supplier recommendation.

**Target market:** US general contractors and subcontractors. No EU presence identified.

**Why they're not our real competitor:**
- Procurement management tool, not an AI recommendation and matching engine
- No fine-tuning, no specification-to-supplier matching, no explainability
- US-only

**Threat level:** LOW — different product category, no EU presence.

---

### 5. Mercell (formerly Negometrix)
> Dutch public procurement platform — largest private e-procurement player in NL

**What they do:** E-procurement platform managing the tendering process — publishing tenders, receiving bids, bid evaluation, award management. Acquired Negometrix (NL) in 2021. Negometrix held ~33% of Dutch public sector e-procurement before acquisition.

**Deployment:** Cloud (SaaS). Well-embedded in Dutch municipalities and government bodies.

**Construction specialisation:** None — horizontal public procurement process management.

**AI approach:** Workflow, process, compliance tracking. No AI-driven supplier matching, no material specification reasoning, no fine-tuned models.

**Target market:** Dutch municipalities, provinces, central government, public bodies. Also expanding EU.

**Why they're not our real competitor — but they matter:**
- Mercell manages the *procurement process* (tendering, compliance); we provide the *AI decision layer* (which supplier, which material, why)
- These are complementary, not competing functions
- Mercell is deeply embedded in municipalities — they are a potential integration or channel partner, not a threat

**Threat level:** LOW as a competitor. HIGH as a potential strategic partner or integration target.

**Opportunity:** Municipalities already use Mercell for tender management. Our AI assistant could sit alongside Mercell — the AI recommends and documents; Mercell processes the formal tender. This is not a conflict.

---

### 6. TenderNed
> Dutch national public tender publication platform

**What they do:** Statutory platform where Dutch public bodies must publish above-threshold tenders (national and EU Directive). Mandatory by law, not a commercial product.

**What they're not:** Not an AI tool, not a procurement recommendation system, not a competitor.

**Relevance:** Our municipality clients use TenderNed for formal publication. Our AI assistant helps them *prepare* the evaluation and documentation before and during the tender — TenderNed handles the formal publication step.

---

## Differentiation Matrix

| | SAP Ariba / Coupa | Procore | Parspec | Kojo | Mercell | **Us** |
|---|:---:|:---:|:---:|:---:|:---:|:---:|
| **Local / on-premise deployment** | ✗ | ✗ | ✗ | ✗ | ✗ | **✅** |
| **Construction material domain** | ✗ | ✅ | ✅ | ✅ | ✗ | **✅** |
| **AI specification matching** | ✗ | ✗ | ✅ | ✗ | ✗ | **✅** |
| **Fine-tuned per client** | ✗ | ✗ | ✗ | ✗ | ✗ | **✅** |
| **Explainable AI / audit trail** | ✗ | ✗ | ✗ | ✗ | ✗ | **✅** |
| **Municipal / public sector compliance** | ⚠️ | ✗ | ✗ | ✗ | ✅ | **✅** |
| **Dutch / EU market focus** | ⚠️ | ⚠️ | ✗ | ✗ | ✅ | **✅** |
| **SME-accessible pricing** | ✗ | ⚠️ | ✅ | ✅ | ✅ | **✅** |
| **Data sovereignty** | ✗ | ✗ | ✗ | ✗ | ✗ | **✅** |

> ✅ = yes · ⚠️ = partial · ✗ = no

**The combination of all nine criteria exists only in our product.**

---

## Competitive White Space

The gap we occupy:

> A construction-specific AI procurement assistant, deployed on the client's own infrastructure, with a model fine-tuned on their own data, that produces explainable, audit-ready output — for the Dutch and EU market.

No current player combines all of these. The closest single competitor on AI + construction is Parspec — but Parspec is cloud-only, US-focused, catalogue-driven, and not designed for public-sector compliance or explainability.

The closest Dutch player on compliance + municipalities is Mercell — but Mercell is a process platform, not an AI decision layer, and has no material specification reasoning at all.

---

## Competitive Risks

| Risk | Trigger | Mitigation |
|---|---|---|
| **Procore builds AI matching** | Procore adds a spec-to-supplier AI feature or acquires Parspec | Build client lock-in through fine-tuned models before Procore reaches feature parity; target local-deployment clients Procore cannot serve |
| **Parspec enters EU** | Parspec raises Series B, begins EU expansion | Establish NL market presence and first clients before they arrive; local deployment is a structural barrier Parspec cannot replicate quickly |
| **SAP/Coupa adds local deployment** | SAP offers private cloud / on-premise Ariba for regulated sectors | Our per-client fine-tuning remains a differentiator even in that scenario; construction domain depth is hard to replicate with a horizontal platform |
| **Mercell adds AI layer** | Mercell builds or buys an AI recommendation engine | Position as complementary integration rather than competitor; approach Mercell for a partnership before they build it |
| **New NL construction AI startup** | A local startup copies the positioning | First-mover advantage via Windesheim + pilot clients; fine-tuned models create switching costs |

---

## Sources

- [Parspec $20M Series A — PR Newswire](https://www.prnewswire.com/news-releases/parspec-raises-20-million-series-a-to-modernize-the-construction-supply-chain-with-ai-302498075.html)
- [Parspec company profile — Contrary Research](https://research.contrary.com/company/kojo)
- [Kojo competitors — Tracxn](https://tracxn.com/d/companies/kojo/__9bC3hRKmoIfOZkN55nm11_MbjNgp_w2hcO-XWDvr7-w)
- [Mercell acquires Negometrix — M&A Worldwide](https://m-a-worldwide.com/mercell-holding-acquires-negometrix-in-the-netherladnds/)
- [Dutch Public Procurement guide — TenderMetric](https://tendermetric.com/insights/dutch-procurement-guide)
- [11 Best Construction Procurement Software Tools 2026 — ConstructionBids.ai](https://constructionbids.ai/blog/procurement-software-construction-contractors)
- [Best AI Procurement Software 2026 — Tropic](https://www.tropicapp.io/glossary/best-ai-procurement-software)
- [Europe AI in Construction Market — MarketDataForecast](https://www.marketdataforecast.com/market-reports/europe-artificial-intelligence-in-construction-market)
- [Procore construction procurement — Procore](https://www.procore.com/library/construction-procurement)
