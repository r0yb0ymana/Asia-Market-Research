# Automation Opportunity Map: Every Clinic Process, Scored and Sequenced

**Abstract.** This document inventories 44 operational processes of a digital-first clinic across eight domains (acquisition, onboarding, clinical, fulfilment, billing, retention, compliance, analytics) and scores each on automation potential (full / assisted / human-only), impact, complexity, and regulatory constraint under Malaysian law. It then sequences the build into three phases (launch, scale, advanced), sets make-vs-buy positions per component, models the cost of AI-leveraged operations against traditional clinic staffing (labelled analyst estimates), and defines the metrics stack to instrument from day one. The scoring logic follows the architecture in [ai-clinic.md](ai-clinic.md): anything administrative or logistical automates fully; anything monitoring-shaped automates with human escalation; anything involving diagnosis, prescribing, dose decisions or abnormal-result interpretation stays human by regulatory design ([SaMD Class B boundary](../10-market-intelligence/malaysia-regulations.md)), with AI limited to preparation and drafting. The stage-level patient experience these processes produce is designed in [ai-patient-journey.md](ai-patient-journey.md); channel mechanics in [malaysia-whatsapp-healthcare.md](../10-market-intelligence/malaysia-whatsapp-healthcare.md) and the [WhatsApp operating model](whatsapp-operating-model.md).

**Last updated: July 2026**

---

## 1. How to read the scores

- **Automation potential** — *Full*: AI/software executes end-to-end, humans handle exceptions only. *Assisted*: AI drafts/monitors/packages; a human decides or signs. *Human-only*: AI may prepare context but the act itself is human (regulatory or relational).
- **Impact** — effect on the researched failure economy: retention revenue ([weight-loss market: retention is the entire business](../10-market-intelligence/malaysia-weight-loss-market.md)), complaint prevention ([T1–T9](../30-patient-reviews/recurring-complaints.md)), doctor-time release ([clinician pain points](../40-doctor-experience/clinician-pain-points.md)), or cost. H/M/L.
- **Complexity** — engineering + integration + safety-assurance effort. H/M/L.
- **Regulatory constraint** — the binding Malaysian rule, if any ([regulations](../10-market-intelligence/malaysia-regulations.md)).
- **AI role** — which [ai-clinic.md](ai-clinic.md) agent owns it.

## 2. Process inventory (44 processes)

### 2.1 Acquisition (A)

| # | Process | Potential | Impact | Complexity | Regulatory constraint | AI role |
|---|---|---|---|---|---|---|
| A1 | CTWA ad response / first-touch reply | Full | H | L | Creative pre-approved (KKLIU); no molecule names | Receptionist |
| A2 | Lead qualification & FAQ handling | Full | H | M | AI answers whitelisted content only | Receptionist |
| A3 | Eligibility screening (structured intake rules) | Assisted | H | M | Administrative screening only — outcome is "consult offered", never "suitable for medication" (SaMD line) | Receptionist + Nurse |
| A4 | Price quoting (all-in, pre-commitment) | Full | H | L | Price-display rules; anti-T1 requirement | Billing |
| A5 | Marketing template campaigns / broadcasts | Assisted | M | L | MASA/KKLIU review; opt-out mandatory; Meta marketing class | Follow-up |
| A6 | Ad-creative compliance linting (molecule/claim blocklist) | Assisted | M | L | MASA 1956; MDA claim-drift risk | Guardrails |
| A7 | Attribution & funnel analytics (conversation-level) | Full | M | M | PDPA purpose limitation | Analytics |

### 2.2 Onboarding (B)

| # | Process | Potential | Impact | Complexity | Regulatory constraint | AI role |
|---|---|---|---|---|---|---|
| B1 | Consent capture (PDPA, purpose-itemised, BM/EN) | Full | H | L | PDPA explicit consent for sensitive data — launch gate | WhatsApp Agent |
| B2 | Booking & slot management | Full | H | M | First GLP-1 visit must be in-person (consult-type rules) | Scheduling |
| B3 | Payment collection & confirmation | Full | H | M | Off-platform payment links (no WhatsApp Pay in MY) | Billing |
| B4 | Pre-consult intake (Flows: history, meds, goals) | Full | H | M | Data minimisation; consent precedes health questions | Care Coordinator |
| B5 | Side-effect expectation-setting education | Full | H | L | Doctor-authored content library | Coach |
| B6 | Chart assembly / pre-consult brief | Assisted | H | M | Brief is decision *support prep*, not decision | Doctor Assistant |
| B7 | Identity verification & record matching | Full | M | M | PDPA accuracy principle | Memory |

### 2.3 Clinical (C)

| # | Process | Potential | Impact | Complexity | Regulatory constraint | AI role |
|---|---|---|---|---|---|---|
| C1 | Diagnosis & suitability decision | **Human-only** | H | — | Medical Act; MMC AI guideline (doctor accountable) | Doctor (AI preps) |
| C2 | Prescribing & dose selection / titration decisions | **Human-only** | H | — | Poisons Act; SaMD Class B if algorithmic | Doctor |
| C3 | Consult scribing (SOAP draft from audio) | Assisted | H | M | Doctor signs; hallucination QA; modest-savings evidence[^1][^2] | Clinical Documentation |
| C4 | WhatsApp-thread → EMR encounter summarisation | Assisted | H | M | MMC record-keeping (chat is not the record) | Clinical Documentation |
| C5 | Structured side-effect check-ins & grading | Assisted | H | M | Protocol-bound; escalation matrix; grade 2+ human | Nurse |
| C6 | Red-flag detection & emergency routing | Assisted | H | H | Deterministic tripwires outside the model; zero-miss audit | Nurse + Guardrails |
| C7 | Routine self-care advice (pre-approved library) | Full | M | L | Doctor-authored, versioned content only | Nurse |
| C8 | Lab ordering & collection logistics | Full | M | M | Doctor orders; AI orchestrates | Care Coordinator |
| C9 | Result explanation drafting | Assisted | H | M | Doctor signs before patient sees anything | Doctor Assistant |
| C10 | Abnormal-result interpretation & action | **Human-only** | H | — | MMC standards | Doctor |
| C11 | MC issuance | **Human-only** (and never post-teleconsult) | M | — | MMC Sep 2025 prohibition — brightest line in MY telehealth | Doctor, in-person only |
| C12 | Referral letters & inter-provider handoffs | Assisted | M | L | Doctor signs | Doctor Assistant |
| C13 | Behavioural coaching cadence | Assisted | H | M | Whitelisted content; disordered-eating escalation | Coach |
| C14 | Ramadan-mode protocol activation | Assisted | H | L | Doctor-reviewed dosing calendars | Coach + Nurse |
| C15 | Adverse-event capture & NPRA reporting prep | Assisted | M | M | Pharmacovigilance duties (e.g., GLP-1 aspiration alert) | Nurse + Compliance |

### 2.4 Fulfilment (D)

| # | Process | Potential | Impact | Complexity | Regulatory constraint | AI role |
|---|---|---|---|---|---|---|
| D1 | e-Rx transmission to dispensary/pharmacy | Full (post-signature) | H | M | OHS 2025 signed-digital-script pathway; Poisons records | Care Coordinator |
| D2 | Dispensing verification | **Human-only** | H | — | Pharmacist legal duty | Pharmacist (AI queues) |
| D3 | Cold-chain courier orchestration & tracking | Full | H | M | GDP-by-analogy documentation | Care Coordinator |
| D4 | Proactive delay notification & recovery | Full | H | L | The anti-T4→T2→T5 chain-breaker | Care Coordinator |
| D5 | Refill forecasting & reorder nudges | Full | H | L | No drug names in templates | Follow-up |
| D6 | Inventory & stock-visibility management | Full | M | M | Batch-level records (counterfeit defence) | Ops systems |
| D7 | Therapeutic-switch communication (shortages) | Assisted | M | L | Doctor decides switch; AI communicates | Coordinator + Doctor |

### 2.5 Billing & payments (E)

| # | Process | Potential | Impact | Complexity | Regulatory constraint | AI role |
|---|---|---|---|---|---|---|
| E1 | Itemised receipts & LHDN e-invoicing | Full | M | M | e-invoice mandate (all clinics from Jul 2026) | Billing |
| E2 | Subscription management & renewal collection | Full | H | M | Consumer Credit Act for BNPL partners | Billing |
| E3 | Failed-payment retry & dunning | Full | H | L | Never care-blocking mid-titration without human review | Billing |
| E4 | Refund execution (published policy, within threshold) | Full | H | L | Auto-triggers on missed SLAs — anti-T5 | Billing |
| E5 | Refund/dispute adjudication (above threshold) | **Human-only** | M | — | Consumer-protection exposure | Finance (AI packages) |
| E6 | Corporate/insurer claim bundling | Assisted | M | M | Panel contract terms | Billing |
| E7 | Revenue reconciliation | Full | M | L | — | Billing |

### 2.6 Retention (F)

| # | Process | Potential | Impact | Complexity | Regulatory constraint | AI role |
|---|---|---|---|---|---|---|
| F1 | Titration check-in cadence (weeks 1–8) | Full (delivery) / Assisted (responses) | H | M | Utility-class messaging; escalation matrix | Nurse + Follow-up |
| F2 | Churn-risk scoring & save-list generation | Full | H | M | PDPA profiling transparency | Follow-up |
| F3 | Human save-calls for flagged patients | **Human-only** | H | — | Evidence: live contact outperforms automation | Nurse/Coach (AI targets) |
| F4 | Month-2 renewal intervention set | Assisted | H | M | No hard-sell scripts (anti-T7) | Follow-up |
| F5 | Plateau-content & expectation management | Assisted | M | L | Clinical claims pre-approved | Coach |
| F6 | Step-down/maintenance tier migration | Full | M | L | Proactive downgrade as trust event | Billing + Follow-up |
| F7 | Reactivation ladders (lapsed segments) | Assisted | M | L | Marketing class: KKLIU + opt-out + caps | Follow-up |
| F8 | Cancellation & off-boarding | Full (process) / Human (conversation) | H | L | One-message cancellation; published refunds | Billing + Doctor offer |

### 2.7 Compliance & governance (G)

| # | Process | Potential | Impact | Complexity | Regulatory constraint | AI role |
|---|---|---|---|---|---|---|
| G1 | Audit logging (AI outputs, gates, overrides) | Full | H | M | MMC/PDPA/MDA evidence spine ([ai-clinic §6.3](ai-clinic.md)) | Infrastructure |
| G2 | Consent-ledger maintenance & opt-out enforcement | Full | H | L | PDPA; Meta opt-out rules (immediate) | WhatsApp Agent |
| G3 | Message archiving to EMR | Full | H | M | MMC record-keeping | WhatsApp Agent |
| G4 | Transcript QA sampling & missed-flag audit | Assisted | H | M | Clinical governance programme; 100% of grade-2/3 threads | QA + clinician |
| G5 | Template/creative compliance workflow | Assisted | M | L | KKLIU 4–6 week lead time; dual review | Guardrails |
| G6 | Breach detection & 72-h notification runbook | Assisted | H | M | PDPA amendment; drilled, not just documented | Security + DPO |
| G7 | Regulatory watch (OHS Act, MDA, Meta policy) | Assisted | M | L | Quarterly review cadence | Compliance |

### 2.8 Analytics (H)

| # | Process | Potential | Impact | Complexity | Regulatory constraint | AI role |
|---|---|---|---|---|---|---|
| H1 | Persistence/retention cohort dashboards | Full | H | M | — | Analytics |
| H2 | Escalation & safety metrics reporting | Full | H | L | Feeds clinical governance | Analytics |
| H3 | Outcome dataset assembly (weight, labs, adherence) | Full | H | M | PDPA research-use consent; anonymisation | Memory + Analytics |
| H4 | Doctor workload & boundary dashboards | Full | M | L | The clinician-experience KPIs ([pain points §6](../40-doctor-experience/clinician-pain-points.md)) | Analytics |
| H5 | Unit-economics & message-cost monitoring | Full | M | L | — | Analytics |

**Tally**: 21 Full · 17 Assisted · 6 Human-only. The human-only set (diagnosis, prescribing, dispensing verification, abnormal-result interpretation, MCs, save-calls/dispute judgment) is exactly the licence-bearing and relationship-bearing core — consistent with the design principle that Welltech automates the clinic *around* the clinician, never the clinician.

### 2.9 Priority quadrant (impact × complexity)

*(analyst placement of the high-impact processes above; low-impact processes omitted)*

| | **Low complexity** | **Medium complexity** | **High complexity** |
|---|---|---|---|
| **High impact** | Quick wins — build first: A1 first-touch reply, A4 all-in quoting, B1 consent, B5 expectation-setting, D4 proactive delay notices, D5 refill nudges, E3/E4 dunning & auto-refunds, F8 clean cancellation | Core machine — the phase-1 spine: A2 qualification, B2/B3 booking & payment, B4 intake Flows, B6 briefs, C3/C4 documentation, C5 check-in grading, C9 result drafting, D1/D3 e-Rx & cold chain, E2 renewals, F1/F2/F4 retention engine, G1 audit log, G3 archiving | Handle with governance: C6 red-flag detection — the only high-impact/high-complexity item, and the one with zero error tolerance; deterministic tripwires + 100% grade-2/3 audit, never "ship and iterate" |
| **Medium impact** | A6 creative linting, C7 advice library, C14 Ramadan mode, F5 plateau content, F6 step-down, H2/H4/H5 dashboards | A7 attribution, B7 identity, C8 labs logistics, C12 referrals, C15 AE capture, D6/D7 inventory & switches, E1/E6 invoicing & claims, F7 reactivation, G4–G6 QA/compliance, H1/H3 cohort & outcome data | — (nothing medium-impact justifies high complexity at launch) |

Reading: the quick-win column is disproportionately *communication* processes — consistent with the research finding that the second failure (silence after a problem) is what converts operational slip-ups into public complaints ([recurring complaints §10.1](../30-patient-reviews/recurring-complaints.md)). Cheap automation buys expensive reputation.

---

## 3. Prioritised build roadmap

Sequencing logic: (1) revenue protection first — the weeks-2–8 persistence machine is the highest-ROI clinical activity in the company ([weight-loss market](../10-market-intelligence/malaysia-weight-loss-market.md)); (2) compliance spine cannot be retrofitted (consent, archiving, audit log ship before patient #1); (3) doctor-time automation scales with doctor headcount, so scribes matter more in phase 2; (4) anything with a 4–6-week external lead time (KKLIU, template review, clinic registration) starts immediately regardless of phase.

### Phase 1 — Launch (months 0–6): "answer, book, monitor, deliver"

| Build | Processes covered | Why now |
|---|---|---|
| WhatsApp channel core: BSP integration, consent ledger, archiving, template library | B1, G2, G3, A5 | Compliance spine + channel viability |
| AI Receptionist + Scheduling + price quoting | A1–A4, B2 | First-response and anti-T1 are the visible differentiators from message one |
| Intake & screening Flows + pre-consult brief v1 | B4–B7, A3 | Prepared consults from day one |
| Payments + receipts + published-refund automation | B3, E1–E4 | Payment-friction and anti-T5 design |
| AI Nurse check-in engine + escalation matrix + red-flag tripwires | C5–C7, F1, C6 | The churn firewall — the business case |
| Fulfilment orchestration + proactive delay notices | D1, D3–D5 | Anti-T4; cold-chain trust |
| Audit log + transcript QA workflow + human console v1 | G1, G4 | Governance from patient #1 |
| Metrics stack v1 (§6) | H1–H2, H5 | Baselines start day 1 |

Phase-1 deliberate exclusions: no scribe dependency for launch (doctors are few; briefs matter more), no churn-ML (rule-based risk flags suffice at small n), no reactivation ladders (nobody has lapsed yet).

### Phase 2 — Scale (months 6–18): "remove the doctor's keyboard, defend month 2"

| Build | Processes covered | Why now |
|---|---|---|
| AI scribe integration + chat-to-EMR summarisation | C3, C4 | Doctor headcount now justifies it; benchmark honestly[^1][^2] |
| Result-explanation drafting + lab-cycle automation | C8, C9 | Labs volume arrives with month-3 panels |
| Churn-risk scoring v2 (learned) + save-call ops + month-2 intervention set | F2–F4 | Enough cohort data to model; the churn cliff is now measurable |
| Coach personalisation + Ramadan mode productised | C13, C14, F5 | First full Ramadan cycle with cohort at scale |
| Billing depth: claims bundling, dunning ladders, step-down automation | E2, E3, E6, F6 | Renewal base exists |
| Reactivation ladders + segment suppression | F7 | Lapsed pool now exists |
| Move BSP layer toward Cloud API direct (>50K msgs/month trigger) | Channel core | Per the [break-even heuristic](../10-market-intelligence/malaysia-whatsapp-healthcare.md) |

### Phase 3 — Advanced (months 18+): "compound the data moat"

| Build | Processes covered | Why now |
|---|---|---|
| Outcome-dataset productisation (anonymised persistence evidence, publishable) | H3 | The proprietary-evidence asset ([WhatsApp healthcare §4.4](../10-market-intelligence/malaysia-whatsapp-healthcare.md)) |
| Fine-tuned/distilled models for Manglish tone, template selection, extraction | Cross-cutting | ≥6 months of QA-labelled transcripts now exist ([ai-clinic §4.1](ai-clinic.md)) |
| Titration decision-support as a **registered Class B SaMD** (optional, deliberate) | C2-adjacent | Only if strategy warrants CAB conformity assessment; never a feature flag |
| Longevity/preventive membership automation (screening cycles, biomarker trends) | C8, H3 | P1→P2 conversion engine ([journey stage 11](ai-patient-journey.md)) |
| Multi-market replication layer (SG/HK panels on shared tech) | Cross-cutting | Market-by-market licensing per [regulations §10](../10-market-intelligence/malaysia-regulations.md) |

### 3.4 Phase gates *(analyst-designed; growth gated the way clinical safety gates a drug launch — [clinician pain points §6.1](../40-doctor-experience/clinician-pain-points.md))*

| Gate | Criteria to pass | If failed |
|---|---|---|
| Launch → open enrolment | Missed-red-flag audit clean over 4 consecutive weeks at pilot volume; consent/archiving verified end-to-end; escalation SLAs met ≥95%; refund automation fires correctly on injected test breaches | Hold marketing spend; fix before scale |
| Phase 1 → Phase 2 | Week-8 cohort persistence ≥ target on ≥200 patients; containment rate ≥60% without CSAT degradation; doctor non-clinical minutes measured ≤10 (path to ≤5); number quality rating "High" sustained | Scale humans, not automation, until quality recovers |
| Phase 2 → Phase 3 | Month-6 persistence beats unmanaged baseline by ≥15pp; ≥6 months QA-labelled transcripts; edit-distance on doctor sign-offs stable (no rubber-stamping drift) | Defer fine-tuning/SaMD projects; data isn't ready |

---

## 4. Make vs buy

| Component | Position | Reasoning |
|---|---|---|
| Orchestration layer (state machine, escalation router, HITL gates) | **Make** | This *is* the company; embeds the escalation matrix and regulatory gates; no vendor sells it Malaysia-shaped |
| Longitudinal memory / patient context store | **Make** | The moat; schema is proprietary ([ai-clinic §5](ai-clinic.md)); vendors would own the data model |
| Conversational agents (prompts, guardrails, advice libraries) | **Make** (on bought models) | BM/EN/Manglish handling and clinical governance are the differentiation |
| LLM models | **Buy** (API, multi-model routing) | Frontier quality unmatchable in-house; benchmark via physician-rubric evals[^3]; abstraction layer prevents lock-in |
| BSP / WhatsApp connectivity | **Buy** — respond.io phase 1 → 360dialog/direct phase 2 | Speed now, economics later ([BSP analysis](../10-market-intelligence/malaysia-whatsapp-healthcare.md)) |
| Ambient scribe | **Buy** + own sign-off UX | Mature vendor category with published benchmarks[^1][^2]; revisit for Manglish edge cases |
| EMR | **Buy** (API-first) | Undifferentiated heavy lifting; non-negotiables: API access, archive ingestion, audit log, e-invoice |
| e-Rx module | **Make thin** on EMR rails | OHS 2025 pathway is specific and load-bearing; small surface |
| Payments/BNPL | **Buy** (HitPay/Curlec/Stripe + Atome et al.) | Regulated, commodity ([pricing §4.4](../50-marketing-intelligence/pricing.md)) |
| Human care console | **Make** (phase 2; BSP inbox phase 1) | Escalation packets need memory + EMR context vendors can't join |
| Guardrails/evals | **Make** core (tripwires, red-team suite, golden sets) + **buy** eval tooling | Safety cases are bespoke; harnesses are commodity |
| Analytics warehouse & dashboards | **Buy** warehouse/BI, **make** metric definitions | Standard stack; definitions are the IP |
| Cold-chain logistics | **Buy** (courier partners) + make the tracking/notification layer | Asset-light; the *communication* layer is the differentiator (anti-T4) |

---

## 5. Cost model: AI-native ops vs traditional clinic staffing

*(analyst estimates, July 2026; 1,000 active programme patients; salaries from Malaysian market norms — clinic nurse RM3.5–4.5K/month, receptionist RM2–2.8K, salaried private GP RM12–16K, dietitian RM4–6K, admin RM2.5–3.5K; +~15% statutory (EPF/SOCSO). Staffing ratios from [ai-clinic.md §7](ai-clinic.md); validate all figures in pilot.)*

### 5.1 Monthly operating cost at 1,000 active patients

| Line | Traditional model | AI-native model | Notes |
|---|---|---|---|
| Reception/booking (3.0 vs 0.5 FTE) | RM7,500 | RM1,400 | AI contains 60–80% of inbound |
| Nursing (4.0 vs 1.5 FTE) | RM16,000 | RM6,000 | Humans handle grade 2+ only |
| Care coordination (2.0 vs 0.5 FTE) | RM6,000 | RM1,500 | State-machine watchdog |
| Doctors (3.0 vs 1.75 FTE) | RM42,000 | RM24,500 | Panels ≈500–650 vs ≈300–350 via prepared consults + async absorption |
| Dietitian/coaching (2.0 vs 0.75 FTE) | RM10,000 | RM3,800 | AI cadence, human sessions |
| Billing/admin (2.0 vs 0.5 FTE) | RM6,000 | RM1,500 | Auto-invoice/refunds |
| Retention ops (1.0 vs 0.25 FTE) | RM3,500 | RM900 | Usually doesn't exist traditionally |
| QA/clinical auditor (0 vs 0.5 FTE) | — | RM2,500 | New AI-governance role |
| AI ops engineering (share) | — | RM4,000 | Fractional across cohorts |
| DPO/compliance (share) | RM1,000 | RM2,000 | Heavier by design (moat) |
| Statutory (~15%) | RM13,800 | RM7,300 | |
| **People subtotal** | **≈RM105,800** | **≈RM55,400** | |
| LLM inference | — | RM4,000–8,000 | Routed: cheap models for volume, frontier for clinical-adjacent |
| BSP/platform licence | — | RM1,000–2,000 | respond.io tier → flat licence at scale |
| Meta messaging fees | RM500 (ad-hoc) | RM500–1,100 | ≈RM0.5–1.05/patient ([modelled](../10-market-intelligence/malaysia-whatsapp-healthcare.md)) |
| Scribe API | — | RM2,000–4,000 | Per-consult pricing |
| EMR + infra + observability | RM2,000 | RM5,000–8,000 | Heavier stack, still cheap vs people |
| **Technology subtotal** | **≈RM2,500** | **≈RM13,000–23,000** | |
| **Total / month** | **≈RM108,000** | **≈RM68,000–78,000** | **≈30–37% lower** |
| **Per patient / month** | **≈RM108** | **≈RM68–78** | |

### 5.2 The real economics are not the cost line

1. **Touchpoint asymmetry.** The traditional RM108/patient buys ~1–2 touches/month (reactive); the AI-native RM68–78 buys 12–15 structured touches plus 24/7 response. Cost per delivered touchpoint falls ~90% *(derived from the two models above)*.
2. **Retention is the multiplier.** Each +10pp of 12-month persistence ≈ RM400–700 LTV/patient ([weight-loss market](../10-market-intelligence/malaysia-weight-loss-market.md)); at 1,000 patients a 10pp persistence gain (≈RM40–70K/month annualised) exceeds the entire cost saving. The automation case is a **revenue** case wearing a cost disguise.
3. **Scaling shape.** Traditional cost scales linearly with patients; AI-native people-cost scales with *exceptions* (≈0.4–0.5 FTE per +100 patients) while technology cost scales with tokens (near-linear but small). At 5,000 patients the models diverge to roughly RM95–105/patient (traditional, unchanged) vs RM45–55 *(analyst extrapolation)*.
4. **Where not to save.** Doctor compensation is deliberately above market ([clinician value proposition](../40-doctor-experience/clinician-pain-points.md)) and human save-calls are deliberately retained — the evidence says live contact outperforms automation where it matters ([WhatsApp healthcare §4.4](../10-market-intelligence/malaysia-whatsapp-healthcare.md)).

### 5.3 Sensitivity *(analyst analysis of the §5.1 model)*

| Assumption stressed | Effect on AI-native model | Break-even observation |
|---|---|---|
| Containment rate 70% → 50% | +0.5–1.0 human FTE (≈RM3–5K/month) | Model still ≈25% cheaper; containment below ~35% erodes most of the people saving |
| Doctor panel 600 → 400 (heavier acuity mix) | +0.5–0.75 doctor FTE (≈RM7–11K/month) | Cost advantage narrows to ~15–20%; the retention upside is unaffected |
| LLM prices double | +RM4–8K/month | Immaterial (<10% of total); inference is not the cost driver, people are |
| Escalation volume 2× (sicker cohort or looser guardrails) | Nurse 1.5 → 2.5 FTE | Still cheaper; but signals guardrail tuning, not staffing, as the fix |
| Persistence uplift only +5pp (not +10pp) | Revenue upside ≈RM20–35K/month | Automation still pays for itself on retention alone at half the assumed effect |

The model is robust to every single-variable stress; the genuinely dangerous scenario is compound (low containment **and** heavy escalation **and** small panels), which is the signature of shipping the conversational layer before the protocol book and guardrails are tuned — the phase gates in §3.4 exist to prevent exactly that sequence.

---

## 6. The metrics stack (instrument from day 1)

Layered like the architecture; every metric has an owner, a target, and an alert threshold. Cohort persistence is the north star; safety metrics gate growth.

| Layer | Metrics (day-1 set) |
|---|---|
| **Safety (gates growth)** | Missed-red-flag audit findings (zero tolerance); grade-2/3 SLA compliance; escalation precision; guardrail-trip log review; adverse events → NPRA; doctor override rate & edit distance (rubber-stamp detector) |
| **Persistence (north star)** | Week-4/8, month-3/6/12 cohort persistence vs unmanaged baselines[^4]; churn-reason taxonomy (side-effect vs cost vs goal-met vs ghosted); save-rate on flagged patients |
| **Funnel** | First-response time; conversation→qualified→booked→enrolled conversions; Flow completion rates; payment completion & recovery; CAC and cost/started-conversation by creative |
| **Experience** | CSAT per journey stage; complaint rate per 100 patients scored against [T1–T9](../30-patient-reviews/recurring-complaints.md); proactive-vs-reactive delay-notification ratio; refund cycle time; cancellation NPS |
| **Clinical outcomes** | % body-weight change at 3/6/12 months; lab-marker deltas; check-in completion; the anonymised outcome dataset (the publishable asset) |
| **Doctor experience** | Non-clinical minutes/doctor/day (≤5 target); after-hours messages reaching doctors (≤3/day); brief-ready rate; note sign-off latency; doctor NPS ([pain-point KPI set](../40-doctor-experience/clinician-pain-points.md)) |
| **Channel & AI ops** | Number quality rating; template rejection rate; containment rate; misroute rate; LLM cost/patient; eval-suite pass rates per release; model drift dashboards |
| **Unit economics** | Cost/patient/month vs §5 model; cost/touchpoint; LTV:CAC by cohort; messaging spend per patient |

Instrumentation rules: (a) every AI decision carries model + prompt version for cohort-level attribution of quality changes; (b) metrics compute from the same event log that serves audit (§G1) — one spine, two consumers; (c) publish a quarterly internal "complaint-taxonomy scorecard" — the researched incumbent failures as Welltech's standing QA checklist ([recurring complaints §11](../30-patient-reviews/recurring-complaints.md)).

---

## 7. Automation anti-patterns (what this map deliberately avoids)

| Anti-pattern | Why it fails here | This map's counter-position |
|---|---|---|
| Automating the doctor's judgment to cut the biggest cost line | SaMD Class B registration trigger; MMC accountability; the researched market *trusts clinicians and punishes administration* ([recurring complaints §15](../30-patient-reviews/recurring-complaints.md)) | Six human-only processes are load-bearing by design; doctors get leverage, not replacement |
| Chatbot-first, workflow-later (a bot bolted onto manual ops) | The Malaysian incumbent pattern — keyword bots over unstructured inboxes ([WhatsApp healthcare §8.1](../10-market-intelligence/malaysia-whatsapp-healthcare.md)); the bot answers, then the T4→T2→T5 chain fires anyway | Orchestration/state machine is the phase-1 core; conversation is its interface |
| Marketing-blast economics | Pays RM0.30–0.45/message, degrades number quality, triggers MASA exposure | Service-led messaging; marketing class confined to stage-12 reactivation |
| Automating retention as pressure (win-back scripts, exit friction) | Recreates the slimming-centre T7 record that defines the category's reputation | Retention by service quality; one-message cancellation is itself automated |
| Shipping unmeasured automation | Cannot prove safety to MMC, value to the board, or improvement to itself | The §6 metrics stack and audit spine are phase-1 deliverables, not phase-3 polish |

## 8. Bottom line

Of 44 clinic processes, 21 automate fully and 17 more become AI-drafted/human-signed; the six that remain human-only are precisely the acts Malaysian law and good medicine reserve for licensed judgment. The build order follows the money and the law:

1. **Phase 1 buys trust and safety** — consent, archiving, audit, instant response, honest prices, kept delivery promises, and the weeks-2–8 check-in engine.
2. **Phase 2 buys doctor leverage and month-2 revenue** — scribes, result drafting, churn scoring, save-calls, renewals.
3. **Phase 3 buys the moat** — the outcome dataset, tuned local-language models, and (only deliberately) regulated decision support.

The cost model says an AI-native clinic runs ~30–37% cheaper per patient and is robust to every single-variable stress (§5.3) — but the decisive line is that it delivers an order of magnitude more care touches, and in a category where half of unmanaged patients quit within a year[^4], those touches *are* the revenue.

---

## References

[^1]: STAT News, "Large AI scribe study finds modest time savings, inconsistent use" (Apr 2026) — 16 min documentation time saved per 8 h of care across 1,800 clinicians, https://www.statnews.com/2026/04/01/ai-ambient-scribes-modest-time-savings-clinical-documentation/ (accessed July 2026).
[^2]: American Hospital Association, "6 Health Systems Enhancing Care Delivery with Ambient AI Scribes" (Apr 2026) — Cleveland Clinic −14 min/day in EHR; Cooper University Healthcare 4.15 min/patient, https://www.aha.org/aha-center-health-innovation-market-scan/2026-04-14-6-health-systems-enhancing-care-delivery-ambient-ai-scribes (accessed July 2026).
[^3]: OpenAI HealthBench — physician-rubric evaluation of health LLM conversations (262 physicians, 48,562 criteria), the reference pattern for Welltech's eval suite, https://www.mobihealthnews.com/news/openai-unveils-healthbench-evaluate-llms-safety-healthcare (accessed July 2026).
[^4]: Medscape, "Real-World Study Finds Over 50% Stop GLP-1s Within 1 Year" (2025) — Danish cohort n=77,310: 18%/31%/52% discontinuation at 3/6/12 months, https://www.medscape.com/viewarticle/real-world-study-finds-over-50-stop-glp-1s-within-1-year-2025a1000obm (accessed July 2026).
