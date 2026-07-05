# Welltech Build Roadmap — Prioritised Phases, Make-vs-Buy, and the $500K Plan

**Abstract.** This is the execution roadmap for standing Welltech up in Malaysia on the **US$500,000 secured tranche**, weighted toward marketing and build. It frames what this money's real job is (reach a Series-A-unlocking proof point, not build the whole company), sets the make-vs-buy position for every component (make the moat, subscribe to the commodity — LLMs, WhatsApp/BSP, EMR, payments), sequences the work into prioritised phases with stage-gates, and lays out an illustrative spend plan with the one financial-discipline rule that matters most: **do not pour marketing until the funnel and retention are proven.** All figures are illustrative planning numbers, not forecasts — see [financial-model.md](financial-model.md) and [../90-verification/methodology.md](../90-verification/methodology.md).

Last updated: July 2026. Builds on: [implementation-roadmap.md](implementation-roadmap.md) · [automation.md §4 Make vs Buy](../60-ai-operating-model/automation.md) · [ai-clinic.md](../60-ai-operating-model/ai-clinic.md) · [malaysia-go-to-market.md](malaysia-go-to-market.md) · [pricing-strategy.md](pricing-strategy.md).

---

## 1. What the $500K is actually for

US$500K (≈ RM2.35M) does **not** fund the three-market company — the full trajectory needs ~US$5M of peak funding ([financial-model.md](financial-model.md)). This tranche has one job:

> **Prove the Malaysia weight-loss wedge to a point that de-risks the Series A** — a working WhatsApp-native clinic, a proven and repeatable acquisition funnel with a known CAC, a first patient cohort, and the beginnings of the one asset no competitor has: **published local retention/outcome data.**

Everything below is prioritised against that single outcome. If a task doesn't move toward the proof point, it waits for the Series A.

**The proof point (what "done" looks like for this tranche):**

| Metric | Target to unlock Series A |
|---|---|
| Enrolled patients | ~300–600 (Malaysia, weight wedge) |
| Proven CAC | A stable, documented cost per enrolled patient (target ≈ RM650, validated by real spend) |
| Funnel | Repeatable click-to-WhatsApp → consult → enrolment conversion, instrumented end-to-end |
| Retention signal | Week-8 persistence measured on ≥200 patients, beating the unmanaged baseline |
| Outcome data | First cohort's weight/metabolic outcomes captured in a publishable structure |
| Unit economics | Positive contribution margin per patient demonstrated at small scale |
| Compliance | Clinic registered, e-prescription pathway working, PDPA + advertising compliance clean |

---

## 2. Guiding principles

1. **Make the moat, subscribe to the commodity.** Build only what is proprietary and Malaysia-shaped (the orchestration layer, the longitudinal patient-memory store, the care protocols, the metric definitions). Rent everything undifferentiated (LLMs, WhatsApp connectivity, EMR, payments, couriers). This is the settled position in [automation.md §4](../60-ai-operating-model/automation.md) and it is doubly right on a small budget.
2. **Compliance spine before patient #1.** Consent capture, record archiving, and the audit log cannot be retrofitted. They ship first, cheaply.
3. **Do not front-load marketing.** The $500K's biggest risk is spending the marketing budget before the funnel and retention are proven. Marketing is *phased*: a small test budget to find real CAC and prove conversion, then scale only after unit economics and week-8 persistence clear their gates. Acquiring 1,500 patients before the ops are proven would burn the tranche and the reputation at once.
4. **Buy speed now, buy economics later.** Start on a fast, managed WhatsApp BSP (respond.io); migrate to direct Cloud API / 360dialog only when message volume makes the economics worth it.
5. **Clinicians and drugs are mostly variable cost.** Sessional doctors and drug supply are largely covered by patient revenue (the RM999 programme is margin-positive by design). Keep *fixed* team lean; let delivery scale with revenue.
6. **Every phase has a kill/scale gate.** Money moves to the next phase only when the current phase's gate is met — otherwise fix, don't scale.

---

## 3. Make vs Buy — master table

Aligned to [automation.md §4](../60-ai-operating-model/automation.md), with cost posture for this tranche.

| Component | Position | Why | Cost posture on $500K |
|---|---|---|---|
| **Orchestration layer** (state machine, escalation router, human-in-the-loop gates) | 🔨 **MAKE** | This *is* the company; embeds the escalation matrix and regulatory gates; no vendor sells it Malaysia-shaped | Core engineering spend |
| **Longitudinal patient-memory / context store** | 🔨 **MAKE** | The data moat; proprietary schema | Core engineering spend |
| **Care protocols & clinical content** (titration flows, red-flag rules, message library) | 🔨 **MAKE** (clinician-authored) | Bespoke, safety-critical, differentiating | Medical-director time |
| **WhatsApp conversation logic / AI agent behaviour** | 🔨 **MAKE** (on top of bought LLM + BSP) | The care experience is the moat | Core engineering spend |
| **Metric definitions & the retention/outcome dataset** | 🔨 **MAKE** | Definitions are the IP; the dataset is the Series-A asset | Analyst/founder time |
| **Guardrails / evals** (tripwires, red-team suite, golden sets) | 🔨 **MAKE** core + 🛒 buy eval tooling | Safety cases are bespoke | Small |
| **LLM models** | 🛒 **BUY** — API, multi-model routing (Claude / GPT / a cheaper model for routing) | Frontier quality is unmatchable in-house; an abstraction layer prevents lock-in | Low at pilot volume (usage-based) |
| **WhatsApp / BSP connectivity** | 🛒 **BUY** — respond.io (Phase 0–1) → 360dialog / direct Cloud API (Phase 2) | Speed now, economics later | Subscription + per-message |
| **Ambient scribe** (doctor note generation) | 🛒 **BUY** + own the sign-off UX | Mature vendor category; revisit for Manglish | Deferred to Phase 2 |
| **EMR / clinic-management system** | 🛒 **BUY** (API-first; must have API access, audit log, e-invoice) | Undifferentiated heavy lifting | Subscription |
| **E-prescription rails** | 🛒 **BUY / PARTNER** (DOC2US or Teleme-style compliant e-Rx; or minimal in-clinic dispensing first) | Regulated; a proven compliant pattern exists — don't rebuild the CA-signature stack | Partner fee / integration |
| **Payments & BNPL** | 🛒 **BUY** (HitPay / Curlec / Stripe + Atome for instalments) | Regulated commodity | Transaction fees |
| **Pharmacy fulfilment & cold-chain** | 🛒 **PARTNER** (Alpro or equivalent) + 🔨 make the tracking/notification layer | Asset-light; the *communication* layer is the differentiator, not the logistics | Partner margin share |
| **Labs / diagnostics** | 🛒 **PARTNER** (BP Healthcare / Pathlab / Innoquest) | Commodity network; negotiate B2B rates | Per-test COGS |
| **Human care console** | 🛒 BSP inbox (Phase 1) → 🔨 **MAKE** (Phase 2) | Escalation packets need memory + EMR context vendors can't join | Phase 2 build |
| **Analytics warehouse & BI** | 🛒 **BUY** warehouse/BI + 🔨 make the metric definitions | Standard stack; definitions are the IP | Low |
| **Cloud hosting / infra** | 🛒 **BUY** (one cloud, keep it boring) | Commodity | Usage-based |

**The rule of thumb:** if it touches the *patient relationship, the clinical logic, or the data model*, make it. If it's plumbing, rent it.

---

## 4. The phased roadmap

Three phases fit inside the $500K; Phase 3 is explicitly post-raise.

### Phase 0 — Foundations (Weeks 0–8) · "legal, built, and connected"

**Objective:** a compliant, working MVP and the partnerships/licences in place to legally see and treat the first patient. Near-zero marketing.

**MAKE:** the MVP orchestration layer + patient-memory store; the WhatsApp intake→consult→enrolment flow (v1); the compliance spine (consent ledger, record archiving, audit log); the core care protocols (clinician-authored) for the weight wedge.
**BUY / SET UP:** LLM API access + routing; respond.io BSP + a verified WhatsApp Business number; EMR (API-first); payments (HitPay/Curlec + Atome); cloud infra.
**PARTNER / LOCK:** the anchor physical clinic + medical director (the entity that anchors prescriptions); fulfilment (Alpro or equivalent) with cold-chain; e-prescription pathway; a lab for baseline bloods; a bariatric referrer for escalation.
**REGULATORY (start day 1 — 4–6 week lead times):** clinic registration; KKLIU/MAB advertising-creative approval pipeline; PDPA setup (DPO, TIA for cross-border data); GLP-1 prescribing protocol signed by the medical director.

**Milestones:** entity + clinic registered · medical director + first sessional doctors contracted · WhatsApp number live and template-approved · one end-to-end test patient run through intake→consult→e-Rx→fulfilment→first check-in · legal + clinical sign-off obtained.

**Gate to Phase 1:** a real patient can be acquired, consulted, prescribed to, fulfilled, and monitored — legally and end-to-end.

### Phase 1 — Launch & Prove (Months 2–6) · "find the CAC, prove the funnel, see the retention"

**Objective:** soft-launch to a controlled cohort; establish the *real* cost per enrolled patient and the funnel conversion; stand up the retention engine and get the first week-8 persistence signal. **Marketing is a test budget, not a scale budget.**

**MAKE:** retention engine v1 (the weeks-2–8 proactive check-in cadence — the highest-ROI clinical activity in the company); the escalation matrix in operation (AI→nurse→doctor); outcome/metric capture from day one.
**BUY:** scale LLM/BSP usage with volume; add churn-signal instrumentation.
**GROW:** run a *small* click-to-WhatsApp + SEO/content test (see [funnels.md](../50-marketing-intelligence/funnels.md), [seo.md](../50-marketing-intelligence/seo.md), [paid-search.md](../50-marketing-intelligence/paid-search.md)) to a few hundred leads — enough to measure CAC and conversion honestly, not to fill the clinic. Doctor-KOL content as the compliant reach engine.

**Milestones:** first ~100–200 enrolled patients · CAC measured on real spend · funnel conversion instrumented end-to-end · week-8 persistence measured · first patient reviews (the trust flywheel) · no compliance incidents.

**Gate to Phase 2 (scale gate — do not skip):** week-8 persistence ≥ target on ≥200 patients · funnel conversion stable and repeatable · CAC within striking distance of RM650 with a path down · contribution margin per patient positive · WhatsApp number quality-rating "High" sustained. **If the gate fails, fix the funnel/retention — do not pour marketing.**

### Phase 2 — Scale in Malaysia (Months 6–12) · "pour marketing, defend month 2, publish the cohort"

**Objective:** now that the economics are proven, scale acquisition; deepen the retention engine at the month-2 churn cliff; capture the first publishable cohort — the asset that unlocks the Series A.

**MAKE:** the human care console (replace the BSP inbox); churn-scoring + save-call workflows; the month-2 retention interventions; the outcome dataset in publishable form.
**BUY:** add the ambient scribe (remove the doctor's keyboard as volume grows); direct Cloud API / 360dialog migration if message volume justifies the economics.
**GROW:** scale the proven channels; add corporate/employer pilots as a secondary channel; broaden SEO content to own the Bahasa + Chinese GLP-1 search that paid ads can't touch.

**Milestones:** ~300–600+ enrolled patients · month-6 persistence beating the unmanaged baseline by a clear margin · first cohort outcomes written up · a second care line (longevity/metabolic) piloted · a repeatable, documented growth playbook.

**Gate to Series A:** a published/publishable Malaysian cohort · proven LTV:CAC · a documented, repeatable acquisition + retention machine · a credible Singapore-entry plan. **This is what you raise the ~US$5M against.**

### Phase 3 — Beyond this tranche (post-raise) · "platform, then Singapore"

Explicitly **not funded by the $500K.** After the Series A: Singapore entry (the HCSA-licensed credibility market), the deeper AI moat (Manglish-tuned models, and — only as a deliberate registration project — SaMD-classed titration decision support), the longevity line at scale, and eventually Hong Kong. Sequencing and rationale: [implementation-roadmap.md](implementation-roadmap.md), [expansion-strategy.md](expansion-strategy.md).

---

## 5. The $500K spend plan (illustrative)

Weighted to marketing and build per your steer — but with marketing *phased* behind the Phase-1 gate. Figures illustrative; tune to actual quotes.

| Bucket | Allocation | ~US$ | What it covers |
|---|---|---|---|
| **Marketing & growth** | ~40% | **~$200K** | Phased: ~$30–50K Phase-1 *test* budget to find CAC; the balance released into Phase 2 *only after the gate*. Content/SEO, click-to-WhatsApp, doctor-KOL, creative + KKLIU approvals. |
| **Product & engineering (MAKE)** | ~27% | **~$135K** | Lean build team (founder-led + 1–2 engineers or a trusted dev partner) for the orchestration layer, memory store, WhatsApp agent, care console, retention engine. |
| **Clinical, regulatory & legal** | ~15% | **~$75K** | Fractional medical director; clinic registration + licensing; legal sign-off (virtual-clinic structure, e-Rx, advertising); PDPA/DPO; clinical protocol authoring. Sessional doctor fees + drug COGS run largely against revenue, not this bucket. |
| **Tooling & subscriptions (BUY)** | ~8% | **~$40K** | LLM API usage, respond.io/BSP + WhatsApp messaging, EMR, payments fees, cloud, analytics/BI, eval tooling — usage-based and cheap at pilot volume. |
| **G&A + contingency** | ~10% | **~$50K** | Entity, accounting, insurance, buffer. |

**Runway logic:** with marketing gated, *fixed* monthly burn (team + tooling + fractional clinical + G&A) is kept lean enough to run ~12 months to the Series-A proof point, with the larger marketing spend deployed only in the back half once it's earning its keep. The discipline rule protects the tranche: **the marketing scale-up is a reward for a passed gate, not a launch expense.**

> Reallocation note: if the Phase-1 gate is hit *early* and cheaply, shift the underspent build/contingency into marketing to accelerate the cohort. If the gate is *missed*, the unspent marketing is your runway to fix the funnel — which is exactly why it isn't committed up front.

---

## 6. Lean team for the tranche

Keep fixed headcount minimal; scale delivery with revenue.

| Role | Type | Phase |
|---|---|---|
| Founder(s) — product, growth, partnerships | Full-time | 0 |
| Engineer(s) ×1–2 (or a trusted dev partner) | Full-time / contract | 0 |
| Medical Director | Fractional → part-time | 0 |
| Doctors | Sessional (paid per consult — variable) | 1 |
| Nurse / care coordinator ×1 | Hire when volume needs it | 1→2 |
| Growth / marketing lead | Full-time or fractional | 1 |
| Legal, accounting, DPO | Outsourced / fractional | 0 |

---

## 7. Stage gates & kill criteria (one screen)

| Transition | Scale if… | Otherwise |
|---|---|---|
| Phase 0 → 1 | A patient can be legally acquired→consulted→prescribed→fulfilled→monitored end-to-end | Don't launch; finish compliance + integration |
| Phase 1 → 2 | Week-8 persistence ≥ target on ≥200 patients; funnel repeatable; CAC on track; contribution positive; number quality "High" | **Fix funnel/retention — do not scale marketing** |
| Phase 2 → Series A | Publishable Malaysian cohort; proven LTV:CAC; documented growth+retention machine; credible SG plan | Extend runway on core; raise later on stronger data |

---

## 8. What must be true (the honest risks)

- **Retention is the whole thesis.** The financial model shows it is the #1 sensitivity, and the [verification pass](../90-verification/README.md) flags that the unmanaged baseline may be drifting — so Phase 1's real job is to *measure* retention honestly and prove Welltech beats the baseline. Everything downstream depends on it.
- **Compliance is a moat only if it's real.** The legal/clinical sign-off items in [regulatory-verification.md](../90-verification/regulatory-verification.md) must be closed in Phase 0 — virtual-clinic structure, e-prescription validity, GLP-1 advertising boundaries, titration protocol.
- **Drug supply economics.** Confirm distributor terms early (the model flags this as unvalidated) — it sets your real margin.
- **Don't out-run the ops.** The failure mode is scaling acquisition before the care engine and the compliance spine can hold the volume — which is exactly what the phased marketing and the gates are designed to prevent.
