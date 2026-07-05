# Phase 0 Handoff — Start-Here for the Execution Session

**Read this first. It is written so a fresh session (human or AI) with no prior context can pick up Welltech's Phase 0 and start executing.** It carries the essential context, the Phase 0 scope and definition-of-done, the sequenced critical path, the facts you should not have to re-derive, the hard constraints, and a ready-to-paste kickoff prompt. Everything points back into the repository for depth.

Last updated: July 2026. Repo: this folder (`welltech-intelligence/`). Git branch: `claude/welltech-health-intelligence-5zytb2` — keep committing and pushing work here.

---

## 1. 60-second context

**Welltech** is building the first *outcome-accountable, retention-led, WhatsApp-native* medical clinic for weight / metabolic / longevity care in Southeast Asia — **Malaysia first**, then Singapore, then Hong Kong. The wedge product is a **doctor-led medical weight-loss (GLP-1) programme** delivered on WhatsApp with an AI-operated care model, so a small clinical team can run continuous, high-touch care at a cost structure incumbents can't match.

**Why it works (the thesis):** demand is epidemiological (54.4% of Malaysian adults overweight/obese, 15.6% diabetic); GLP-1 drugs just arrived; and across ~40 competitors in three markets **no one combines medical prescribing + retention infrastructure + WhatsApp-native care + published outcomes** — because their economics punish continuous care. The window before an incumbent copies is ~6–24 months. The defensible move is to build the slow-to-copy assets first: **published local retention/outcome data**, WhatsApp clinical ops, and locked partners.

Full thesis: [REVIEW-GUIDE.md](REVIEW-GUIDE.md) → [00-executive-summary/malaysia-executive-summary.md](00-executive-summary/malaysia-executive-summary.md).

## 2. The money and where Phase 0 sits

**US$500K secured** (≈ RM2.35M), marketing-weighted. This is the **"prove the Malaysia wedge" tranche**, not the full build (that needs ~US$5M). Its job: reach a Series-A-unlocking proof point. The plan is three phases inside the $500K; **Phase 0 is Weeks 0–8: get legal, built, and connected so the first patient can be seen.** Near-zero marketing in Phase 0.

Full plan: [70-welltech-blueprint/build-roadmap.md](70-welltech-blueprint/build-roadmap.md) (read §4 Phase 0 and §5 spend plan).

## 3. Phase 0 objective & definition of done

**Objective:** a compliant, working MVP and the partnerships/licences in place to legally acquire, consult, prescribe to, fulfil, and monitor the first patient — end to end.

**Definition of done (the gate to Phase 1):**

> A real patient can be **acquired → consulted → prescribed → fulfilled → monitored**, legally and end-to-end, with consent captured, records archived, and an audit trail — and legal + clinical sign-off obtained.

## 4. Phase 0 workstreams

Grouped by owner-type. Items marked ⏱ have 4–6 week external lead times — **start them on day 1 regardless of build progress.**

**A. Entity & legal**
- Incorporate the operating entity (SSM); bank account; accounting/bookkeeping set up.
- ⏱ Legal opinion + structure on the **virtual-clinic model**: the defensible structure is a *registered physical clinic* anchoring prescriptions with the platform as a tech/services layer (there is no PHFSA category for virtual-only clinics). Confirm with local counsel.
- Engage a healthcare lawyer for the sign-off items in [90-verification/regulatory-verification.md](90-verification/regulatory-verification.md) §"Requires healthcare-lawyer sign-off".

**B. Regulatory & compliance** (see [10-market-intelligence/malaysia-regulations.md](10-market-intelligence/malaysia-regulations.md))
- ⏱ Register the anchor clinic (PHFSA / relevant licensing).
- ⏱ Stand up the **KKLIU/MAB advertising-approval pipeline** (every consumer health creative needs approval, ~4–6 weeks; you cannot advertise prescription drugs to the public at all — market the *programme*, never the molecule).
- PDPA setup: appoint a DPO, consent architecture, a Transfer Impact Assessment for cross-border data (WhatsApp/Meta, cloud, AI vendors).
- Confirm the **e-prescription pathway** is legally valid for Group B poisons (Poisons Act 1952) — partner a compliant e-Rx rail rather than rebuilding it.
- **Do NOT** issue MCs after teleconsult-only encounters (MMC ban, Sept 2025).

**C. Clinical setup**
- Contract a **Medical Director** (fractional → part-time) — accountable clinician, protocol author, sign-off authority.
- Contract the first **sessional doctors** (paid per consult — variable cost).
- Author + sign the **GLP-1 clinical protocol**: titration schedule against *current* product labels, red-flag/stop-rule escalation matrix, BMI ≥27.5 initiation threshold + contraindication screen, peri-operative hold. (Do not ship the clinic-blog version — a clinician must approve against the label.) See sign-off list in [90-verification/regulatory-verification.md](90-verification/regulatory-verification.md) §"Requires medical-director sign-off".

**D. Product / build (MAKE — the moat)** (see [60-ai-operating-model/](60-ai-operating-model/))
- MVP **orchestration layer** (state machine + escalation router + human-in-the-loop gates).
- **Longitudinal patient-memory / context store** (proprietary schema).
- **WhatsApp intake → consult → enrolment flow v1** + the AI agent behaviour on top of the bought LLM + BSP.
- **Compliance spine — ships before patient #1:** consent ledger, record archiving, append-only audit log.
- Core **care protocols** encoded (from workstream C).

**E. Buy / subscribe (set up accounts)** (see [60-ai-operating-model/automation.md §4](60-ai-operating-model/automation.md))
- LLM API access + multi-model routing (with an abstraction layer to avoid lock-in).
- **respond.io** BSP + a verified WhatsApp Business number + approved message templates.
- EMR (API-first: must have API access, audit log, e-invoice).
- Payments: HitPay / Curlec / Stripe + Atome (instalments).
- Cloud hosting; analytics/BI; eval tooling.

**F. Partnerships to lock** (compete-vs-partner logic in [20-competitor-dossiers/competitor-comparison.md](20-competitor-dossiers/competitor-comparison.md))
- **Fulfilment / pharmacy + cold-chain:** Alpro (or equivalent) — GLP-1 is cold-chain; own the tracking/notification layer.
- **E-prescription rails:** a DOC2US / Teleme-style compliant partner.
- **Labs:** BP Healthcare / Pathlab / Innoquest for baseline bloods (B2B rates).
- **Bariatric / specialist referral:** an escalation pathway (e.g. a Gleneagles/Prince Court/Sunway weight or bariatric service).

## 5. The 8-week critical path (sequence)

| Weeks | Focus |
|---|---|
| **1** | Kick off ALL ⏱ lead-time items day 1: clinic registration, KKLIU pipeline, legal structure opinion. Incorporate entity. Contract Medical Director. Open LLM/BSP/EMR/payment/cloud accounts. |
| **2–3** | Build compliance spine (consent, archive, audit) + orchestration-layer skeleton + patient-memory store. Draft GLP-1 clinical protocol with Medical Director. Begin partner conversations (Alpro, e-Rx, labs, referral). |
| **3–5** | Build WhatsApp intake→consult→enrolment flow v1; wire LLM + respond.io; connect EMR + payments. Submit first KKLIU creatives. Sign fulfilment + e-Rx + lab partners. |
| **5–7** | Integrate e-prescription + fulfilment + labs end-to-end. Load signed clinical protocols. PDPA/DPO live. Contract first sessional doctors. |
| **7–8** | **End-to-end test patient**: acquire → consult → e-Rx → fulfil (cold-chain) → first WhatsApp check-in. Legal + clinical sign-off. Fix gaps. |
| **Gate** | The definition-of-done in §3 is met → proceed to Phase 1 (launch & prove). |

## 6. Facts you shouldn't have to re-derive

- **Pricing (planned):** RM49 credited entry consult; **RM999/month flat-across-titration** core weight programme (drug included; flat price disarms the month-3–4 dose-escalation churn); premium tier ~RM1,599; longevity membership RM3,600–8,800/yr. Rationale: [70-welltech-blueprint/pricing-strategy.md](70-welltech-blueprint/pricing-strategy.md).
- **Unit economics (illustrative):** target CAC ≈ RM650/enrolled patient; LTV:CAC ≈ 3.8×; **retention is the #1 lever** (each +10pp of 12-month retention ≈ RM900–1,000/patient). Model: [70-welltech-blueprint/financial-model.md](70-welltech-blueprint/financial-model.md).
- **Make-vs-buy rule:** touches the patient relationship, clinical logic, or data model → **MAKE**; plumbing → **BUY**.
- **Channel:** WhatsApp is the care rail (~90%+ Malaysian reach); acquisition is click-to-WhatsApp + SEO/content + doctor-KOL — **not** paid drug-keyword ads (illegal).
- **FX:** US$1 ≈ RM4.70.

## 7. Hard constraints & caveats (do-not-skip)

- **Compliance spine before patient #1** — consent, archiving, audit log are not retrofittable.
- **Never advertise the molecule** (Ozempic/Wegovy/Mounjaro) to the public; market the programme. KKLIU/MAB approval on every creative.
- **No tele-only MCs.** **No AI diagnosing/dosing** — AI prepares and drafts; a licensed doctor decides and signs (SaMD Class B boundary).
- **Two figures to treat with care** (from the verification pass, [90-verification/README.md](90-verification/README.md)): the competitor NOVI "708-patient / 12.7%" outcome stat is *uncorroborated* — don't repeat it externally; and the unmanaged GLP-1 retention baseline may be drifting — Phase 1's real job is to *measure* retention honestly.
- **Confirm drug-distributor terms early** — they set your real margin (flagged unvalidated in the model).
- **Marketing stays near-zero in Phase 0.** The marketing budget is gated behind the Phase-1 proof, not spent at launch.

## 8. Where to read more (repo map)

- Plan & budget: [70-welltech-blueprint/build-roadmap.md](70-welltech-blueprint/build-roadmap.md), [implementation-roadmap.md](70-welltech-blueprint/implementation-roadmap.md), [malaysia-go-to-market.md](70-welltech-blueprint/malaysia-go-to-market.md)
- Operating model: [60-ai-operating-model/](60-ai-operating-model/) (ai-clinic, ai-doctor, ai-nurse, whatsapp-operating-model, automation, ai-patient-journey)
- Regulation: [10-market-intelligence/malaysia-regulations.md](10-market-intelligence/malaysia-regulations.md); sign-off lists in [90-verification/regulatory-verification.md](90-verification/regulatory-verification.md)
- Clinical/prescribing: [40-doctor-experience/prescribing-models.md](40-doctor-experience/prescribing-models.md)
- Growth (for Phase 1 prep): [50-marketing-intelligence/](50-marketing-intelligence/) (funnels, seo, paid-search, positioning, pricing)
- Trust map / what to caveat: [90-verification/README.md](90-verification/README.md)

## 9. First actions for the new session

1. Read this handoff, then [build-roadmap.md](70-welltech-blueprint/build-roadmap.md) §4 (Phase 0) and §5 (spend).
2. Turn §4 + §5 into a **week-by-week Phase 0 project plan** with named owners, dependencies, and the ⏱ lead-time items started on day 1.
3. Draft the **partner outreach one-pagers** (fulfilment, e-Rx, labs, referral) and the **Medical Director role spec**.
4. Draft the **regulatory task list** (clinic registration, KKLIU pipeline, PDPA/DPO, e-Rx validity) with the legal questions for counsel.
5. Draft the **MVP build spec** (orchestration layer, memory store, WhatsApp flow, compliance spine) an engineer or dev partner could start on.
6. Keep committing to branch `claude/welltech-health-intelligence-5zytb2`.

## 10. Open decisions for the founder (surface early)

- Anchor-clinic model: partner an existing registered clinic, or register a new one?
- Build team: in-house engineer(s) vs a trusted dev partner for the MVP?
- First fulfilment partner: Alpro vs alternative — and the data/patient-ownership terms.
- Medical Director: who, and fractional vs part-time?
- Klang Valley launch geography and the first beachhead persona (see [10-market-intelligence/malaysia-consumer-behaviour.md](10-market-intelligence/malaysia-consumer-behaviour.md)).

---

### Ready-to-paste kickoff prompt for the new session

> I'm executing **Phase 0** of the Welltech build (Weeks 0–8: get legal, built, and connected so the first patient can be seen). Read `welltech-intelligence/PHASE-0-HANDOFF.md` first, then `welltech-intelligence/70-welltech-blueprint/build-roadmap.md` (§4 Phase 0, §5 spend). We have US$500K secured (marketing-weighted, gated behind the Phase-1 proof). Start by turning the Phase 0 workstreams into a week-by-week project plan with owners, dependencies, and the 4–6-week lead-time items flagged to start day 1 — then help me draft the partner outreach one-pagers, the Medical Director spec, the regulatory task list, and the MVP build spec. Commit work to branch `claude/welltech-health-intelligence-5zytb2`.
