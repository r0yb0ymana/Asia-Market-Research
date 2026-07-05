# Welltech Build Roadmap — Prioritised Phases, Make-vs-Buy, and the $500K Plan

> **Canonical build version now lives in the Mesura build repo: `github.com/r0yb0ymana/mesura`** (Mesura-named, standalone, cross-links fixed — the single source of truth going forward). This copy is retained for research context.

**Abstract.** This is the execution roadmap for launching **NewCo** — a subsidiary of WellTech Health — on the **US$500,000 WellTech-funded tranche**, weighted toward marketing and build. NewCo runs a WhatsApp-native, AI-operated medical weight-loss / longevity programme, piloting through WellTech's existing **Medimind KL** clinic (doctors + pharmacy) and integrating with WellTech's existing **clinic operations software** as the clinical system of record. This document frames what the money's real job is (reach a Series-A-unlocking proof point), sets the corporate/commercial structure, sets the make-vs-buy position for every component (make the moat; subscribe to the commodity; **reuse what WellTech already owns**), sequences the work into prioritised phases with stage-gates, and lays out an illustrative spend plan with the one financial-discipline rule that matters most: **do not pour marketing until the funnel and retention are proven.** All figures are illustrative planning numbers, not forecasts — see [financial-model.md](financial-model.md) and [../90-verification/methodology.md](../90-verification/methodology.md).

Last updated: July 2026. Builds on: [implementation-roadmap.md](implementation-roadmap.md) · [automation.md §4 Make vs Buy](../60-ai-operating-model/automation.md) · [ai-clinic.md](../60-ai-operating-model/ai-clinic.md) · [malaysia-go-to-market.md](malaysia-go-to-market.md) · [pricing-strategy.md](pricing-strategy.md).

---

## 1. What the $500K is actually for

The **US$500K is WellTech parent funding** (intra-group), not an external round. It does **not** fund the three-market company — the full trajectory needs ~US$5M of peak funding ([financial-model.md](financial-model.md)). This tranche has one job:

> **Prove the Malaysia weight-loss wedge — piloted at Medimind KL — to a point that de-risks the Series A:** a working WhatsApp-native service, a proven and repeatable acquisition funnel with a known CAC, a first patient cohort, and the beginnings of the one asset no competitor has — **published local retention/outcome data**, owned by NewCo.

**The money stretches further than a greenfield build**, because WellTech already provides the clinic, the doctors, the pharmacy/dispensing, the clinic operations software, *and* the engineers who built it. So NewCo is **not** paying to register a clinic, recruit doctors, buy an EMR, or stand up external fulfilment — freeing more of the tranche for **marketing and the new-service build**.

Everything below is prioritised against the proof point. If a task doesn't move toward it, it waits for the Series A.

**The proof point (what "done" looks like for this tranche):**

| Metric | Target to unlock Series A |
|---|---|
| Enrolled patients | ~300–600 (Malaysia, weight wedge; longevity as fast-follow) |
| Proven CAC | A stable, documented cost per enrolled patient (target ≈ RM650, validated by real spend) |
| Funnel | Repeatable click-to-WhatsApp → consult → enrolment conversion, instrumented end-to-end |
| Retention signal | Week-8 persistence measured on ≥200 patients, beating the unmanaged baseline |
| Outcome data | First cohort's weight/metabolic outcomes captured in a NewCo-owned, publishable structure |
| Unit economics | Positive contribution margin per patient demonstrated at small scale |
| Compliance | e-prescription/dispensing working via Medimind, PDPA + advertising + fee-structure compliance clean |

---

## 2. Corporate & commercial structure

The pilot deliberately uses the lowest-barrier path — WellTech's existing assets — while keeping the **fundable assets inside NewCo** so it can raise externally or spin out later (**Option A**). *(NewCo's working name is **Mesura** / brand **Mesura Health**, tagline "Metabolic health, measured" — provisional, pending trademark/SSM clearance; see [naming-decision.md](naming-decision.md). "NewCo" is used generically here until the name is cleared.)*

| Party | Role |
|---|---|
| **NewCo** (subsidiary of WellTech) | Owns the **brand, patient relationship, recurring programme revenue, the retention/outcome dataset (the moat), and the care-orchestration IP.** Builds and runs the WhatsApp-native service; collects the patient fee; owns the data. |
| **WellTech Health** (parent) | **Shareholder + funder** of this tranche; **arm's-length service provider** (via Medimind) and **software licensor** (clinic OS). Compensated at fair market value. |
| **Medimind KL** (WellTech clinic) | Provides the **regulated clinical act** — its doctors run the telehealth consults, prescribe, and **dispense from its own pharmacy**; the **doctor keeps the full consult fee (100%)**. Medimind **adds GLP-1 to its pharmacy formulary** and dispenses it. |

**Commercial mechanic (drug economics).** Medimind does not currently stock GLP-1s, so **Medimind adds GLP-1 to its pharmacy formulary** — procuring via its existing distributor accounts (Zuellig/DKSH/Pharmaniaga) and dispensing in-house under its own licence (a new SKU, not a new capability). The programme is priced **all-in (RM999/month, drug included)** and **NewCo collects the full patient payment**. The **doctor keeps the full consult fee (100%)** — the cleanest fee-for-service structure (NewCo takes no cut of the clinical fee, keeping it clear of MMC fee-splitting). Medimind bills NewCo **drug-at-cost + a dispensing fee**; **NewCo's revenue is the programme/care fee + a modest drug margin marked into the RM999** (not pure pass-through — with the doctor keeping the full consult fee and the drug at cost, pure pass-through would squeeze NewCo's contribution). NewCo holds **no** pharmacy or wholesale licence (it rides Medimind's pharmacy). **NewCo-as-drug-wholesaler is deferred to Phase 2** (a direct-sourcing margin lever that requires a Type A wholesale poisons licence + pharmacist + GDP cold-chain, and only pays off at multi-clinic volume). **The one live economic action is to obtain Medimind's GLP-1 distributor cost** — the #1 unvalidated input, now an internal check.

**Compliance guardrails to bake into the founding/service agreements** (with counsel):
- **Fair-market fee-for-service to Medimind** — documented as payment for services (doctor time + drug + dispensing), **not** a referral kickback or a split of the consultation fee (MMC prohibits fee-splitting).
- **NewCo does not practise medicine.** The medical act — consult, diagnosis, prescription — stays with **Medimind's licensed doctor**, who retains independent clinical judgment (including the freedom to decline to prescribe).
- **IP and patient-data ownership assigned to NewCo**, even though WellTech's engineers build the service and WellTech owns the clinic OS (license the clinic OS to NewCo; assign the new-service IP to NewCo).
- **PDPA consent covers the dual-entity flow** (patient consents to NewCo owning their data *and* to sharing between NewCo and Medimind for care).
- **Advertising:** market the programme and outcomes; **never name the molecule**; KKLIU/MAB approval on every creative.

---

## 3. Make vs Buy — master table

Aligned to [automation.md §4](../60-ai-operating-model/automation.md), updated for the WellTech-asset reality. **New third category: REUSE — what WellTech already owns.**

| Component | Position | Why | Cost posture |
|---|---|---|---|
| **Orchestration layer** (state machine, escalation router, human-in-the-loop gates) | 🔨 **MAKE** | This *is* NewCo; embeds the escalation matrix and regulatory gates; no vendor sells it Malaysia-shaped | Core engineering (WellTech team) |
| **Longitudinal patient-memory / context store** | 🔨 **MAKE** | The data moat; proprietary schema; NewCo-owned | Core engineering |
| **Care protocols & clinical content** (titration flows, red-flag rules, message library) | 🔨 **MAKE** (Medimind doctor-authored) | Bespoke, safety-critical, differentiating | Medimind doctor time |
| **WhatsApp conversation logic / AI agent behaviour** | 🔨 **MAKE** (on top of bought LLM + BSP) | The care experience is the moat | Core engineering |
| **Clinic-OS ↔ NewCo integration / data + consent bridge** | 🔨 **MAKE** | Automated capture of consult/prescription/dispensing/results into NewCo's store so the cohort dataset builds itself; same engineers own both codebases | Core engineering |
| **Metric definitions & the retention/outcome dataset** | 🔨 **MAKE** | Definitions are the IP; the dataset is the Series-A asset | Analyst/founder time |
| **Guardrails / evals** (tripwires, red-team suite, golden sets) | 🔨 **MAKE** core + 🛒 buy eval tooling | Safety cases are bespoke | Small |
| **EMR / clinic-management system** | ♻️ **REUSE** (WellTech clinic OS, licensed to NewCo) | Already built and mature — EMR, pharmacy/inventory, billing/payments, appointments all exist; NewCo integrates, does not buy or build | Licence fee to parent |
| **Doctor consult + prescribing + dispensing** | ♻️ **REUSE** (Medimind, fee-for-service) | Regulated clinical act; Medimind is licensed and staffed | Fair-market service fee |
| **Pharmacy fulfilment & cold-chain (pilot)** | ♻️ **REUSE** (Medimind pharmacy, in-house GP dispensing) + 🔨 make the tracking/notification layer | No external fulfilment or signed e-Rx needed in-house; the *communication* layer is the differentiator | Dispensing fee |
| **LLM models** | 🛒 **BUY** — API, multi-model routing (Claude / GPT / a cheaper router model) | Frontier quality unmatchable in-house; abstraction layer prevents lock-in | Low at pilot volume (usage-based) |
| **WhatsApp / BSP connectivity** | 🛒 **BUY** — respond.io (Phase 0–1) → 360dialog / direct Cloud API (Phase 2) | Speed now, economics later | Subscription + per-message |
| **Payments & BNPL** | 🛒 **BUY** — reuse the clinic OS's FIUU gateway where possible; add Atome for instalments | Regulated commodity; partly already integrated in the clinic OS | Transaction fees |
| **Ambient scribe** (doctor note generation) | 🛒 **BUY** + own the sign-off UX | Mature vendor category; revisit for Manglish | Deferred to Phase 2 |
| **Labs / diagnostics** | ♻️/🛒 **REUSE Medimind's lab arrangements** (clinic OS has lab requests); add BP Healthcare/Pathlab at scale | Commodity; Medimind already orders labs | Per-test COGS |
| **Human care console** | 🛒 BSP inbox (Phase 1) → 🔨 **MAKE** (Phase 2) | Escalation packets need memory + clinic-OS context | Phase 2 build |
| **Analytics warehouse & BI** | 🛒 **BUY** warehouse/BI + 🔨 make the metric definitions | Standard stack; definitions are the IP | Low |
| **Cloud hosting / infra** | 🛒 **BUY** (one cloud, keep it boring) | Commodity | Usage-based |
| **External fulfilment (Alpro) + signed/external e-Rx + NewCo drug wholesale** | ⏭ **PHASE 2** | Scale levers, not pilot needs — external pharmacy triggers the signed-script requirement; wholesale triggers the Type A licence | Deferred |

**The rule of thumb:** if it touches the *patient relationship, the clinical logic, or the data model* → **MAKE** (and keep it in NewCo). If WellTech already owns it → **REUSE** (licensed at fair value). If it's plumbing → **BUY**.

---

## 4. The phased roadmap

Three phases fit inside the $500K; Phase 3 is explicitly post-raise.

### Phase 0 — Foundations (Weeks 0–8) · "structured, built, and connected"

**Objective:** a compliant, working service and the agreements/integration in place to legally acquire, refer, treat (via Medimind), and monitor the first patient — end to end. Near-zero marketing. *(No clinic to register, no doctors to recruit, no EMR to buy — Medimind and the clinic OS already exist.)*

**MAKE:** the MVP orchestration layer + NewCo patient-memory store; the WhatsApp intake → eligibility → payment → **booking-handoff-to-Medimind** flow (v1); the **clinic-OS ↔ NewCo integration + data/consent bridge**; the compliance spine (consent ledger, record archiving, audit log); the core care protocols (Medimind-doctor-authored) for the weight wedge.
**REUSE / SET UP:** license the WellTech **clinic OS** to NewCo and wire the integration; confirm the **Medimind accountable doctor** (Medical Director) and the two telehealth doctors; use Medimind's pharmacy for dispensing and its lab arrangements for baseline bloods.
**BUY / SET UP:** LLM API access + routing; respond.io BSP + a verified WhatsApp Business number; payments (reuse FIUU + add Atome); cloud infra.
**LEGAL / COMMERCIAL (start day 1 — lead times):** the **WellTech ↔ NewCo ↔ Medimind service agreement** (fair-market fee-for-service, IP + patient-data assigned to NewCo, clinic-OS licence); **KKLIU/MAB advertising-creative approval pipeline** (~4–6 weeks); **PDPA setup** (DPO, dual-entity consent, TIA for cross-border data); **fee-splitting / practice-of-medicine structuring** confirmed by counsel; GLP-1 (and longevity) prescribing protocol signed by the Medimind Medical Director.

**Milestones:** NewCo incorporated (subsidiary) · service agreement signed with IP + data assigned to NewCo · clinic OS integrated and pushing consult/prescription/dispensing/results into NewCo's store · WhatsApp number live and template-approved · one end-to-end test patient run (acquire → refer → Medimind consult/prescribe/dispense → NewCo monitoring) · legal + clinical sign-off obtained.

**Gate to Phase 1:** a real patient can be acquired on WhatsApp, referred to a Medimind doctor, consulted/prescribed/dispensed in the clinic OS, and monitored by NewCo — legally and end-to-end, with consent + data flowing to NewCo.

### Phase 1 — Launch & Prove (Months 2–6) · "find the CAC, prove the funnel, see the retention"

**Objective:** soft-launch to a controlled cohort; establish the *real* cost per enrolled patient and the funnel conversion; stand up the retention engine and get the first week-8 persistence signal. **Marketing is a test budget, not a scale budget.**

**MAKE:** retention engine v1 (the weeks-2–8 proactive check-in cadence — the highest-ROI clinical activity in the company); the escalation matrix in operation (AI → care coordinator → Medimind doctor); outcome/metric capture from day one.
**BUY:** scale LLM/BSP usage with volume; add churn-signal instrumentation.
**GROW:** run a *small* click-to-WhatsApp + SEO/content test (see [funnels.md](../50-marketing-intelligence/funnels.md), [seo.md](../50-marketing-intelligence/seo.md), [paid-search.md](../50-marketing-intelligence/paid-search.md)) to a few hundred leads — enough to measure CAC and conversion honestly, not to fill the clinic. Doctor-KOL content as the compliant reach engine.

**Milestones:** first ~100–200 enrolled patients · CAC measured on real spend · funnel conversion instrumented end-to-end · week-8 persistence measured · first patient reviews (the trust flywheel) · no compliance incidents.

**Gate to Phase 2 (scale gate — do not skip):** week-8 persistence ≥ target on ≥200 patients · funnel conversion stable and repeatable · CAC within striking distance of RM650 with a path down · contribution margin per patient positive · WhatsApp number quality-rating "High" sustained. **If the gate fails, fix the funnel/retention — do not pour marketing.**

### Phase 2 — Scale in Malaysia (Months 6–12) · "pour marketing, defend month 2, publish the cohort"

**Objective:** now that the economics are proven, scale acquisition; deepen the retention engine at the month-2 churn cliff; capture the first publishable cohort — the asset that unlocks the Series A. **This is where the deferred scale levers come online.**

**MAKE:** the human care console (replace the BSP inbox); churn-scoring + save-call workflows; the month-2 retention interventions; the NewCo-owned outcome dataset in publishable form.
**BUY / BUILD OUT (the deferred levers):** **external fulfilment (Alpro or equivalent)** to serve demand beyond Medimind's counter — which triggers **signed / external e-prescription** (DOC2US / Teleme-style compliant rail, closing the clinic OS's signed-script gap); add the ambient scribe; evaluate **NewCo-as-drug-wholesaler** (direct sourcing at better COGS across Medimind KL + Johor + Ipoh — needs the Type A poisons licence); direct Cloud API / 360dialog migration if volume justifies it.
**GROW:** scale the proven channels; add corporate/employer pilots as a secondary channel; broaden SEO content to own the Bahasa + Chinese GLP-1 search that paid ads can't touch; extend the longevity/metabolic line.

**Milestones:** ~300–600+ enrolled patients · month-6 persistence beating the unmanaged baseline by a clear margin · first cohort outcomes written up · longevity line live · external fulfilment + signed e-Rx operational · a repeatable, documented growth playbook.

**Gate to Series A:** a published/publishable Malaysian cohort · proven LTV:CAC · a documented, repeatable acquisition + retention machine · a credible Singapore-entry plan. **This is what you raise the ~US$5M against.**

### Phase 3 — Beyond this tranche (post-raise) · "platform, then Singapore"

Explicitly **not funded by the $500K.** After the Series A: extend to the other WellTech clinics (Johor, Ipoh) and external clinics; Singapore entry (the HCSA-licensed credibility market); the deeper AI moat (Manglish-tuned models, and — only as a deliberate registration project — SaMD-classed titration decision support); the longevity line at scale; and eventually Hong Kong. Sequencing and rationale: [implementation-roadmap.md](implementation-roadmap.md), [expansion-strategy.md](expansion-strategy.md).

---

## 5. The $500K spend plan (illustrative)

Weighted to marketing and build per your steer — with marketing *phased* behind the Phase-1 gate, and infrastructure buckets light because WellTech's assets (clinic, doctors, pharmacy, clinic OS, engineers) are reused. Figures illustrative; tune to actual quotes.

| Bucket | Allocation | ~US$ | What it covers |
|---|---|---|---|
| **Marketing & growth** | ~45% | **~$225K** | Phased: ~$30–50K Phase-1 *test* budget to find CAC; the balance released into Phase 2 *only after the gate*. Content/SEO, click-to-WhatsApp, doctor-KOL, creative + KKLIU approvals. |
| **Product & engineering (MAKE)** | ~25% | **~$125K** | The NewCo service build (orchestration, memory store, WhatsApp agent, clinic-OS integration, retention engine). Built by WellTech's engineers — cost may be partly a **parent contribution / recharge**, so cash draw may be lower. |
| **Clinical, regulatory & legal** | ~13% | **~$65K** | The service agreement + IP/data assignment; legal sign-off (fee-splitting, practice-of-medicine, advertising, e-Rx validity); PDPA/DPO; protocol authoring (Medimind doctor time). No clinic-registration or doctor-recruitment cost. |
| **Tooling & subscriptions (BUY)** | ~7% | **~$35K** | LLM API usage, respond.io/BSP + WhatsApp messaging, payments fees, cloud, analytics/BI, eval tooling. No EMR line (reused). |
| **G&A + contingency** | ~10% | **~$50K** | Subsidiary setup, accounting, insurance, buffer. |

**Runway logic:** with marketing gated and infra reused, *fixed* monthly burn is low enough to run ~12 months to the Series-A proof point, with the larger marketing spend deployed only in the back half once it's earning its keep. **The marketing scale-up is a reward for a passed gate, not a launch expense.**

> Reallocation note: if the Phase-1 gate is hit *early* and cheaply, shift underspent build/contingency into marketing to accelerate the cohort. If the gate is *missed*, the unspent marketing is your runway to fix the funnel — which is exactly why it isn't committed up front. The reused-asset savings (no EMR, no clinic registration, no doctor recruitment) are best redirected to marketing + the cohort.

---

## 6. Lean team for the tranche

Keep NewCo's fixed headcount minimal; reuse WellTech's people; scale delivery with revenue.

| Role | Type | Phase |
|---|---|---|
| Founder(s) — product, growth, partnerships | Full-time (NewCo) | 0 |
| Engineers | **WellTech's existing team** (built the clinic OS) — recharged to NewCo | 0 |
| Medical Director / accountable clinician | **One of Medimind's 2 doctors** | 0 |
| Telehealth doctors | **Medimind's 2 doctors** (fair-market fee-for-service — variable) | 1 |
| Care coordinator / nurse ×1 | NewCo hire when volume needs it | 1→2 |
| Growth / marketing lead | Full-time or fractional (NewCo) | 1 |
| Legal, accounting, DPO | Outsourced / fractional | 0 |

---

## 7. Stage gates & kill criteria (one screen)

| Transition | Scale if… | Otherwise |
|---|---|---|
| Phase 0 → 1 | A patient can be legally acquired → referred → consulted/prescribed/dispensed (Medimind) → monitored (NewCo) end-to-end, data flowing to NewCo | Don't launch; finish integration + agreements |
| Phase 1 → 2 | Week-8 persistence ≥ target on ≥200 patients; funnel repeatable; CAC on track; contribution positive; number quality "High" | **Fix funnel/retention — do not scale marketing** |
| Phase 2 → Series A | Publishable NewCo-owned Malaysian cohort; proven LTV:CAC; documented growth+retention machine; credible SG plan | Extend runway on core; raise later on stronger data |

---

## 8. What must be true (the honest risks)

- **Retention is the whole thesis.** The financial model shows it is the #1 sensitivity, and the [verification pass](../90-verification/README.md) flags that the unmanaged baseline may be drifting — so Phase 1's real job is to *measure* retention honestly and prove NewCo beats the baseline. Everything downstream depends on it.
- **Get the corporate structure right, or the Series A is hard.** WellTech is parent, funder, service provider, and software owner — so the **IP, patient-data, brand, and recurring revenue must be assigned to NewCo** by contract, or NewCo owns nothing to raise against. This is a founding-docs decision to close in Phase 0.
- **Fee-splitting and practice-of-medicine lines.** Structure Medimind's payment as fair-market fee-for-service (not a referral cut), and keep the medical act with the licensed doctor — both must be right in the service agreement (MMC rules).
- **Compliance is a moat only if it's real.** The legal/clinical sign-off items in [regulatory-verification.md](../90-verification/regulatory-verification.md) must be closed in Phase 0 — the service structure, GLP-1 advertising boundaries, PDPA dual-entity consent, and the signed titration protocol.
- **Drug supply economics.** Once Medimind adds GLP-1 to its formulary, **obtain its distributor cost** (the model flags this as unvalidated) — it sets your real margin and the programme-fee/drug-margin split inside the RM999, and it's now an internal check rather than an external negotiation.
- **Don't out-run the ops.** The failure mode is scaling acquisition before the care engine and the compliance spine can hold the volume — which is exactly what the phased marketing and the gates are designed to prevent.
