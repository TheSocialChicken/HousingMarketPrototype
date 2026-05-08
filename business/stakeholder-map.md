# Stakeholder Map
> AI-Powered Construction Procurement | Last updated: 2026-05-08
>
> Status: DRAFT — incomplete. Task is to review all candidate stakeholders, decide their role (customer segment, channel partner, data partner, regulatory body), and create value proposition canvases for any confirmed new segments.

---

## Currently Documented Segments

| Segment | File | Role | Priority |
|---|---|---|---|
| A — Construction company (procurement team) | [vpc-a](value-propositions/vpc-a-construction-company.md) | Primary customer | **Launch now** |
| B — Municipality / local government | [vpc-b](value-propositions/vpc-b-municipality.md) | Primary customer | **Launch now** |
| C — Large infrastructure organisation | [vpc-c](value-propositions/vpc-c-infrastructure-org.md) | Customer (V2) | Enterprise tier |
| D — Project developer / real estate developer | [vpc-d](value-propositions/vpc-d-project-developer.md) | Customer (V2) | Tertiary |
| E — Material supplier | [vpc-e](value-propositions/vpc-e-material-supplier.md) | Data partner (now) / potential customer (V2) | Start unpaid |

---

## Unstudied Candidates — Needs Review

The following stakeholder types were identified in conversation (2026-05-08) as potentially missing from the current map. For each: decide the role, assess fit, and create a VPC if they qualify as a customer segment.

---

### 1. Auditors and Certification Bodies

**Examples:** Kiwa, TÜV Rheinland, Lloyd's Register, SGS, Bureau Veritas, DNV

**Why they came up:**
Construction procurement involves verifying that suppliers hold current certificates for materials, processes, and sustainability claims. Right now this verification is manual — buyers chase certificates per order. Certification bodies are the authoritative source of that data.

**Possible roles:**
- **Data partner:** Certification bodies could provide a live API or data feed of valid certificates, replacing manual verification. This would make the certification checker feature dramatically more reliable.
- **Channel partner:** Certification bodies already have relationships with the construction companies and municipalities that are the product's target customers. They could introduce or co-sell.
- **Customer:** Could a certification body want the product to improve their own internal procurement? Less obvious, but worth asking.

**Open questions:**
- Do Kiwa, TÜV etc. have APIs or data licensing arrangements that could feed a certification checker?
- Are they interested in a distribution partnership — i.e. recommending the product to their construction company clients?
- Does the new CPR 2024/3110 regulation (mandatory environmental performance indicators from Jan 2026, requiring accredited lab testing) create a new urgency for certification data integration?

**Decision needed:** Data partner / channel partner / customer segment / not relevant

---

### 2. Trucking and Logistics Companies

**Examples:** Van den Bosch, Vos Logistics, Jan de Rijk, Rhenus, DSV (construction materials division)

**Why they came up:**
Construction procurement doesn't end at order placement — delivery reliability is a critical part of supplier evaluation. Late delivery = project delay = cost overrun. A supplier comparison that includes delivery performance data would be more useful than one that only covers price and certification.

**Possible roles:**
- **Data partner:** Logistics providers hold delivery performance data that could enrich supplier scoring (on-time delivery rates, damage rates, lead time variance).
- **Customer (V2):** Trucking companies have their own procurement needs (fuel, tyres, parts, subcontractors). The product could be adapted. But this is a different domain and a different product — likely out of scope.

**Open questions:**
- Is delivery performance data accessible or shareable from logistics providers?
- Do construction procurement teams currently factor delivery reliability into supplier selection — and if so, how?
- Is this a V1 feature (integrate delivery data into scoring) or a V2/V3 roadmap item?

**Decision needed:** Data partner (for delivery scoring) / out of scope for now

---

### 3. Material Component Manufacturers

**Examples:** Saint-Gobain, Knauf, Rockwool, Kingspan, Lafarge Holcim (cement), Arcelor Mittal (steel)

**Why they came up:**
Segment E (material supplier) currently treats suppliers as **data partners** — they contribute their product catalogue and certification data to the matching engine. But large manufacturers have their own procurement operations: they buy raw materials, components, and subcontracted services at scale. Could they be **customers** of the procurement AI, not just data contributors?

**Possible roles:**
- **Data partner (current plan):** Onboard supplier catalogues early, unpaid, to build the matching engine. This is already in the VPC.
- **Customer — own procurement:** A manufacturer like Knauf or Saint-Gobain buying raw materials (gypsum, glass wool, steel) has procurement teams with the same pains as a construction company. The product may be adaptable.
- **Channel partner:** Manufacturers who are in the product catalogue could recommend the tool to their construction company customers ("our products are in the database — use this tool to find and compare us").

**Open questions:**
- Do large material manufacturers have procurement teams with the same pain profile as construction companies? What's different?
- Is the procurement domain (raw materials for manufacturing) meaningfully different from the domain (construction materials for building) — would the same model work, or would separate fine-tuning be needed?
- Is the manufacturer-as-channel-partner angle worth pursuing early to build catalogue density?

**Decision needed:** Separate customer segment (V2) / channel partner / data partner only / out of scope

---

### 4. CO₂ and Sustainability Bodies

**Examples:** Dutch Green Building Council (DGBC), MilieuCentraal, RVO (Rijksdienst voor Ondernemend Nederland), SBK (Stichting Bouwkwaliteit), Nederlandse Emissieautoriteit (NEa)

**Why they came up:**
Sustainability and CO₂ reduction is increasingly embedded in Dutch construction procurement — not as an optional add-on but as a legal and policy requirement. Several layers:

- **Dutch municipalities** are required to apply MVO (Maatschappelijk Verantwoord Ondernemen), circularity, and SROI criteria in procurement decisions. This is already in vpc-b.
- **CPR 2024/3110** (EU Construction Products Regulation, operational Jan 2026) adds mandatory environmental performance indicators for all construction products. This is already in vpc-b.
- **Large construction companies** are subject to CSRD (Corporate Sustainability Reporting Directive) from 2026 — they must report Scope 3 emissions, which includes supplier emissions. Procurement is a Scope 3 source.

**Possible roles:**
- **Regulatory context (not a customer):** The sustainability compliance layer is a feature requirement, not a separate customer segment. The product needs to score suppliers on CO₂/environmental criteria because buyers are legally required to consider it — not because sustainability bodies are customers.
- **Data partner:** SBK maintains the Nationale Milieudatabase (NMD) — the Dutch database of environmental performance data for construction products (EPDs). This is the authoritative data source for environmental scoring in Dutch construction procurement. Integrating NMD data would make the product's sustainability scoring credible and legally defensible.
- **Channel partner / credibility:** DGBC and RVO relationships could validate the product's sustainability credentials and open doors with sustainability-forward buyers.

**Open questions:**
- Is NMD (Nationale Milieudatabase / SBK) accessible via API or data licensing? This is the highest-priority data integration question for sustainability scoring.
- Does CSRD Scope 3 reporting create a procurement data need that the product can directly address — i.e. can clients use procurement records from the product to generate Scope 3 reports?
- Are sustainability bodies (DGBC, RVO) worth approaching as channel or credibility partners, or is the regulatory compliance layer sufficient to address this without formal partnerships?

**Decision needed:** Feature requirement (already planned) + NMD data partner (pursue) + CSRD Scope 3 angle (evaluate as gain creator in vpc-a)

---

## Review Checklist

- [ ] Auditors/certification bodies — decide role; assess Kiwa/TÜV API or data licensing feasibility
- [ ] Trucking/logistics — decide if delivery performance data is a V1 or V2 feature; assess data accessibility
- [ ] Material manufacturers — decide if they qualify as a separate customer segment (V2); assess procurement pain overlap
- [ ] CO₂/sustainability bodies — confirm NMD data licensing feasibility; evaluate CSRD Scope 3 as a gain creator in vpc-a
- [ ] After review: update [value-proposition-canvas.md](value-proposition-canvas.md) segment table and create VPCs for any new confirmed segments
