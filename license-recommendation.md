# Software License Recommendation for Dundir

## The core question: where is the moat?

The moat is not the code. It is Nina's construction domain expertise calibrating the optimizer, the client's accumulated procurement data creating lock-in, and the objective function definition for Dutch construction procurement. A competitor taking the code still cannot replicate any of that. This changes the licensing calculus: locking up the code protects something that is not actually the competitive advantage, while losing the trust and transparency benefits that open code provides with conservative buyers like municipalities.

---

## Recommendation: AGPL-3.0 on the platform, dual license ready

### What AGPL-3.0 means

Anyone can use, modify, and distribute the code — but any derivative work, including running it as a hosted cloud service, must also be released under AGPL-3.0. This closes the most important loophole: a large competitor (Onventis, SAP, Oracle) cannot take the code, deploy it as a SaaS, and keep their modifications closed. The domain expertise and client data that constitute the actual moat remain fully proprietary.

### Why this fits Dundir specifically

**Municipalities and public sector clients** often prefer or require auditable, transparent code. AGPL directly supports this and removes a common objection in public procurement processes.

**Grant alignment** — Windesheim and Belgrade partnerships via Horizon Europe and RAAK-PRO align with open science principles. Open source strengthens grant applications and is increasingly expected by EU research funders.

**The code is not the moat** — opening it costs nothing competitively. What protects the business is the domain calibration, the client data, and the deployment and fine-tuning service — none of which are in the public repository.

**Competitor protection** — AGPL is the only open source license that prevents the cloud-service loophole. MIT and Apache 2.0 are too permissive; a well-funded competitor could take the codebase, wrap it, and compete directly.

### Dual license path

Keep AGPL as the default. Add a commercial license option for clients who cannot accept copyleft terms in a public procurement contract (some municipalities may have this constraint). This is the standard GitLab / MongoDB model: open source community gets AGPL, paying enterprise clients get commercial terms. Revenue from commercial licenses is a secondary stream; the primary protection is AGPL.

---

## Per-repo breakdown

| Repo | License | Rationale |
|---|---|---|
| `dundir/platform` | AGPL-3.0 (+ commercial exception) | Core product - open source with copyleft protection |
| `dundir/website` | MIT (code) / proprietary (content) | No competitive risk in the site code; content stays owned |
| `dundir/company` | Private - no license (proprietary by default) | Internal business docs, not for public distribution |
| `dundir/research` | To be decided with Windesheim / Belgrade | Grant terms may specify open access; confirm before publishing |

---

## What to do before applying the license

1. Milan to review and confirm he has no objection — as CTO he should sign off on the platform license
2. Check whether any dependencies the platform will use have license incompatibilities with AGPL (most ML/optimization libraries are compatible; confirm for any proprietary data connectors)
3. Draft a one-paragraph commercial license exception clause before the first enterprise pilot agreement is signed
4. Confirm with Windesheim legal whether RAAK-PRO grant terms impose any open access obligations on the research outputs

---

## Alternatives considered and rejected

| License | Reason rejected |
|---|---|
| Proprietary / All Rights Reserved | Protects something that is not the moat; loses transparency benefits with municipalities and grant bodies |
| MIT / Apache 2.0 | Too permissive — competitors can take the code and build a competing cloud product |
| Business Source License (BSL) | More complex and less understood; AGPL achieves the same protection with better ecosystem recognition |
| GPL-2.0 | Does not close the network/SaaS loophole that AGPL-3.0 was specifically designed to close |
