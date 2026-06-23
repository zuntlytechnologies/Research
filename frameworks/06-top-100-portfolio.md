# 06 — Top 100 Opportunity Portfolio (Living Tracker)

> **Purpose.** A single, continuously-updated, ranked inventory of every qualified opportunity discovered across all 30 sections. This is the **output artifact** of the entire research program. It is re-ranked as evidence arrives. Sections 1–13/14 *populate* it; Sections 24–30 *re-rank and synthesize* it.

---

## Part A — Column schema (every opportunity row carries these)

| Field | Meaning |
|-------|---------|
| **ID** | Stable code: `OPP-NN` |
| **Opportunity** | Short name |
| **Problem** | The pain, in customer terms |
| **Customer / Segment** | Who buys; which pharma segment |
| **User / Buyer / Budget owner** | Who uses / signs / owns budget |
| **Existing solutions** | Incumbents + "do nothing / Excel + consultant" |
| **Business model (03)** | Primary + secondary archetypes |
| **Opportunity type (02E)** | Fast revenue / Platform / Hardware / Fintech / Marketplace / Export / Long-term strategic / Avoid |
| **TAM estimate** | Range, sourced or `[ASSUMPTION]` |
| **Reg complexity** | Low / Med / High |
| **Capital band (05A)** | C1–C5 (+ phased note) |
| **TTF revenue / TT scale (05B)** | T-band each |
| **Applicability** | AI / SaaS / HW / Infra / Services / Export / Marketplace (H/M/L each) |
| **Competitive intensity** | Low / Med / High |
| **Moat potential** | Low / Med / High |
| **Founder fit (04)** | 1–10 + lead/hire/partner/phase/avoid |
| **Expertise to hire** | Roles |
| **Partnership required** | Assets/partners |
| **Attractiveness / Risk (05)** | 0–100 each |
| **Priority** | High / Med / Low / Avoid |
| **Source section** | Where it was discovered |
| **Status** | Idea / Validating / Shortlist / Parked / Rejected (+reason) |

> Because a flat 24-column table is unreadable in Markdown, each opportunity is maintained as a **compact card** below, and the **ranking table** (Part C) holds the key comparison columns. Full scorecards live in the originating section file.

---

## Part B — Theme buckets (for navigation as the list grows toward 100)

1. **RegTech & Compliance** (S6, S10, S17, S18, S20, S23)
2. **Export & Dossier Intelligence** (S13, S23)
3. **Quality & Audit Services-to-Platform** (S10, S17)
4. **Supply Chain, Cold Chain & Track-and-Trace** (S12, S20)
5. **Pharma Fintech & Working Capital** (S12, S16)
6. **Commercial, Tender & Channel Intelligence** (S11, S21)
7. **Manufacturing 4.0 & Facility Support** (S9)
8. **CDMO/CRO Enablement & Marketplaces** (S4, S22)
9. **API Sourcing & Procurement** (S7, S12)
10. **PV / Medical Affairs / Clinical Data** (S4, S18, S19)
11. **Data Networks & Intelligence** (S5, S21)
12. **Training & Workforce Enablement** (cross-cut)

---

## Part C — Ranking table (re-sorted each update by Attractiveness, then Founder fit)

> Status after Section 1: these are **macro-level seed theses** identified from industry structure. They will be split, sharpened, scored precisely, and re-ranked as their home sections are executed. Scores below are **preliminary directional** estimates pending section deep-dives.

| ID | Opportunity | Bucket | Model (primary) | Type | Capital | TTF rev | Founder fit | Attractiveness (prelim) | Priority (prelim) | Home section |
|----|-------------|--------|-----------------|------|---------|---------|-------------|--------------------------|-------------------|--------------|
| OPP-01 | Export registration & dossier-lifecycle intelligence platform | Export | Data intelligence | Platform | C2 | T2 | 9 | ~80 | High | S23/S13 |
| OPP-02 | Managed regulatory affairs + RegTech for mid-market exporters | RegTech | Managed services→SaaS | Platform | C2 | T2 | 8 | ~76 | High | S6/S23 |
| OPP-03 | Tender & govt-procurement intelligence (India + export tender markets) | Commercial | Data intelligence | Platform | C2 | T2 | 8 | ~75 | High | S11/S13 |
| OPP-04 | Distributor / channel working-capital financing | Fintech | Pharma fintech | Fintech | C3 (phase C2) | T2 | 8 | ~74 | High | S12/S16 |
| OPP-05 | Cold-chain IoT monitoring + analytics for distribution/exports | Cold chain | IoT/device→SaaS | Hardware-enabled | C2/C3 | T2 | 7 | ~72 | High | S12/S20 |
| OPP-06 | Serialization / track-and-trace compliance for exporters | Track & trace | Hybrid SW+compliance | Platform | C2 | T2 | 8 | ~72 | High | S20 |
| OPP-07 | Managed pharmacovigilance (case processing + signal AI) | PV | Managed services→AI | Platform | C2 | T2 | 7 | ~70 | High | S18 |
| OPP-08 | Audit-readiness & data-integrity managed compliance | Quality | Managed services→SaaS | Platform | C2 | T2 | 8 | ~70 | High | S10/S17 |
| OPP-09 | API/raw-material sourcing & vendor-qualification marketplace+intel | API sourcing | Marketplace+data | Marketplace | C2/C3 | T2 | 7 | ~68 | Medium | S7/S12 |
| OPP-10 | Mid-market India QMS / eQMS SaaS (Veeva/MasterControl gap) | RegTech | SaaS | Platform | C2 | T2 | 8 | ~68 | Medium | S15/S10 |
| OPP-11 | CDMO/CRO capacity discovery & RFQ marketplace + tech-transfer tooling | CDMO | Marketplace+SaaS | Marketplace | C2 | T2–T3 | 7 | ~66 | Medium | S22 |
| OPP-12 | Export receivable / trade financing for pharma exporters | Fintech | Pharma fintech | Fintech | C3 | T2 | 7 | ~66 | Medium | S13/S16 |
| OPP-13 | Plant/facility digital ops: calibration, validation, maintenance SaaS | Mfg 4.0 | SaaS (+IoT) | Platform | C2 | T2 | 7 | ~64 | Medium | S9 |
| OPP-14 | Pharma workforce training & GxP certification + placement | Training | Training/workforce | Long-term strategic | C1/C2 | T1–T2 | 7 | ~62 | Medium | cross-cut |
| OPP-15 | Channel sell-out / distributor reconciliation & inventory visibility | Supply chain | SaaS+data | Platform | C2 | T2 | 7 | ~62 | Medium | S12 |

*(Target: grow to ~100 rows; maintain Top 15–20 as the actively-tracked shortlist. Each row gets a full scorecard in its home section.)*

---

## Part D — Compact cards (seeded — full detail to come in home sections)

### OPP-01 — Export registration & dossier-lifecycle intelligence platform
- **Problem:** Mid-market exporters decide *which product to register in which country* and manage dossiers, variations, renewals via Excel + email + local agents + shared drives. Decisions are slow, blind, and error-prone; missed renewals = lost market access.
- **Why now:** India exports ~US$27–28B (FY24, directional; Pharmexcil/DGCIS) and is pushing into more regulated/semi-regulated markets; data is fragmented.
- **Model:** Services-first (do registrations) → accumulate registration/competitor/country data → sell intelligence + lifecycle SaaS. Hybrid: Data intelligence + Services + SaaS.
- **Founder fit 9/10:** Lead directly; hire RA specialists + country consultants; partner with local agents.
- **Why it could fail:** Data acquisition is hard; agents guard relationships; sales cycles long. → mitigated by services beachhead.

### OPP-04 — Distributor / channel working-capital financing
- **Problem:** Stockists/distributors run on 30–90 day credit; working capital is trapped across the chain; retailers and distributors are chronically under-financed; banks lack pharma-specific underwriting data.
- **Model:** Originate via channel/ERP/marketplace data → finance receivables/inventory (NBFC partner or co-lending). Marketplace→Fintech.
- **Founder fit 8/10:** Native finance fit; needs lending capital partner + risk hire. Phase: start as origination SaaS / data, then add the book.
- **Why it could fail:** Credit losses, capital cost, distribution; needs proprietary data edge.

### OPP-05 — Cold-chain IoT monitoring + analytics
- **Problem:** Temperature excursions in transit/storage are tracked manually or with dumb loggers; excursion data is reconstructed after the fact; biologics/vaccines/insulin at risk; export buyers increasingly demand digital cold-chain proof.
- **Model:** Razor-blade — sensors/devices near cost + recurring connectivity/SaaS + data network. Hardware-enabled→Data→SaaS.
- **Founder fit 7/10:** Needs hardware partner/OEM; founder owns software/data/GTM/compliance. Phase: pilot fleets, then scale.
- **Why it could fail:** Hardware logistics, commoditized loggers, thin margins if no recurring layer.

*(Remaining seed opportunities OPP-02, 03, 06–15 carry analogous cards; they are expanded with full `05` scorecards in their home sections.)*

---

## Part E — Update protocol

1. After each section, **add** new opportunities as cards + ranking rows.
2. **Re-score** affected existing rows with section evidence.
3. **Re-sort** Part C by Attractiveness, tie-break Founder fit, then lower Capital band.
4. Maintain a **Top 15–20 shortlist** as the active hunting ground.
5. In Section 30, converge to **3 wedge candidates** + a 90-day validation plan.
