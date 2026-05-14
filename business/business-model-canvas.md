# Business Model Canvas
> AI-Powered Construction Procurement - v0.6 | Last updated: 2026-05-08

---

## 1. Customer Segments

### Primary (paying)
- Construction procurement managers
- Purchasing departments
- Project planners
- Supplier relationship managers
- Warehouse and inventory teams

### Organisational buyers
- Mid-size construction companies (50-500 employees) - fastest sales cycle, clearest ROI on procurement admin
- Dutch municipalities - compliance driver, 342 identical buyers; one reference unlocks many
- Large construction or infrastructure organisations (enterprise tier - higher data sovereignty needs; V2)

### Named prospects (pre-LOI)
- **ED. Züblin AG (STRABAG)** - insider contact: Dusko Stojanovic, Project Lead Bid Processing, Stuttgart. Practitioner of exactly what the product supports. Entry point: pilot client (Segment A/C) and/or grant industry partner.
- Dutch municipalities via Gerard Tunteler's HPE Ronde Tafel voor Gemeenten relationships (342 municipalities, direct access)

> Universities and research partners (Windesheim, Belgrade) are **Key Partners**, not customer segments. They provide accreditation, validation, and grant access.

---

## 2. Value Propositions

### Core: Local AI with a fine-tuned procurement model
- On-premise deployment - company data never leaves the client environment
- Fine-tuned model on client's own procurement and supplier data → domain-specific accuracy, fewer errors than a generic model
- Continuous improvement - each procurement cycle adds to the model's understanding of the client's specific supplier base, material categories, and past decisions; the model gets smarter over time without extra effort from the client
- Switching cost is structural: the fine-tuned model encodes the client's institutional procurement knowledge (preferred suppliers, historical decisions, material standards). Migrating to a competitor means rebuilding that knowledge from scratch. The moat is the accumulated data and domain training, not the software itself.
- Fine-tuning quality depends on construction domain depth - understanding Dutch specification standards (CROW RAW chapters, UAV conditions, CPR 2024 product categories, KOMO and SKG-IKOB certification structures). This is Nina's expertise and is not replicable by a generic AI vendor without equivalent domain knowledge.
- Potential for lightweight edge deployment (mobile subagents for field purchasing)

### Design philosophy: decision support, not autonomous AI
- The AI handles retrieval, ranking, scoring, and documentation - the procurement professional reviews and decides
- Not a generative AI making things up from a generic model; a fine-tuned process tool trained on real procurement data
- Output is a structured comparison with an explicit reasoning trail - designed for human review, management approval, and audit
- This framing is essential for public sector clients who are legally accountable for every procurement decision

### Procurement efficiency
- Faster material search and supplier comparison
- Less time digging through scattered supplier information
- Faster preparation of comparison reports
- Better material availability insight

### Decision quality
- Better matching between specifications and available materials
- Clear, structured comparison of price, delivery time, quality, reliability, and certifications
- Transparent, explainable output with full reasoning trail - not black-box AI
- Reduced risk of ordering the wrong material

### Data & control
- AI trained on the client's own ERP and procurement history
- Enriched with publicly available subsupplier data (locations, certifications, lead times) - scraped from public sources only, GDPR-compliant
- Where a supplier runs their own AI or API, richer structured data can be exchanged programmatically (future: supplier-side integrations)
- Full control over the model - no dependency on external APIs

---

## 3. Channels

| Phase | Channel |
|-------|---------|
| Awareness | LinkedIn, website, construction sector events |
| Awareness | Windesheim / Value Chain Hackers network |
| Evaluation | Pilot projects with real procurement cases |
| Evaluation | Demonstrations with real procurement cases |
| Evaluation | Procurement workshops |
| Purchase | Direct outreach to construction companies |
| Partnership | Supplier network introductions |
| Partnership | ERP / procurement system integrators |

---

## 4. Customer Relationships

- Co-creation with procurement teams during onboarding
- Fine-tuning the model on the client's own data (high-touch, high-value)
- Training and onboarding for procurement staff
- Continuous model improvement as new supplier data comes in
- Trust-building through explainable AI results
- Long-term support contract and model maintenance
- Workshops around procurement workflow improvement

---

## 5. Revenue Streams

### Pre-product (now - before the AI platform is built)
| Stream | Stage | Type | Notes |
|--------|-------|------|-------|
| **Procurement simulation workshops** | Pre-product | One-time / recurring | Run interactive simulations that make procurement pain visible - like the Beer Game does for supply chain. Generates immediate revenue, funds early development, and is disguised customer discovery. Christiaan's core skill set. |
| **Procurement process consulting** | Pre-product | Project-based | Map and assess a client's procurement workflow; deliver a report with recommendations. Seeds the relationship for the AI product pitch. |
| **Research and innovation funding (grants)** | Pre-product / early | Institutional | Separate track - RAAK-PRO, Horizon Europe, NWO-KIEM. Requires named industry partner (Züblin is a candidate) + Windesheim. Not operating revenue. |

### Product (once pilot is running)
| Stream | Stage | Type | Notes |
|--------|-------|------|-------|
| Paid pilot | Early | One-time | First engagement - scoped project, proves value before full implementation |
| **Implementation fee** | Early / growth | One-time | Full delivery: ERP integration, data ingestion, fine-tuning, deployment, handover - client owns everything |
| **Annual maintenance contract** | Growth | Recurring (optional) | Software updates, support SLA, minor iterations - ~15% of implementation fee; client-initiated |
| **Retraining engagement** | Growth | Project-based | Full model refresh when client data has grown or categories expand - client-initiated |
| Custom integration work | Any | Project-based | ERP connectors, procurement system adapters beyond standard scope |
| Procurement data cleanup service | Any | Project-based | Pre-implementation data structuring for clients with messy procurement history |
| **Managed service (alternative tier)** | Growth | Recurring | Hosted subscription for clients without IT infrastructure to self-host - higher cost, more legal complexity; not the default |

> **No subscription in the default model.** The client owns the deployed system completely. Maintenance and retraining are purchased because they are genuinely useful - not because they are required for the system to function. This removes vendor dependency, simplifies the legal profile (no data processing agreement needed), and fits how municipalities and construction companies already procure enterprise software: as implementations, not SaaS.

> **Strategic note on workshops:** The simulation/workshop track solves three problems at once. (1) Revenue before the product exists. (2) Customer discovery - every workshop is a paid conversation about the procurement workflow; the scenarios participants generate are real, not hypothetical. (3) Demo data - workshop scenarios from real procurement teams produce realistic material categories, supplier structures, and decision patterns that seed the synthetic dataset used in pre-sales demos. This breaks the chicken-and-egg: a demo trained on workshop-derived scenarios is credible because it reflects real procurement logic, not fabricated data. Build the workshop programme as if it's a product in its own right.

---

## 6. Key Resources

### Data
- Client's own ERP and procurement history (brought in during onboarding)
- **Minimum viable dataset: [TBD] months of procurement history** - threshold at which fine-tuning demonstrably outperforms a general model; qualify prospects against this
- Publicly available supplier data from structured registries: KvK (Chamber of Commerce), certification body registers (KOMO, SKG-IKOB, Kiwa, BRL scheme registers), and open government datasets. These are designed for public use and carry no database rights risk.
- **Legal note on scraping:** "Publicly accessible" is not the same as "legally usable." EU Directive 96/9/EC grants sui generis database rights to any database requiring substantial investment - supplier catalogues, proprietary certification lists, and product spec sheets qualify. The data strategy relies on structured public registries and supplier-submitted data, not wholesale scraping of supplier websites. Legal review required before any automated data collection beyond KvK and certification body APIs.
- Simulated/synthetic procurement datasets for demo and pre-sales purposes - generated from Nina's domain knowledge and Christiaan's workshop scenarios to be realistic enough to demonstrate spec matching on real Dutch material categories
- Material specifications and certification data
- Supplier reliability signals
- Future: structured supplier data via supplier-side AI or API integrations

### AI / Technical
- Fine-tuning pipeline for domain-specific procurement models
- Local model deployment capability (on-premise, edge-ready)
- Specification-to-material matching logic
- Comparison and scoring framework

### Human / domain
- **Nina Gluhovic: Dutch and EU construction specification domain knowledge** - CROW RAW chapters, UAV contractual conditions, CPR 2024/3110 product categories, KOMO and SKG-IKOB certification structures, structural materials specification. This is what makes the fine-tuning accurate rather than generic. A horizontal AI vendor cannot replicate this without equivalent domain expertise.
- Christiaan's procurement workflow and simulation expertise - shapes how the tool fits actual procurement processes
- Procurement workflow templates
- User feedback loop from purchasing teams

### Network
- University partners (Windesheim, Belgrade) - validation and grant access
- Construction company partners - early adopters and co-creators
- Supplier network

---

## 7. Key Activities

- Customer discovery and procurement workflow mapping
- Client data ingestion, cleaning, and standardisation
- **Determining and validating the minimum training data threshold** (research activity - outcome feeds product qualification and pitch)
- Collecting supplier data from structured public registries (KvK, certification body registers) - scoped to sources with clear legal basis
- Fine-tuning AI model on client-specific procurement data
- Synthetic dataset generation for demos and pre-sales
- Local model deployment and infrastructure setup
- Specification-to-material matching engine development
- Comparison report generation
- Certification and paperwork checking
- Approval workflow design and integration
- Pilot testing and iteration
- ERP / procurement system integration
- Model maintenance and retraining

---

## 8. Key Partners

| Partner | Role |
|---------|------|
| Construction companies | Early adopters, co-creation, distribution |
| **ED. Züblin AG (STRABAG)** | **Named industry partner for grant applications; potential pilot client (large Segment A/C); insider contact via Milan** |
| Material suppliers | Data source, credibility, network |
| Windesheim University | Accreditation, validation, grant access, talent |
| Belgrade University | R&D, talent, additional grant access |
| HPE / Gerard's municipality network | Distribution into Segment B via HPE Ronde Tafel voor Gemeenten |
| ERP / procurement system providers | Integration, route to market |
| AI and data specialists | Fine-tuning and infrastructure capability |
| Industry associations | Credibility, events, distribution |

---

## 9. Cost Structure

| Cost item | Type | Notes |
|-----------|------|-------|
| Software development | Fixed | Core platform |
| Fine-tuning pipeline development | Fixed | One-time build, ongoing iteration |
| Data cleaning and integration | Variable | Per client onboarding |
| Subsupplier data scraping and maintenance | Variable | Ongoing |
| Local infrastructure setup per client | Variable | Hardware or VM provisioning |
| AI model maintenance and retraining | Variable | Per client, ongoing |
| Customer pilots and workshops | Variable | |
| Procurement domain research | Fixed | |
| Sales and onboarding | Variable | |
| Support and maintenance | Fixed | |
| ERP integration work | Variable | Per client |

---

## Strategic Decisions Locked

| Decision | Rationale |
|----------|-----------|
| Local / on-premise deployment as core product | Data sovereignty, reduced hallucination, client lock-in |
| Fine-tuned model per client | Domain accuracy + switching cost. The moat is Nina's Dutch construction domain expertise making the fine-tuning accurate - not the fine-tuning mechanism itself, which any competitor could copy. Domain depth is the differentiator. |
| Data = client ERP + structured public registries (KvK, certification body registers) | Solves data sourcing gap without database rights exposure; client owns their data; legally grounded |
| Synthetic data for demos seeded by workshop scenarios | Workshops generate real procurement logic (material categories, supplier structures) that make the synthetic demo credible; breaks the chicken-and-egg between needing client data to demo and needing a demo to get client data |
| Minimum training data threshold (TBD) | Qualifies prospects, sets expectations, becomes a credibility argument in pitch |
| Simulation/workshop programme as pre-product revenue | Generates cashflow before product is built; customer discovery in disguise; warms leads for the AI pitch |
| Züblin as named grant partner | Provides the industry partner slot required for RAAK-PRO and Horizon Europe applications; also a potential large pilot client |
| Supplier-side AI/API integrations | Future path to richer data without scraping; network effect if suppliers adopt |
| Universities as Key Partners, not customers | Accreditation, validation, grant access - not revenue |
| Edge/mobile deployment (subagents) | Future direction - field purchasing use case |

---

## Resolved Decisions

| Decision | Resolution |
|----------|------------|
| Segment priority | Mid-size construction companies (Segment A) first - fastest sales cycle (1-3 months), clearest ROI. Municipalities (Segment B) in parallel where Gerard opens the door. Enterprise (Segment C) after proof of concept. |
| Grant priority | MIT R&D AI Samenwerkingsprojecten first (deadline May 26, 2026 - needs SME co-applicant). KIEM Arbeidsbesparende AI in Sep 2026. RAAK-PRO only once product is live with a pilot reference. |
| Supplier-side AI / edge deployment | V2 features. Not on the V1 roadmap. |

---

## Customer Discovery Action Plan

These are not open questions - they are assumptions that need to be validated in the next 10 customer discovery conversations. Conversations to be led by Christiaan (construction segment) and Gerard (municipality segment).

| Assumption to validate | How to test | Target |
|------------------------|-------------|--------|
| Minimum training data threshold: how much ERP history is enough for fine-tuning to beat a generic model? | Ask procurement managers how many years of structured order data they have; test with Milan on a sample dataset | Answer in hand before first pilot scoping |
| ERP systems in target construction companies: Exact Online, SAP, Unit4, or other? | Ask in discovery calls - "what does your procurement data live in?" | Determines integration priority; Exact Online most likely for NL mid-size |
| Full software stack beyond ERP: what procurement tools, supplier portals, approval workflows, and document management systems do they already use? | Map the full tool stack in every discovery call - "walk me through how a procurement decision gets made, start to finish, and what software you touch" | Stack map for at least 5 companies before product scoping begins |
| AI layer vs. new deployment: would procurement teams prefer an AI capability added to their existing software over a new locally deployed system? | Ask directly - "if your current ERP could do this, would you prefer that over a separate tool?" | Determines whether the product is a standalone or an integration/plugin |
| Who is the actual end user vs. the buyer: does the procurement manager doing the daily work want this, or only the manager above them? | In discovery calls, speak to both levels separately - the procurement manager and their direct superior | Do not sign a pilot without having spoken directly to the person who will use the system daily |
| Real sales cycle length: how long does it actually take a mid-size construction company to evaluate and adopt new procurement software? | Ask about the last time they adopted a new digital tool - "how long did that take from first conversation to go-live?" | Adjust financial model runway assumptions if answer is consistently above 6 months |
| Entry point scope: is bid comparison / supplier evaluation the right single starting problem, or is there a more painful, more bounded entry point? | Ask "what is the single most painful moment in your procurement week?" - listen for what comes first, unprompted | Identify one specific workflow before scoping the pilot |
| Willingness to pay for a scoped pilot before full implementation | Present a pilot proposal in discovery call and ask for a conditional yes | 3 signed LOIs or pilot agreements by [target date] |
| Züblin as pilot client: Dusko Stojanovic's role and procurement pain | Christiaan + Milan meeting with Dusko to qualify - is the entry point a pilot, a grant co-application, or both? | Meeting held, role and interest confirmed |
| Workshop format: does a 2-4 hour procurement simulation make the cost of bad procurement viscerally obvious? | Run a first pilot workshop with a willing construction company and debrief | First workshop delivered; warm lead for pilot generated |

---

## Critical Open Challenges (raised 2026-05-14)

These are structural risks raised by Kirsten Coppoolse that are not yet resolved. They must be addressed before the first pilot agreement is signed.

| Challenge | What is at stake | Owner | Status |
|---|---|---|---|
| **Liability for AI recommendations** | If the system recommends a supplier that fails - wrong material, late delivery, uncertified product - who is legally responsible? The product, the company, or the procurement manager who approved it? "The human decides" is a design principle, not a legal answer. | Christiaan + legal counsel | Open - legal review required |
| **Data boundary and security** | What data does the system actually touch? ERP procurement history, supplier contacts, order values, contract terms - some of this is commercially sensitive, some may be personal data under GDPR. A data boundary document does not exist. | Milan + Kirsten | Open - define before any pilot data ingestion |
| **User adoption vs. buyer adoption** | The buyer (management) and the user (the procurement manager in the spreadsheet) are different people. The buyer may approve it; the user may resist it. Construction industry moves slowly; end users are often experienced practitioners who have worked the same way for decades. Change management is not addressed in the product or go-to-market plan. | Christiaan + Kirsten | Open - requires user-level discovery conversations |
| **Sales cycle realism** | The financial model assumes 1-3 month sales cycles for mid-size construction. This may be optimistic for an industry known for slow technology adoption. If cycles are 6-12 months, runway calculations change materially. | Kirsten + Christiaan | Open - validate in discovery calls |
| **Scope discipline** | The current product scope covers supplier comparison, certification tracking, and audit reporting. There is a risk of expanding into the full supply chain before proving value in one narrow workflow. The entry point should be one specific pain, proved end-to-end, before expansion. | Milan + Christiaan | Open - define MVP scope explicitly |
