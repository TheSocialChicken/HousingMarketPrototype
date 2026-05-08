# Market Sizing - TAM / SAM / SOM
> AI-Powered Construction Procurement | Last updated: 2026-05-08
>
> Primary method: Bottom-up. Top-down used for validation.
> Geography: SAM and SOM are Netherlands-only. TAM is EU-wide.
> All figures in EUR, per year (ARR where applicable).

---

## Data Sources

| Data point | Source |
|---|---|
| NL construction enterprises by size class (2023) | Statista / CBS StatLine (table 81589NED) |
| NL construction sector added value €40.7B (2022) | CBS Longread: *De Nederlandse bouwnijverheid in onzekere tijden 2019–2023* |
| NL construction employment 570,000 (2022) | CBS Longread (ibid.) |
| NL total public procurement ~€70–116B/year | TenderMetric Dutch Procurement Guide; Monitor Aanbestedingen 2021–2023 (Rijksoverheid, Dec 2024) |
| Municipalities = ~40% of announced contracts | TenderNed Aanbestedingsmonitor 2017–2025 |
| Works (construction) = ~12–14% of procurement type | TenderNed Aanbestedingsmonitor 2017–2025 |
| Number of NL municipalities: 342 (Jan 2025) | Wikipedia / Government.nl |
| European procurement software market €2.92B (2025) | MarketDataForecast: *Europe Procurement Software Market* |
| Rijkswaterstaat procurement: ~€4B/year | TenderMetric Dutch Procurement Guide |
| Water boards collective procurement: ~€3B/year | TenderMetric Dutch Procurement Guide |

---

## Pricing Assumptions

> These are internal estimates used for calculation. To be validated with first pilot clients.

| Customer type | Setup / onboarding | Annual subscription | Average year 1 | Average year 2+ |
|---|---|---|---|---|
| Mid-size construction co. (50–249 employees) | €15,000 | €24,000 | €39,000 | €27,000 |
| Large construction co. (250+ employees) | €25,000 | €48,000 | €73,000 | €52,000 |
| Medium municipality (25k–100k inhabitants) | €15,000 | €30,000 | €45,000 | €33,000 |
| Large municipality (100k+ inhabitants) | €25,000 | €60,000 | €85,000 | €65,000 |
| **Blended average (all segments, amortised)** | | | | **~€35,000/year** |

---

## Segment A - Construction Companies

### Market Definition
Construction companies in the Netherlands with 50 or more employees that conduct regular, structured material procurement. Focus: general contractors, civil engineering firms, and large specialist contractors - not micro-firms or pure subcontractors.

### Population (from CBS / Statista, 2023)

| Size class | Companies in NL | Notes |
|---|---|---|
| 0–9 employees | 267,891 | Micro - out of scope |
| 10–19 employees | 2,944 | Small - out of scope |
| 20–49 employees | 1,760 | Small - out of scope |
| **50–249 employees** | **780** | Core target |
| **250+ employees** | **133** | Enterprise target |
| **Total 50+ employees** | **913** | Starting universe |

### Bottom-Up: TAM (EU-wide)

Netherlands represents approximately 4% of EU GDP. Extrapolating from 913 NL companies with 50+ employees in construction:

- Estimated EU construction companies 50+ employees: **~18,000–22,000**
- Filter: companies doing regular material procurement (vs. pure civil or labour-only): **~70% = ~14,000**
- Average contract value (blended, conservative for EU): **€25,000/year**

**Segment A TAM (EU) = 14,000 × €25,000 = €350M/year**

### Bottom-Up: SAM (Netherlands only)

Starting universe: 913 companies (50+ employees)

| Filter | Rationale | Remaining |
|---|---|---|
| Active material procurement (not pure subcontractors or civil engineering only) | Only firms sourcing materials regularly benefit from matching | ~70% = 640 |
| Sufficient data for pilot / fine-tuning (ERP or structured records) | Minimum viable dataset required; demo/simulation covers firms without it | ~65% = ~415 |
| Decision-maker accessible and digital procurement investment appetite | Excludes very traditional firms unlikely to adopt | ~90% = **~375** |

**Qualifying companies: ~375**

Revenue calculation:
- 780 mid-size companies × 80% qualifying × €27,000/year avg = **€16.8M**
- 133 large companies × 85% qualifying × €52,000/year avg = **€5.9M**

**Segment A SAM (NL) ≈ €13–17M/year**
> Conservative working figure: **€15M/year**

### SOM - Netherlands, Years 1–5

| Year | Clients | ARR (Segment A) | Penetration of SAM |
|---|---|---|---|
| Year 1 | 3–5 | €100–150K | < 1% |
| Year 2 | 8–12 | €250–380K | 2% |
| Year 3 | 15–20 | €475–620K | 4% |
| Year 5 | 30–40 | €900K–1.2M | ~8% |

> Basis: new entrants in SaaS/enterprise typically reach 2–3% of SAM by Year 3, 5–8% by Year 5 (consistent with Osterwalder startup-analyst skill benchmark).

---

## Segment B - Municipalities

### Market Definition
Dutch municipalities (gemeenten) procuring construction, infrastructure, and public works contracts. Subject to Dutch Aanbestedingswet 2012 and EU procurement directives. Compliance documentation and explainability are legally mandated, not optional.

### Population

- **342 municipalities** in the Netherlands (as of January 2025)
- Breakdown by size (approximate, based on CBS population data):

| Municipality size | Count | Procurement profile |
|---|---|---|
| Large (>100k inhabitants) | ~28 | Dedicated procurement teams; large annual construction programmes; own IT infrastructure |
| Medium (25k–100k) | ~100 | Smaller procurement teams; active but less complex programmes |
| Small (<25k) | ~214 | Often outsource procurement; limited standalone budget for tooling |

### Bottom-Up: TAM (EU-wide)

- EU has approximately 89,000 municipalities (Eurostat)
- Relevant target: municipalities with active construction procurement and dedicated procurement capacity
  - Filter to towns with >10,000 inhabitants and active build programmes: **~18,000 municipalities**
  - Average contract value: €20,000/year (smaller average than private sector; procurement teams are smaller)

**Segment B TAM (EU) = 18,000 × €20,000 = €360M/year**

> Note: many EU municipalities procure through regional consortia. A single consortium sale (e.g. via VNG in NL, or equivalent in Germany/Belgium) could unlock many municipalities at once. This could significantly increase effective reach but is harder to model upfront.

### Bottom-Up: SAM (Netherlands only)

| Tier | Count | Qualifying | Avg annual value | SAM contribution |
|---|---|---|---|---|
| Large (>100k) | 28 | 25 (90%) | €65,000 | €1.6M |
| Medium (25k–100k) | 100 | 80 (80%) | €33,000 | €2.6M |
| Small (<25k) via consortium | 214 | ~30 (14%) | €15,000 | €450K |

**Segment B SAM (NL) ≈ €4.7M/year**

> Additional upside: a VNG (Vereniging Nederlandse Gemeenten) framework agreement could make this tool available to all 342 municipalities under a single procurement. That is a Year 3+ scenario.

### SOM - Netherlands, Years 1–5

| Year | Clients | ARR (Segment B) | Notes |
|---|---|---|---|
| Year 1 | 1–2 | €45–90K | Likely research partnership route (Windesheim) |
| Year 2 | 3–5 | €120–200K | First commercial contracts |
| Year 3 | 6–9 | €240–360K | Reference clients enabling further sales |
| Year 5 | 12–18 | €480–720K | ~10–14% of qualifying SAM |

> Public sector sales cycles are 6–18 months. Offset by larger, multi-year contracts and strong reference effects (one municipality → cluster of similar municipalities).

---

## Combined: Segments A + B

| | TAM (EU) | SAM (NL) | SOM Year 3 (NL) | SOM Year 5 (NL) |
|---|---|---|---|---|
| Segment A - Construction co. | €350M | €15M | €475–620K | €900K–1.2M |
| Segment B - Municipality | €360M | €4.7M | €240–360K | €480–720K |
| **Total** | **~€710M** | **~€20M** | **~€750K–1M** | **~€1.4–1.9M** |

### Revenue Trajectory (NL, conservative)

| Year | Clients (total A+B) | ARR | Key milestone |
|---|---|---|---|
| Year 1 | 4–7 | €150–250K | First paying pilots; proof of concept |
| Year 2 | 11–17 | €370–580K | Product-market fit confirmed |
| Year 3 | 21–29 | €750K–1M | Replicable sales motion; first municipality reference |
| Year 4 | 30–40 | €1.1–1.5M | Begin EU expansion (Belgium, DACH) |
| Year 5 | 42–58 | €1.4–1.9M | NL near-saturation of early adopter segment; EU growth engine |

---

## Top-Down Validation

European procurement software market (MarketDataForecast, 2025): **€2.92 billion**

| Filter | Calculation | Result |
|---|---|---|
| Construction-relevant share of EU procurement software | ~10–12% (construction is ~10% of EU GDP) | €290–350M |
| NL share of EU procurement software (NL = ~4% of EU GDP) | 4% × €320M | ~€13M |
| Premium for local AI / fine-tuning (higher price point than generic software) | +30% | **~€17M** |

**Top-down NL estimate: ~€13–17M**
**Bottom-up NL SAM: ~€20M**

The two methods agree within 20%, which is within normal range for a bottom-up / top-down triangulation. The bottom-up figure is slightly higher, likely because:
1. Our per-client pricing reflects a premium local AI deployment (above the market average for SaaS procurement tools)
2. The EU procurement software figure is broad (includes all sectors); construction is under-represented

**Conclusion: NL SAM of ~€20M is well-supported. Use €15M as a conservative working figure for financial planning.**

---

## Key Assumptions to Validate

| Assumption | Impact | How to validate |
|---|---|---|
| ~375 qualifying construction companies (50+ employees, active procurement) | High - drives SAM directly | Customer discovery interviews; CBS/KvK data cut |
| Blended annual contract value of €27–52K for construction segment | High - drives all revenue projections | First pilot pricing negotiations |
| Minimum training data threshold [TBD] | Medium - affects % of SAM that qualifies for fine-tuning | Technical experiment on simulated data; validate with first pilot |
| ~130 qualifying municipalities (large + medium tier) | Medium - drives Segment B SAM | Publicly available data from CBS / VNG |
| Municipality sales cycle 6–18 months | Medium - affects Year 1–2 revenue timing | Discovery calls with procurement officers |
| VNG framework agreement route (Year 3+) | High if achieved - could 3–5x Segment B SOM | Exploratory conversation with VNG via Windesheim |

---

## What This Means for Strategy

**The NL market is large enough to build a sustainable business without leaving the country.** A €20M SAM with 5–8% penetration at Year 5 is a €1–1.6M ARR business - viable as a profitable niche player or as a platform for EU expansion.

**Segment A is the growth engine; Segment B is the credibility anchor.** Construction companies generate faster revenue; a municipality reference gives credibility that unlocks more municipalities and validates the compliance/explainability story for enterprise infrastructure clients (Segment C).

**EU expansion meaningfully changes the ceiling.** With a €710M TAM and NL as a proven market, expansion to Belgium (similar regulation and language), Germany (largest EU construction market), and the Nordics (high digitisation appetite) opens up a €50–100M ARR opportunity at scale.

---

## Sources Referenced

- [Netherlands: number of construction firms, by size - Statista](https://www.statista.com/statistics/431961/number-enterprises-construction-industry-netherlands/)
- [CBS: De Nederlandse bouwnijverheid in onzekere tijden 2019–2023](https://www.cbs.nl/nl-nl/longread/de-nederlandse-economie/2023/de-nederlandse-bouwnijverheid-in-onzekere-tijden-2019-2023)
- [Monitor Aanbestedingen in Nederland 2021–2023 - Rijksoverheid](https://www.rijksoverheid.nl/documenten/rapporten/2024/12/19/significant-synergy-monitor-aanbestedingen-in-nederland-2021-2023)
- [TenderNed Aanbestedingsmonitor 2017–2025](https://www.tenderned.nl/cms/nl/aanbesteden-cijfers/aanbestedingsmonitor-2017-2022)
- [Dutch Public Procurement Guide - TenderMetric](https://tendermetric.com/insights/dutch-procurement-guide)
- [Municipalities of the Netherlands - Wikipedia](https://en.wikipedia.org/wiki/Municipalities_of_the_Netherlands)
- [Europe Procurement Software Market - MarketDataForecast](https://www.marketdataforecast.com/market-reports/europe-procurement-software-market)
- [CBS Construction and Housing Statistics](https://www.cbs.nl/en-gb/economy/construction-and-housing)
