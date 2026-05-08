# Shared Value Map
> AI-Powered Construction Procurement | Last updated: 2026-05-08
>
> This is the constant side of the Value Proposition Canvas.
> It describes what we offer, how we relieve pains, and how we create gains.
> Customer Profiles (jobs, pains, gains) are in separate per-segment files.

---

## Products & Services

### Core: Local AI Procurement Assistant
A fine-tuned AI model deployed on the client's own infrastructure (on-premise or private cloud). The model is trained on the client's historical procurement data — orders, suppliers, materials, certifications — and enriched with publicly available subsupplier data. It runs without sending data to external APIs.

### Specification-to-Material Matching Engine
Translates a procurement specification (material type, grade, dimensions, certifications required, delivery window) into a ranked list of matching suppliers and materials from the client's supplier database and enriched external data.

### Automated Supplier Comparison Report
Generates a structured comparison across multiple suppliers on: price, delivery time, quality indicators, reliability history, certifications held, and sustainability credentials. Output is human-readable and audit-ready.

### Certification & Compliance Checker
Automatically verifies whether a supplier's certifications are current, complete, and match the specification requirements. Flags expiring or missing certifications before an order is placed.

### Explainable Recommendations
Every recommendation includes a cited reasoning trail: which criteria drove the ranking, which data points were used, and where the data came from. Designed to support human review and defensible decisions.

### Approval Workflow Integration
Routes comparison reports and recommendations through the client's existing approval process. Configurable for single-buyer sign-off or multi-level authorisation.

### ERP / Procurement System Integration
Connects to the client's existing ERP or procurement platform (e.g. SAP, Exact, Unit4) to ingest order history and push approved decisions back into the system of record.

### Demo & Simulation Environment
A pre-configured environment using synthetic procurement data that replicates real procurement scenarios. Used in pre-sales and onboarding before the client's own data is integrated.

### Model Maintenance & Retraining Service
Scheduled retraining of the client's model as new procurement data accumulates. Includes data quality checks, performance benchmarking against the previous version, and a changelog of what the model has learned.

### (Roadmap) Edge / Mobile Subagents
Lightweight model variants deployable on tablets or phones for field purchasing — enabling on-site material sourcing decisions without a connection back to central infrastructure.

---

## Pain Relievers

| Pain relieved | How we relieve it | Relevant segments |
|---|---|---|
| Supplier information is scattered across email, Excel, portals, and phone calls | Single unified search across all integrated supplier and material data | A, B, C, D |
| Comparing suppliers manually is slow and error-prone | Automated comparison report generated in seconds from a specification input | A, B, C, D |
| Certificates expire or are missing — discovered too late | Certification checker runs at query time and flags gaps before ordering | A, B, C |
| Procurement knowledge is concentrated in one person | Fine-tuned model encodes past procurement decisions and supplier logic | A, C |
| Hard to justify or document why a supplier was chosen | Explainable AI with full reasoning trail and cited data sources | A, B, C |
| Fear that AI will hallucinate or give wrong material matches | Model fine-tuned on client's own domain data; outputs grounded in real supplier records | A, B, C, D |
| Concern about sensitive procurement data leaving the organisation | On-premise deployment — model and data stay within client infrastructure | A, B, C |
| New team members take months to get productive | AI encodes institutional knowledge; onboarding accelerated by guided search | A, C |
| Difficult to include sustainability criteria consistently | Scoring framework includes configurable sustainability and circularity weighting | B, C |
| Long lead times cause project delays | Material availability and lead time data visible at search time | A, C, D |
| Hard to discover suppliers beyond existing relationships | Matching engine surfaces qualified alternatives from enriched supplier database | A, B, D, E |

---

## Gain Creators

| Gain created | How we create it | Relevant segments |
|---|---|---|
| Faster procurement cycles — from specification to approved order | Automated matching, comparison, and routing replaces days of manual work | A, B, D |
| Better supplier decisions — more criteria, less bias | Multi-criteria scoring across price, quality, reliability, certs, sustainability | A, B, C |
| Institutional procurement knowledge retained and shareable | Model captures decision logic from historical data; survives staff turnover | A, C |
| Audit-ready documentation on every decision | Auto-generated comparison report serves as a complete procurement record | A, B, C |
| Reduced dependency on external AI providers | Local model with no API calls; no per-query cost; no third-party data exposure | A, B, C |
| Continuous improvement as data grows | Model retrains on new procurement history; gets more accurate over time | A, C |
| Broader supplier visibility beyond incumbent relationships | Enriched subsupplier database surfaces alternatives the buyer may not know | A, B, D |
| Compliance confidence | Spec matching aligned to regulatory and certification requirements | B, C |
| Explainable, defensible recommendations | Reasoning trail supports review by managers, auditors, and elected officials | B, C |
| Data ownership and sovereignty | Client owns their model, their data, and their supplier intelligence | A, B, C |

---

## Value Proposition Statement (generic)

> We give construction procurement teams a locally deployed, fine-tuned AI that matches materials to specifications, compares suppliers on every relevant dimension, and generates audit-ready reports — all without their data leaving their own infrastructure.
