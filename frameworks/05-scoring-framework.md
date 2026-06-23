# 05 — Scoring Framework

> **Purpose.** A consistent, transparent way to score every opportunity so the Top 100 Portfolio can be ranked objectively. Defines the 1–10 dimensions, the capital bands, the timeline bands, and the formulas for **Attractiveness**, **Risk**, **Priority**, and **Opportunity Type**.

---

## Part A — Capital-requirement bands

| Band | Label | Range (INR) | Notes |
|------|-------|-------------|-------|
| C1 | Asset-light | < ₹1 crore | Software/services MVP, tiny team |
| C2 | Early-stage buildable | ₹1–5 crore | Real product + small ops/sales |
| C3 | Moderate capital | ₹5–25 crore | Lab, IoT fleet, fintech book seed, managed-ops scale |
| C4 | Heavy capital | ₹25 crore+ | Plant/infra, large balance sheet |
| C5 | Long-term infra/strategic | Phased, ₹25cr+ over years | Infrastructure-compounding, multi-round |

> Always note: *if C3+, what C1/C2 phased entry exists?*

---

## Part B — Timeline bands

| Band | Label | To first revenue |
|------|-------|------------------|
| T1 | Immediate revenue | 0–6 months |
| T2 | Early revenue | 6–24 months |
| T3 | Medium-term | 2–5 years |
| T4 | Long-term | 5–10 years |
| T5 | Strategic lifetime | 10+ years |

*Track both **time to first revenue** and **time to meaningful scale** separately.*

---

## Part C — The 22 scoring dimensions (each 1–10)

Score each. Where higher = better unless marked **(inverse: higher = worse)**.

**Demand & market**
1. Market size (TAM)
2. Problem severity
3. Customer urgency
4. Willingness to pay

**Difficulty & risk (inverse)**
5. Technical complexity *(inverse)*
6. Regulatory complexity *(inverse)*
7. Capital intensity *(inverse)*
8. Ease of customer acquisition *(higher = easier = better)*

**Model leverage (applicability)**
9. AI leverage
10. SaaS potential
11. Hardware/device potential
12. Infrastructure potential
13. Services potential
14. Marketplace potential
15. Export potential

**Durability & fit**
16. Defensibility (moat)
17. Founder suitability (non-scientist tech/business founder) — from `04`
18. Time to first revenue *(score: T1=10, T2=8, T3=5, T4=3, T5=1)*
19. Time to meaningful scale *(same mapping logic)*
20. Scalability
21. Strategic exit potential
22. Long-term compounding potential

> **Applicability dimensions (9–15) are descriptive**, not all-must-be-high. A great IoT play may score 9 on hardware and 3 on marketplace — that's fine. They feed *type classification*, not just the average.

---

## Part D — Composite scores & formulas

Let each dimension be \(d_i\). For **inverse** dimensions (5,6,7), convert to a "favorability" value \(f = 11 - \text{raw}\) before averaging (so low complexity scores high).

### Attractiveness Score (0–100)
Weighted blend emphasizing demand, defensibility, founder-fit, and compounding:

\[
\text{Attractiveness} = 100 \times \frac{\sum w_i \cdot v_i}{10 \cdot \sum w_i}
\]

Recommended weights \(w_i\):

| Dimension | Weight |
|-----------|--------|
| Market size | 3 |
| Problem severity | 3 |
| Customer urgency | 2 |
| Willingness to pay | 3 |
| Ease of customer acquisition | 2 |
| Defensibility | 3 |
| Founder suitability | 3 |
| Time to first revenue | 2 |
| Time to meaningful scale | 1 |
| Scalability | 2 |
| Long-term compounding | 3 |
| Strategic exit | 1 |
| Best applicable model leverage (max of 9–15) | 2 |
| Capital favorability (11 − capital intensity) | 2 |
| Regulatory favorability (11 − reg complexity) | 1 |
| Technical favorability (11 − tech complexity) | 1 |

*(Use the **max** of the applicability dimensions 9–15 as a single "best-fit leverage" input, so non-SaaS models aren't penalized for being only one type.)*

### Risk Score (0–100, higher = riskier)
\[
\text{Risk} = 100 \times \frac{\sum r_j \cdot g_j}{10 \cdot \sum r_j}
\]
where \(g_j\) are the raw values of risk drivers: technical complexity, regulatory complexity, capital intensity, time-to-scale (inverse: long = risky → use \(11 - \text{score}\)), competitive intensity (raw 1–10, higher=worse), moat-absence (\(11 - \text{defensibility}\)), adoption difficulty (\(11 - \text{ease of acquisition}\)). Suggested equal weights \(r_j = 1\).

---

## Part E — Priority & type decision rules

**Recommended Priority:**

| Attractiveness | Risk | Priority |
|----------------|------|----------|
| ≥ 70 | ≤ 55 | **High** |
| ≥ 70 | > 55 | **Medium** (high upside, manage risk) |
| 55–69 | ≤ 60 | **Medium** |
| 40–54 | any | **Low** |
| < 40 | any | **Avoid** |
| Any | Founder-fit ≤ 4 (vetoed in `04`) | downgrade ≥ one level |

**Opportunity Type** (from `02` Part E; pick the dominant):
- **Fast revenue** — T1/T2 + C1/C2 + repeatable motion.
- **Long-term strategic** — T3+ but high compounding/market.
- **Platform potential** — clear services→data→SaaS/AI/network climb.
- **Avoid** — fails the worth-solving gate or vetoed.

---

## Part F — Standard scorecard template (copy per opportunity)

```
### Opportunity: <name>
One-liner: <what it is, for whom>

Business model (03): Primary=<>, Secondary=<>, Pattern=<services→data→SaaS / razor-blade / etc.>
Opportunity type (02E): <Fast revenue / Long-term strategic / Platform / Hardware-enabled / Fintech / Marketplace / Avoid>

Problem · Customer · User · Buyer · Budget owner · Who can block:
Existing solutions & why inadequate:

Capital band (05A): C? | Phased sub-₹5cr entry: <yes/route/no>
Timeline (05B): First revenue T? | Meaningful scale T?

Scores (1–10):
 Market size __  Problem severity __  Urgency __  WTP __
 Tech complexity(inv) __  Reg complexity(inv) __  Capital intensity(inv) __  Ease of acq __
 AI __  SaaS __  Hardware __  Infra __  Services __  Marketplace __  Export __
 Defensibility __  Founder fit __  TTF-revenue __  TT-scale __  Scalability __  Exit __  Compounding __
 Competitive intensity (higher=worse) __

Attractiveness: __/100   Risk: __/100   Priority: High/Med/Low/Avoid

Required hires/partners: 
GTM (1 line): 
Why it could fail: 
Founder-fit verdict (04G): 
Portfolio row updated: yes/no
```

---

## Part G — Scoring hygiene

- **Calibrate, don't inflate.** Reserve 9–10 for genuinely exceptional; most dimensions cluster 4–7.
- **Cite or assume.** Any TAM/market score must reference a source or be tagged `[ASSUMPTION]`.
- **Re-score over time.** Scores are living; update as evidence arrives (mandate timing, competitor funding, pilot results).
- **Compare within type.** Rank fast-revenue ideas against each other and platform ideas against each other, then blend — so we don't drown long-term gems under quick wins.
