# Phase 0 Handoff — Start-Here for the Execution Session

**Read this first. It is written so a fresh session (human or AI) with no prior context can pick up NewCo's Phase 0 and start executing.** It carries the essential context, the corporate/commercial structure, the Phase 0 scope and definition-of-done, the sequenced critical path, the facts you should not have to re-derive, the hard constraints, and a ready-to-paste kickoff prompt. Everything points back into the repository for depth.

Last updated: July 2026. Repo: this folder (`welltech-intelligence/`). Git branch: `claude/welltech-health-intelligence-5zytb2` — keep committing and pushing work here.

---

## 1. 60-second context

**NewCo** (a subsidiary of **WellTech Health**) is building the first *outcome-accountable, retention-led, WhatsApp-native* medical weight-loss / longevity service in Malaysia — **piloting through WellTech's existing Medimind KL clinic**. The wedge is a **doctor-led medical weight-loss (GLP-1) programme** delivered on WhatsApp with an AI-operated care model, so a small team can run continuous, high-touch care at a cost structure incumbents can't match. (Longevity/metabolic is a fast-follow on the same chassis. Singapore and Hong Kong come much later.)

**Why it works (the thesis):** demand is epidemiological (54.4% of Malaysian adults overweight/obese, 15.6% diabetic); GLP-1 drugs just arrived; and across ~40 competitors in three markets **no one combines medical prescribing + retention infrastructure + WhatsApp-native care + published outcomes** — because their economics punish continuous care. The window before an incumbent copies is ~6–24 months. The defensible move is to build the slow-to-copy assets first: **published local retention/outcome data (owned by NewCo)**, WhatsApp clinical ops, and the care-orchestration IP.

Full thesis: [REVIEW-GUIDE.md](REVIEW-GUIDE.md) → [00-executive-summary/malaysia-executive-summary.md](00-executive-summary/malaysia-executive-summary.md).

## 2. Corporate & commercial structure (the setup that makes Phase 0 low-barrier)

The pilot uses WellTech's existing assets, but keeps the **fundable assets inside NewCo** (Option A) so it can raise externally / spin out later.

| Party | Role |
|---|---|
| **NewCo** (subsidiary) | Owns the **brand, patient relationship, recurring revenue, the retention/outcome dataset (the moat), and the care-orchestration IP.** Builds/runs the WhatsApp service; collects the fee; owns the data. |
| **WellTech Health** (parent) | **Shareholder + funder** of this tranche; **arm's-length service provider** (via Medimind) + **software licensor** (clinic OS). Paid at fair market value. |
| **Medimind KL** (WellTech clinic) | The **regulated clinical act** — its **2 doctors** run the telehealth consults, prescribe, and **dispense from its own pharmacy**. The **doctor keeps the full consult fee (100%)**. Medimind **adds GLP-1 to its pharmacy formulary** and dispenses it. |

**What this removes from Phase 0:** clinic registration, doctor recruitment, external fulfilment, and an EMR purchase — Medimind (clinic + doctors + pharmacy) and WellTech's **clinic operations software** (mature: EMR, pharmacy/inventory, billing/payments, appointments) already exist. **The same WellTech engineers who built the clinic OS build NewCo's service.**

**Drug economics (all-in RM999; margin in NewCo).** Medimind does not currently stock GLP-1s, so **Medimind adds GLP-1 to its pharmacy formulary** — procuring via its existing distributor accounts (Zuellig/DKSH/Pharmaniaga) and dispensing in-house under its own licence (a new SKU, not a new capability). The programme is priced **all-in RM999/month (drug included)** and **NewCo collects the full patient payment**. The **doctor keeps the full consult fee (100%)** — the cleanest fee-for-service structure (NewCo takes no cut of the clinical fee, which keeps it clear of MMC fee-splitting). Medimind bills NewCo **drug-at-cost + a dispensing fee**; **NewCo's revenue is the programme/care fee + a modest drug margin marked into the RM999** (not pure pass-through — because with the doctor keeping the full consult fee and the drug at cost, pure pass-through would squeeze NewCo's contribution). NewCo holds **no** pharmacy/wholesale licence (it rides Medimind's pharmacy). **NewCo-as-drug-wholesaler is deferred to Phase 2** (direct-sourcing margin lever; needs a Type A poisons licence; pays off at multi-clinic volume). **The one live economic action: obtain Medimind's GLP-1 distributor cost** — it is the #1 unvalidated input and sets the real margin.

**Compliance guardrails to bake into the founding/service agreements (with counsel):**
- **Fair-market fee-for-service to Medimind** — *not* a referral kickback or a split of the consult fee (MMC fee-splitting rules).
- **NewCo does not practise medicine** — the consult/diagnosis/prescription stays with **Medimind's licensed doctor**, who keeps clinical independence (freedom to decline to prescribe).
- **IP + patient-data ownership assigned to NewCo** (license the clinic OS to NewCo; assign the new-service IP to NewCo).
- **PDPA consent covers the dual-entity flow** (NewCo owns the data *and* shares with Medimind for care).

Full structure + spend: [70-welltech-blueprint/build-roadmap.md](70-welltech-blueprint/build-roadmap.md) §2–§5.

## 3. The money and where Phase 0 sits

**US$500K — WellTech-funded (intra-group)** (≈ RM2.35M), marketing-weighted. This is the **"prove the Medimind KL pilot"** tranche, not the full build (that needs ~US$5M). It **stretches further** because the clinic, doctors, pharmacy, clinic OS, and engineers already exist — so more goes to **marketing + the new-service build**. **Phase 0 is Weeks 0–8: get structured, built, and connected so the first patient can be seen.** Near-zero marketing in Phase 0.

## 4. Phase 0 objective & definition of done

**Objective:** a compliant, working service and the agreements/integration in place to legally acquire, refer, treat (via Medimind), and monitor the first patient — end to end.

**Definition of done (the gate to Phase 1):**

> A real patient can be **acquired on WhatsApp → referred to a Medimind doctor → consulted / prescribed / dispensed in the clinic OS → monitored by NewCo**, legally and end-to-end, with **consent captured and clinical + outcome data flowing into NewCo's store** — and legal + clinical sign-off obtained.

## 5. Phase 0 workstreams

Grouped by owner-type. Items marked ⏱ have external lead times — **start them on day 1.**

**A. Entity, legal & commercial**
- Incorporate **NewCo** as a WellTech subsidiary; bank account; accounting.
- ⏱ Draft + sign the **WellTech ↔ NewCo ↔ Medimind service agreement**: fair-market fee-for-service (doctor time + drug-at-cost + dispensing), **IP + patient-data assigned to NewCo**, clinic-OS licensed to NewCo.
- ⏱ Counsel sign-off on **fee-splitting / practice-of-medicine structuring** and the items in [90-verification/regulatory-verification.md](90-verification/regulatory-verification.md) §"Requires healthcare-lawyer sign-off". *(No clinic registration — Medimind is already registered.)*

**B. Regulatory & compliance** (see [10-market-intelligence/malaysia-regulations.md](10-market-intelligence/malaysia-regulations.md))
- ⏱ Stand up the **KKLIU/MAB advertising-approval pipeline** (~4–6 weeks; never advertise the molecule — market the programme).
- **PDPA setup:** DPO, **dual-entity consent architecture** (NewCo owns + shares with Medimind), TIA for cross-border data (WhatsApp/Meta, cloud, AI vendors).
- Confirm the **in-house dispensing pathway** at Medimind (GP dispensing — the clinic OS's electronic prescription → dispense queue is sufficient; **no signed/external e-Rx needed for the pilot**; that's a Phase-2 item when serving external pharmacies).
- **Do NOT** issue MCs after teleconsult-only encounters (MMC ban, Sept 2025).

**C. Clinical setup**
- Confirm the **Medimind accountable doctor** as Medical Director (protocol author, sign-off authority) and the two telehealth doctors. The **doctor keeps the full consult fee**.
- **Medimind adds GLP-1 to its pharmacy formulary** (procure via existing distributor accounts; dispense in-house) and **obtains the distributor cost** — the #1 economic input.
- Author + sign the **GLP-1 clinical protocol** (weight-loss/GLP-1 is the v1 scope; longevity is a fast-follow): titration schedule against *current* product labels, red-flag/stop-rule escalation matrix, BMI ≥27.5 initiation threshold + contraindication screen, peri-operative hold. (A clinician must approve against the label, not a clinic blog.) See [90-verification/regulatory-verification.md](90-verification/regulatory-verification.md) §"Requires medical-director sign-off".

**D. Product / build (MAKE — the moat, built by WellTech engineers)** (see [60-ai-operating-model/](60-ai-operating-model/))
- MVP **orchestration layer** (state machine + escalation router + human-in-the-loop gates).
- **Longitudinal patient-memory / context store** (proprietary, NewCo-owned schema).
- **WhatsApp intake → eligibility → payment → booking-handoff-to-Medimind flow v1** + the AI agent behaviour on top of the bought LLM + BSP.
- **Clinic-OS ↔ NewCo integration + data/consent bridge** — push consult-completed / prescription-issued / dispensed / lab-results into NewCo's store so the cohort dataset builds itself.
- **Compliance spine — ships before patient #1:** consent ledger, record archiving, append-only audit log.
- Core **care protocols** encoded (from workstream C).

**E. Buy / subscribe (set up accounts)** (see [60-ai-operating-model/automation.md §4](60-ai-operating-model/automation.md))
- LLM API access + multi-model routing (abstraction layer to avoid lock-in).
- **respond.io** BSP + a verified WhatsApp Business number + approved message templates.
- Payments: reuse the clinic OS's **FIUU** gateway where possible + Atome (instalments).
- Cloud hosting; analytics/BI; eval tooling. *(No EMR buy — reuse the WellTech clinic OS.)*

**F. Reuse WellTech assets (internal, not external partners)**
- **Clinic OS** licensed to NewCo + integrated (workstream D).
- **Medimind** doctors (consult/prescribe) + pharmacy (dispensing) + its existing **lab arrangements** for baseline bloods.
- *(Phase 2, deferred: external fulfilment (Alpro), signed/external e-Rx rail, NewCo drug wholesale.)*

## 6. The 8-week critical path (sequence)

| Weeks | Focus |
|---|---|
| **1** | Kick off ALL ⏱ items day 1: **service agreement** (IP/data to NewCo, doctor keeps full consult fee), **KKLIU pipeline**, counsel on fee-splitting/practice-of-medicine. Incorporate NewCo. Confirm Medimind Medical Director + doctors. **Medimind adds GLP-1 to formulary + obtains distributor cost.** Open LLM/BSP/payment/cloud accounts; license + start integrating the clinic OS. |
| **2–3** | Build compliance spine (consent, archive, audit) + orchestration-layer skeleton + patient-memory store + **clinic-OS integration bridge**. Draft GLP-1/longevity protocol with the Medimind doctor. |
| **3–5** | Build WhatsApp intake → eligibility → payment → booking-handoff flow v1; wire LLM + respond.io; connect payments; complete the data/consent bridge. Submit first KKLIU creatives. |
| **5–7** | End-to-end wiring: acquisition → referral → Medimind consult/prescribe/dispense (clinic OS) → data back to NewCo → monitoring. Load signed clinical protocols. PDPA/DPO + dual-entity consent live. |
| **7–8** | **End-to-end test patient**: acquire → refer → consult → dispense (Medimind) → first WhatsApp check-in, with data + consent flowing to NewCo. Legal + clinical sign-off. Fix gaps. |
| **Gate** | The definition-of-done in §4 is met → proceed to Phase 1 (launch & prove). |

## 7. Facts you shouldn't have to re-derive

- **Pricing (planned):** RM49 credited entry consult; **RM999/month flat-across-titration** core weight programme (**all-in, drug included; NewCo collects. Doctor keeps the full consult fee; Medimind adds GLP-1 to formulary and bills drug-at-cost + dispensing; NewCo's revenue = programme fee + a modest drug margin**); premium tier ~RM1,599; longevity membership RM3,600–8,800/yr (fast-follow, not v1). Rationale: [70-welltech-blueprint/pricing-strategy.md](70-welltech-blueprint/pricing-strategy.md).
- **Unit economics (illustrative):** target CAC ≈ RM650/enrolled patient; LTV:CAC ≈ 3.8×; **retention is the #1 lever** (each +10pp of 12-month retention ≈ RM900–1,000/patient). Model: [70-welltech-blueprint/financial-model.md](70-welltech-blueprint/financial-model.md).
- **Make-vs-buy-vs-reuse:** touches the patient relationship, clinical logic, or data model → **MAKE** (keep in NewCo); WellTech already owns it → **REUSE** (licensed at fair value); plumbing → **BUY**.
- **Channel:** WhatsApp is the care rail (~90%+ Malaysian reach); acquisition is click-to-WhatsApp + SEO/content + doctor-KOL — **not** paid drug-keyword ads (illegal).
- **Drug COGS:** = Medimind's GLP-1 distributor cost once GLP-1 is added to formulary (**obtain this — the #1 economic input; sets the real margin**).
- **FX:** US$1 ≈ RM4.70.

## 8. Hard constraints & caveats (do-not-skip)

- **Get the ownership right:** IP, patient-data, brand, and recurring revenue **must be assigned to NewCo** in the founding docs — or NewCo owns nothing to raise against.
- **Fair-market fee-for-service to Medimind**, not a referral cut (MMC fee-splitting). **NewCo does not practise medicine** — the medical act stays with the licensed doctor.
- **Compliance spine before patient #1** — consent, archiving, audit log are not retrofittable.
- **Never advertise the molecule** (Ozempic/Wegovy/Mounjaro); market the programme. KKLIU/MAB approval on every creative.
- **No tele-only MCs.** **No AI diagnosing/dosing** — AI prepares and drafts; a Medimind doctor decides and signs (SaMD Class B boundary).
- **Two figures to treat with care** (verification pass, [90-verification/README.md](90-verification/README.md)): the competitor NOVI "708-patient / 12.7%" outcome stat is *uncorroborated* — don't repeat it externally; and the unmanaged GLP-1 retention baseline may be drifting — Phase 1's real job is to *measure* retention honestly.
- **Marketing stays near-zero in Phase 0** — gated behind the Phase-1 proof, not spent at launch.

## 9. Where to read more (repo map)

- Plan & budget: [70-welltech-blueprint/build-roadmap.md](70-welltech-blueprint/build-roadmap.md), [implementation-roadmap.md](70-welltech-blueprint/implementation-roadmap.md), [malaysia-go-to-market.md](70-welltech-blueprint/malaysia-go-to-market.md)
- Operating model: [60-ai-operating-model/](60-ai-operating-model/) (ai-clinic, ai-doctor, ai-nurse, whatsapp-operating-model, automation, ai-patient-journey)
- Regulation: [10-market-intelligence/malaysia-regulations.md](10-market-intelligence/malaysia-regulations.md); sign-off lists in [90-verification/regulatory-verification.md](90-verification/regulatory-verification.md)
- Clinical/prescribing: [40-doctor-experience/prescribing-models.md](40-doctor-experience/prescribing-models.md)
- Growth (for Phase 1 prep): [50-marketing-intelligence/](50-marketing-intelligence/) (funnels, seo, paid-search, positioning, pricing)
- Trust map / what to caveat: [90-verification/README.md](90-verification/README.md)

## 10. First actions for the new session

1. Read this handoff, then [build-roadmap.md](70-welltech-blueprint/build-roadmap.md) §2 (structure), §4 (Phase 0), §5 (spend).
2. Turn §5–§6 into a **week-by-week Phase 0 project plan** with named owners, dependencies, and the ⏱ lead-time items started on day 1.
3. Draft the **WellTech ↔ NewCo ↔ Medimind service agreement term sheet** (fair-market fee-for-service, IP + data to NewCo, clinic-OS licence) for counsel.
4. Draft the **clinic-OS ↔ NewCo integration spec** (events to push: consult-completed, prescription-issued, dispensed, lab-results; the consent model) — for the WellTech engineers.
5. Draft the **MVP build spec** (orchestration layer, memory store, WhatsApp flow, compliance spine) and the **regulatory task list** (KKLIU pipeline, PDPA/DPO dual-entity consent, fee-splitting structuring).
6. Keep committing to branch `claude/welltech-health-intelligence-5zytb2`.

## 11. Open decisions for the founder (surface early)

*Resolved:* anchor clinic = **Medimind KL**; build team = **WellTech's engineers**; Medical Director = **a Medimind doctor**; dispensing = **Medimind pharmacy**; ownership = **Option A (assets in NewCo)**.
- **Drug supply** = **Medimind adds GLP-1 to its formulary** (procures via its distributor accounts; dispenses in-house). NewCo holds no drug licence; wholesale deferred to Phase 2.
- **Consult fee** = the **doctor keeps the full consult fee (100%)**. NewCo takes no cut of the clinical fee.
- **Margin structure** = NewCo's revenue is the **programme fee + a modest drug margin** (Medimind bills drug-at-cost + dispensing; NewCo marks a modest margin into the all-in RM999).
- **Pilot volume** = ~**50 soft launch → 200–300 total** enrolled (clears the ≥200 week-8 retention read).
- **Scope** = **weight-loss/GLP-1 only in v1**; longevity/metabolic is a fast-follow on the same chassis.

*Still open:*
- **Medimind's actual GLP-1 distributor cost** — obtain it (the #1 economic input; a now-internal check).
- The exact **programme-fee vs drug-margin split** inside the RM999 — set once the distributor cost is known.
- Klang Valley beachhead **persona / geography** within Medimind's catchment (see [10-market-intelligence/malaysia-consumer-behaviour.md](10-market-intelligence/malaysia-consumer-behaviour.md)).

---

### Ready-to-paste kickoff prompt for the new session

> I'm executing **Phase 0** for **NewCo** — a WellTech Health subsidiary running a WhatsApp-native **medical weight-loss (GLP-1) service (v1; longevity is a fast-follow)**, piloting through WellTech's **Medimind KL** clinic (its 2 doctors consult + prescribe and **keep the full consult fee**; its pharmacy **adds GLP-1 to formulary** and dispenses) and integrating with WellTech's existing **clinic operations software** (EMR/pharmacy/billing/appointments). NewCo builds the standalone WhatsApp + AI care-orchestration layer that brackets the Medimind encounter, prices the programme **all-in RM999** (NewCo revenue = programme fee + a modest drug margin), targets a **~50 soft-launch → 200–300 pilot**, and **owns the brand, patient data, recurring revenue, and care IP (Option A)**. Read `welltech-intelligence/PHASE-0-HANDOFF.md` first, then `welltech-intelligence/70-welltech-blueprint/build-roadmap.md` (§2 structure, §4 Phase 0, §5 spend). We have US$500K of WellTech funding (marketing-weighted, gated behind the Phase-1 proof). Start by turning the Phase 0 workstreams into a week-by-week project plan with owners, dependencies, and the lead-time items flagged to start day 1 (incl. **Medimind adding GLP-1 to formulary + obtaining the distributor cost**) — then help me draft the WellTech↔NewCo↔Medimind service-agreement term sheet, the clinic-OS↔NewCo integration spec, the MVP build spec, and the regulatory task list. Commit work to branch `claude/welltech-health-intelligence-5zytb2`.
