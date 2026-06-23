# Pharma Founder Research — India Pharmaceutical Opportunity Atlas

### 🌐 Live single-page site: **https://zuntlytechnologies.github.io/Research/**
> The entire atlas (6 frameworks + 30 sections + the opportunity portfolio) is rendered as **one beautiful, searchable single-page website** at the link above, deployed automatically via GitHub Pages. If the link 404s, see **[Publishing](#publishing-the-public-page)** below for the one-time enablement step.

A long-horizon (10–20 year) research program to develop **founder-, investor-, and operator-level** understanding of the pharmaceutical ecosystem — with deep emphasis on **India** — in order to discover and prioritize high-potential startup, technology, AI, SaaS, hardware/IoT, services, infrastructure, supply-chain, export, and fintech opportunities for a **non-scientist founder** (finance / compliance / workflow-automation / AI / SaaS background).

> **Objective:** not to learn pharma terminology, but to find where a founder with this profile can **enter, learn, partner, build, compound, and create a meaningful pharma-industry company over a lifetime.**

---

## How this repository is organized

### `frameworks/` — the reusable analysis engine (build once, apply to every section)
| File | What it is |
|------|-----------|
| [`01-research-roadmap.md`](frameworks/01-research-roadmap.md) | The full 30-section roadmap, dependency graph, per-section deliverable template, evidence rules |
| [`02-opportunity-discovery-framework.md`](frameworks/02-opportunity-discovery-framework.md) | Discovery engine, interrogation checklist, worth-solving gate, services→platform ladder, reject rules |
| [`03-business-model-classification.md`](frameworks/03-business-model-classification.md) | 18 model archetypes, classification questions, revenue architectures, hybrid stacking patterns |
| [`04-founder-fit-framework.md`](frameworks/04-founder-fit-framework.md) | Founder profile, fit rubric + vetoes, hire/partner/phase/avoid logic, master validation question bank |
| [`05-scoring-framework.md`](frameworks/05-scoring-framework.md) | Capital/timeline bands, 22 scoring dimensions, attractiveness/risk formulas, scorecard template |
| [`06-top-100-portfolio.md`](frameworks/06-top-100-portfolio.md) | Living, ranked opportunity tracker (the program's output artifact) |

### `sections/` — the 30 deep-dive studies (all complete ✅)
Each section follows the same template: how it really works → stakeholder/money/power maps → manual workflows → pain points → existing solutions & gaps → opportunity harvest (by type) → scored opportunities → weak opportunities to avoid → customer-discovery questions → key learnings.

| # | Section | # | Section |
|---|---------|---|---------|
| 01 | [Industry Foundations](sections/section-01-industry-foundations.md) | 16 | [Pharma Finance](sections/section-16-pharma-finance.md) |
| 02 | [Complete Ecosystem](sections/section-02-pharma-ecosystem.md) | 17 | [Compliance Burden](sections/section-17-compliance-burden.md) |
| 03 | [Drug Discovery & Dev](sections/section-03-drug-discovery-development.md) | 18 | [Pharmacovigilance](sections/section-18-pharmacovigilance.md) |
| 04 | [Clinical Research](sections/section-04-clinical-research.md) | 19 | [Medical Affairs](sections/section-19-medical-affairs.md) |
| 05 | [Intellectual Property](sections/section-05-intellectual-property.md) | 20 | [Serialization & Trace](sections/section-20-serialization-track-trace.md) |
| 06 | [Regulatory Affairs](sections/section-06-regulatory-affairs.md) | 21 | [Data Ecosystem](sections/section-21-pharma-data-ecosystem.md) |
| 07 | [API Industry](sections/section-07-api-industry.md) | 22 | [CDMO & CRDMO](sections/section-22-cdmo-crdmo.md) |
| 08 | [Formulations](sections/section-08-formulations.md) | 23 | [Export Intelligence](sections/section-23-export-intelligence-dossier.md) |
| 09 | [Manufacturing Ops](sections/section-09-manufacturing-operations.md) | 24 | [AI Opportunity Map](sections/section-24-pharma-ai-opportunity-map.md) |
| 10 | [Quality Systems](sections/section-10-quality-systems.md) | 25 | [Problem Database](sections/section-25-problem-database.md) |
| 11 | [Commercialization](sections/section-11-commercialization.md) | 26 | [Industry Power Map](sections/section-26-industry-power-map.md) |
| 12 | [Supply Chain](sections/section-12-supply-chain.md) | 27 | [What CEOs Want Fixed](sections/section-27-what-ceos-want-fixed.md) |
| 13 | [Export Business](sections/section-13-export-business.md) | 28 | [India Opportunity Atlas](sections/section-28-india-opportunity-atlas.md) |
| 14 | [Biologics & Future](sections/section-14-biologics-future-therapies.md) | 29 | [Megatrends 2026–2040](sections/section-29-megatrends-2026-2040.md) |
| 15 | [Software Stack](sections/section-15-pharma-software-stack.md) | 30 | [Founder Mode](sections/section-30-founder-mode-prioritization.md) |

**The bottom line (Section 30):** the recommended wedge is the **Export Regulatory Lifecycle platform** (OPP-01/02) — start as managed RA + renewal/variation tracking for mid-market exporters, accumulate a proprietary regulatory/export **data network**, then compound into tender/IP intelligence and **export finance** — a lifetime-scale compliance→data→fintech platform that fits a non-scientist finance/compliance/AI/SaaS founder.

## Publishing the public page (one-time, ~30 seconds)

> GitHub Pages must be switched on **once by a repo admin** — a security policy prevents automated agents/tokens from enabling it for you. After this single click, the public site at **https://zuntlytechnologies.github.io/Research/** works and stays live automatically.

### ✅ Easiest path — no merge, no workflow needed (recommended)
Publish directly from this branch as plain static files:
1. Open repo **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **“Deploy from a branch”.**
3. **Branch:** select `cursor/pharma-strategy-foundations-8c0d` (or `main` after merging) · **Folder:** `/ (root)` · click **Save**.
4. Wait ~1 minute, then open **https://zuntlytechnologies.github.io/Research/**.

The repo root contains [`index.html`](index.html) plus a [`.nojekyll`](.nojekyll) file, so GitHub serves the page and its Markdown content as-is — no build step required.

### ⚙️ Alternative path — GitHub Actions (auto-redeploy on every push)
1. Open repo **Settings → Pages → Build and deployment → Source: “GitHub Actions”.**
2. Re-run the **“Deploy single-page site to GitHub Pages”** workflow from the **Actions** tab (or merge this PR to `main`).
3. The workflow in [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml) deploys automatically thereafter.

> Either way the page is fully client-side (it renders the Markdown in `frameworks/` + `sections/` + this README into one page), so it also works on **any** static host (Netlify, Vercel, Cloudflare Pages, S3) by serving the repo root.

---

## Operating principles

- **Opportunity universe is broad:** software, AI, SaaS, workflow automation, compliance tech, data intelligence, hardware/IoT, cold chain, serialization, export-enablement, logistics/distribution, marketplaces, managed services, BPO/KPO, training, packaging/anti-counterfeit, equipment, testing/audit, procurement, pharma fintech, tender intelligence, and hybrids. **Not** restricted to pure SaaS.
- **Founder-fit discipline:** avoid opportunities that require the founder to personally lead drug discovery, chemistry, biologics, clinical science, or large-scale manufacturing — unless entered via platform / services / marketplace / infrastructure / data / commercialization / compliance / distribution / partnership / asset-light layers.
- **Don't auto-reject** an idea for not being SaaS, or for payback > 24 months. **Classify and score** it instead.
- **Evidence discipline:** prefer official regulators and credible industry/government sources; never invent precise data; use ranges; tag assumptions as `[ASSUMPTION]`.

## Execution cadence
1. Build the five frameworks + portfolio structure. ✅
2. Execute **Section 1: Industry Foundations.** ✅
3. **Stop and await instruction**, then proceed section-by-section (2 → 30), each building on the previous.
