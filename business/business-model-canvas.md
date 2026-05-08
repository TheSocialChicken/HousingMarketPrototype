# Business Model Canvas
> AI-Powered Construction Procurement - v0.5 | Last updated: 2026-05-08

---

## 1. Customer Segments

### Primary (paying)
- Construction procurement managers
- Purchasing departments
- Project planners
- Supplier relationship managers
- Warehouse and inventory teams

### Organisational buyers
- Mid-size construction companies
- Large construction or infrastructure organisations (enterprise tier - higher data sovereignty needs)

> Universities and research partners (Windesheim, Belgrade) are **Key Partners**, not customer segments. They provide accreditation, validation, and grant access.

---

## 2. Value Propositions

### Core: Local AI with a fine-tuned procurement model
- On-premise deployment - company data never leaves the client environment
- Fine-tuned model on client's own procurement and supplier data → fewer hallucinations, domain-specific accuracy
- Proprietary model per client = switching cost and competitive lock-in
- Potential for lightweight edge deployment (mobile subagents for field purchasing)

### Procurement efficiency
- Faster material search and supplier comparison
- Less time digging through scattered supplier information
- Faster preparation of comparison reports
- Better material availability insight

### Decision quality
- Better matching between specifications and available materials
- Clear comparison of price, delivery time, quality, reliability, and certifications
- Explainable procurement recommendations
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

> **Strategic note on workshops:** The simulation/workshop track is not just a cashflow bridge - it is the fastest path to deeply understanding the procurement workflow problem from the inside. Every workshop delivered is a customer discovery session. Clients who go through a workshop are warm leads for the pilot. Build the workshop programme as if it's a product in its own right.

---

## 6. Key Resources

### Data
- Client's own ERP and procurement history (brought in during onboarding)
- **Minimum viable dataset: [TBD] months of procurement history** - threshold at which fine-tuning demonstrably outperforms a general model; qualify prospects against this
- Publicly scraped subsupplier data (locations, capacity, lead times, certifications) - public sources only, GDPR-compliant
- Simulated/synthetic procurement datasets for demo and pre-sales purposes
- Material specifications and certification data
- Supplier reliability signals
- Future: structured supplier data via supplier-side AI or API integrations

### AI / Technical
- Fine-tuning pipeline for domain-specific procurement models
- Local model deployment capability (on-premise, edge-ready)
- Specification-to-material matching logic
- Comparison and scoring framework

### Human / domain
- Procurement expertise and construction materials domain knowledge
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
- Scraping publicly available subsupplier data (GDPR-compliant)
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
| Fine-tuned model per client | Domain accuracy + switching cost moat |
| Data = client ERP + publicly scraped subsupplier data | Solves data sourcing gap; client owns their data; GDPR-compliant |
| Synthetic data for demos | Removes blocker to pre-sales; lets prospects see value before committing their data |
| Minimum training data threshold (TBD) | Qualifies prospects, sets expectations, becomes a credibility argument in pitch |
| Simulation/workshop programme as pre-product revenue | Generates cashflow before product is built; customer discovery in disguise; warms leads for the AI pitch |
| Züblin as named grant partner | Provides the industry partner slot required for RAAK-PRO and Horizon Europe applications; also a potential large pilot client |
| Supplier-side AI/API integrations | Future path to richer data without scraping; network effect if suppliers adopt |
| Universities as Key Partners, not customers | Accreditation, validation, grant access - not revenue |
| Edge/mobile deployment (subagents) | Future direction - field purchasing use case |

---

## Open Questions

1. **Segment priority:** Mid-size construction companies first (faster sales cycle) or large/enterprise (bigger deal size, more data)? Recommend starting with mid-size for product-market fit, then enterprise.
2. **Minimum training data threshold [research required]:** How much procurement history (orders, suppliers, materials) must a client provide before fine-tuning produces measurably better results than a general model? This number becomes a prospect qualification criterion and a pitch credibility argument: *"Give us X months of your data and we'll build a model that outperforms any generic AI on your specific materials."*
3. **ERP integration:** Which ERP systems are most common in your target construction companies (e.g. SAP, Exact, Unit4)? Determines integration priority and partner channel.
4. **Supplier-side AI timeline:** When is it realistic to integrate with suppliers who have their own AI or API? Likely a v2 feature; define what "supplier-side AI" means concretely.
5. **Mobile/edge timeline:** Is the phone-based subagent a v1 feature or a future roadmap item? Affects model size and architecture choices now.
6. **Grant strategy:** Züblin as named industry partner unlocks RAAK-PRO (requires HBO + industry partner). Horizon Europe bilateral NL–Serbia track is realistic with Windesheim + Belgrade. NWO-KIEM is a lighter entry point. Prioritise which to apply for first.
7. **Züblin relationship:** What is Milan's contact's role at Züblin? Procurement, IT, or innovation? This determines whether the entry point is a pilot client, a grant co-applicant, or both.
8. **Simulation/workshop programme design:** What does the procurement simulation look like? It should make the cost of bad procurement viscerally obvious - like the Beer Game does for the bullwhip effect. A 2–4 hour workshop format with a debrief selling the AI solution naturally.
