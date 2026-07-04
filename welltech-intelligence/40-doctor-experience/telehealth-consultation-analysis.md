# Anatomy of the Malaysian Teleconsultation: Evidence, Doctor Economics and Consult Design

**Abstract.** This document dissects the teleconsultation as a unit of work in Malaysia — what the published evidence says about modality mix, quality and satisfaction; what platform gig work actually pays doctors and why they resent it; the medico-legal anxieties that shape prescriber behaviour (culminating in the MMC's 2025 prohibition on medical certificates from teleconsult-only encounters); and how Malaysian practice compares with global best-practice telemedicine consult design. Headline findings: Malaysian teleconsultation is still predominantly telephone (60.5% of public teleconsult clinics were phone-only), doctor-side barriers are led by medico-legal concerns (cited by 80.6% of surveyed practitioners), platform consumer prices of RM15–30 imply per-consult doctor payouts that undercut the RM40–60/hour locum benchmark, and no Malaysian platform has published doctor-payment rates — an opacity Welltech can exploit by publishing its own. Patient-side demand and market structure are covered in [malaysia-telehealth.md](../10-market-intelligence/malaysia-telehealth.md); this document is doctor-side.

**Last updated: July 2026.**

Related documents: [Doctor workflows](doctor-workflows.md) · [Prescribing models](prescribing-models.md) · [Clinician pain points](clinician-pain-points.md) · [Malaysia regulations](../10-market-intelligence/malaysia-regulations.md) · [Malaysia telehealth](../10-market-intelligence/malaysia-telehealth.md)

---

**Contents:** 1. What a Malaysian teleconsult is (modality, duration) · 2. Published evidence and its limits · 3. Platform gig economics for doctors · 4. Medico-legal anxiety stack and the MC ban · 5. Global best-practice benchmark · 6. Welltech teleconsult blueprint · 7. Bottom line · References

---

## 1. What a Malaysian teleconsult actually is

### 1.1 Modality mix

| Evidence | Finding |
|---|---|
| National census of high-volume public primary-care clinics (n=249, Nov–Dec 2020; JMIR Formative Research 2022) | 45.8% offered teleconsultation; of those, **60.5% telephone-only**, 24.6% phone+video, 14.9% video-only; concentrated in urban clinics; used mainly for diabetes/hypertension follow-up; MOH funding went to video capability while doctors actually used the phone[^1] |
| Private platforms | DoctorOnCall: phone, video and text consults with e-prescription; DOC2US: chat-first ("text a doctor") model; Doctor Anywhere: video-led app; Speedoc: teleconsult sold in ~15-minute blocks from RM30[^2][^3][^4][^5] |
| Hospital telehealth | Adjunct video consults for existing specialist patients (see [telehealth deep dive §5](../10-market-intelligence/malaysia-telehealth.md)) |

*(analyst inference)* The revealed preference of both Malaysian doctors and patients is **asynchronous-capable, low-bandwidth channels** — phone and chat — not scheduled video. This matters for Welltech: WhatsApp-native care is an extension of existing behaviour, not a behaviour change.

### 1.2 Phone vs chat vs video: the trade-off matrix

| Dimension | Telephone | Chat/asynchronous (DOC2US/WhatsApp pattern) | Video |
|---|---|---|---|
| Malaysian adoption | Dominant in public teleconsultation (60.5% of providing clinics phone-only)[^1] | Dominant in private low-cost tier; native to patient behaviour | Funded by MOH, marketed by platforms, used least[^1] |
| Doctor time per encounter | Medium; synchronous but fast | Lowest per message; but encounters fragment across hours | Highest (setup, tech friction, webside expectations) |
| Clinical information yield | Voice cues only | Text + photos + documents; persistent record | Visual inspection possible (rashes, affect, injection technique) |
| Documentation | Must be written separately after call | **The thread is the raw record** — AI-summarisable | Must be written separately |
| Medico-legal posture | Weakest (no artefact of what was said) | Strongest if archived properly; weakest if on personal WhatsApp outside the record[^19] | Intermediate; recording raises consent questions |
| Fit for GLP-1 programme | Escalation channel | **Core channel**: titration check-ins, side-effect triage, adherence nudges | Scheduled checkpoints: initiation follow-up, technique review |

*(analyst assessment built on the modality evidence above)* The chat column wins on five of six dimensions for chronic-programme care — provided the thread is captured into a governed clinical record, which no personal-WhatsApp arrangement achieves today. That capture is precisely what a WhatsApp Business Platform architecture provides (see [WhatsApp healthcare](../10-market-intelligence/malaysia-whatsapp-healthcare.md)).

### 1.2 Duration and throughput

No Malaysian platform publishes consult-duration data. Structural markers: Speedoc's 15-minute billing block; in-person GP consults run <15 minutes at ~40/day (see [doctor-workflows.md §2](doctor-workflows.md)); global telemedicine literature finds unprepared patients inflate visit duration and that pre-visit staff preparation protects clinician time.[^5][^6] *(analyst estimate)* A Malaysian GP teleconsult is realistically 5–12 minutes of doctor time for minor acute presentations, plus unmeasured documentation and follow-up messaging time.

---

## 2. Published Malaysian evidence on quality and satisfaction

| Study | Design/year | Key doctor-relevant finding |
|---|---|---|
| Perception of telemedicine among Malaysian medical practitioners during COVID-19 | Cross-sectional survey; publ. 2021 | Barriers: **medico-legal issues and consent 80.6%**, billing/charges 66.7%, insurance reimbursement 62.5%, technical difficulties 62.5%; recommendations: government engagement, fee standardisation, education[^7][^8] |
| Teleconsultation availability census (public clinics) | n=249 clinics, 2020; JMIR 2022 | Availability ≠ use: video funded, phone used; urban skew[^1] |
| Adoption of virtual care in a Malaysian government hospital | Qualitative, providers; MJPHM | Provider-side barriers and facilitating conditions in public virtual care[^9] |
| Factors influencing telemedicine adoption among Malaysian physicians | Digital Health (SAGE), 2024 | Physician adoption modelling — technology acceptance, facilitating conditions[^10] |
| Patient/physician perceptions of teleconsultation | Qualitative (international/regional), 2022 | Physicians value continuity gains but flag examination limits and workload shift[^11] |
| Patient-side satisfaction and WTP evidence | Multiple studies | Synthesised in [malaysia-telehealth.md §4](../10-market-intelligence/malaysia-telehealth.md): satisfaction decent-not-enthusiastic; WTP RM58–78 sits 2–3× above prevailing prices |

Read-through: the Malaysian evidence base is thin on the doctor's experience — no published study measures teleconsult duration, per-consult pay, documentation time or platform-doctor turnover. Everything doctor-side must be triangulated (as below), and Welltech should treat generating this data internally as proprietary advantage.

### 2.1 How to weigh this evidence base

- **Vintage bias.** The strongest datasets (practitioner perception survey, public-clinic census) collected data in 2020–21 under COVID conditions; doctor attitudes have since been reshaped by two post-pandemic events the studies predate — the OHS Guideline 2025 and the MC ban. Direction of change: medico-legal anxiety validated, commercial optimism reduced. *(analyst assessment)*[^1][^7]
- **Sector bias.** Public-sector clinics are measured; private platform operations are not. The 60.5% phone-only figure describes Klinik Kesihatan practice; private platform modality mix is unpublished and must be inferred from product design (chat-first DOC2US, video-led Doctor Anywhere).[^1][^3][^4]
- **Survivor bias.** Satisfaction studies sample doctors still doing telemedicine; those who tried it and quit — the churn Welltech most needs to understand — appear in no dataset.
- **What this means operationally**: treat published percentages as directional, and treat the absence of doctor-economics data as the market's central information asymmetry — the party that measures it first (Welltech, per §6) prices doctor labour better than every incumbent.

---

## 3. Platform gig economics for doctors

### 3.1 What patients pay vs what doctors can be paid

| Platform | Consumer price (GP consult) | Published doctor payout |
|---|---|---|
| DoctorOnCall | from RM15–19.90 | **Not published**; company states it "pays both doctors and pharmacies for consultations and medicines purchased"[^2][^12] |
| Doctor Anywhere MY | RM25 (promos RM19.80) | **Not published**; provider recruitment page offers "a fixed payout for every completed consultation"[^13] |
| Speedoc | from RM30/15 min | Not published[^5] |
| DOC2US | chat tiers, low-cost/freemium | Not published[^3] |

**The arithmetic doctors do** *(analyst inference, labelled)*: at a RM19.90–25 retail price, after platform margin, payment costs and promos, the plausible doctor payout is **RM10–18 per consult**. A platform doctor must therefore complete 3–4 consults per hour — with no control over demand flow — to match the RM40–60/hour a locum shift pays with certainty, and 5+ consults/hour to match the MOH's own RM80/hour locum allowance benchmark. During off-peak hours with sparse queues, effective hourly earnings fall below CA (clinic assistant) wages. This arithmetic, not technology aversion, is the core reason platform work is treated as marginal income by Malaysian GPs.[^2][^13][^14] (Locum benchmarks: [doctor-workflows.md §4](doctor-workflows.md).)

### 3.2 Entry requirements and onboarding (evidence of the supply bar)

- DoctorOnCall requires MMC registration + current APC and cites partnered doctors having ≥6 years' practice experience; onboarding includes 10–15 supervised training teleconsults with the medical director.[^12][^15]
- Doctor Anywhere recruits GPs, specialists, paediatricians and psychologists for video consults on a per-consultation fixed payout.[^13]
- Government-employed doctors require MOH approval and additional indemnity for private telehealth work — a compliance hurdle platforms largely push onto the doctor (see [regulations §2.1](../10-market-intelligence/malaysia-regulations.md)).

### 3.3 Why doctors churn *(triangulated; no published churn data)*

1. **Pay per unit, risk per encounter**: the payout is transactional but the medico-legal duty (and MMC exposure) is identical to a full consult — an asymmetric trade flagged by 80.6% of practitioners as the top barrier.[^7]
2. **No patient ownership**: the platform owns the relationship and reassigns follow-ups, eliminating the continuity that (per QUALICOPC) drives GP satisfaction more than volume does.[^16]
3. **Queue volatility**: paid only when consults flow; idle time is unpaid.
4. **Post-2025 MC restrictions gutted the core use case**: a large share of B2C demand was MC-seeking; the MMC prohibition (§4) removed it, cutting platform volumes and doctor earnings simultaneously. *(analyst inference from ADHM's own framing of demand drivers)*[^17][^18]

---

### 3.4 The platform-doctor lifecycle *(analyst model)*

Assembling the recruitment, economics and post-2025 regulatory evidence yields a lifecycle every Malaysian platform doctor recognises:

1. **Entry (months 0–2).** Motivated by flexible income around a hospital/clinic job; passes MMC/APC credentialing; completes supervised onboarding consults (DoctorOnCall's 10–15 training calls pattern).[^12][^15]
2. **Honeymoon (months 2–6).** Novelty plus queue access; earnings acceptable during evening peaks; tolerates documentation quirks.
3. **Arithmetic phase (months 6–12).** Doctor computes effective RM/hour across idle time and compares against locum shifts; discovers payout is fixed while the medico-legal duty is full-weight; notices follow-ups route to other doctors.
4. **Disengagement.** Platform work demoted to filler — logged into only when a locum shift falls through; responsiveness drops; platform quality metrics decay.
5. **Exit or dormancy.** No exit event, just silence — which is why churn is invisible in any public dataset.

Interruptions to this decay curve are exactly the levers §5–6 specify: guaranteed-minimum scheduled blocks (kills step 3's volatility discovery), named-panel continuity (kills step 3's ownership grievance), and paid asynchronous bundles (changes the arithmetic itself).

### 3.5 What "good" pays elsewhere: calibration points

- MOH's own price for marginal doctor-hours is **RM80/hour** (2024 locum allowance) — a state-set floor for what an incremental clinical hour is worth in Malaysia.[^30]
- Private locum market clears at **RM40–60/hour** with zero platform risk and guaranteed payment for presence, not throughput.[^31]
- A GLP-1 programme panel restructures the comparison entirely: recurring monthly panel fees per enrolled patient decouple doctor income from queue volatility — the economic design no Malaysian consult-marketplace offers today. *(analyst design point, developed in [clinician-pain-points.md §3](clinician-pain-points.md))*

## 4. The medico-legal anxiety stack

| Anxiety | Substance | Instrument/event |
|---|---|---|
| Misdiagnosis without physical exam | The MMC telemedicine guideline imposes parity of care with in-person practice; the doctor personally carries the gap between what telemedicine can assess and what the standard demands[^19] | MMC Guideline on Telemedicine (2024) |
| MC issuance | **23 September 2025: MMC prohibited MCs after teleconsultation-only encounters** (an MC requires appropriate consultation incl. physical examination). MMA backed the ban — duty of care is "personal, non-transferable and must not be compromised by commercial pressures from employers, insurers or digital health platforms". ADHM warned a blanket ban undermines legitimate care pathways and demanded an evidence-based teleconsultation guideline instead. Doctor Anywhere publicly complied[^17][^18][^20][^21] | MMC notification; MMA/ADHM statements, Nov 2025 |
| Documentation | Teleconsult records live in platform systems the doctor doesn't control; discovery/complaint defence depends on them; chat-based encounters blur the record | MMC guideline record-keeping duties[^19] |
| Consent and identity | Verifying patient identity and obtaining valid consent remotely; OHS 2025 requires patient/practitioner verification at platform level[^19] | OHS Guideline 2025 |
| Prescribing exposure | Off-label GLP-1s, continuation-of-care limits, no psychotropics online (see [prescribing-models.md §4–6](prescribing-models.md)) | Poisons/psychotropic instruments |
| Indemnity | Professional indemnity is an APC prerequisite; whether a doctor's cover extends to platform telemedicine is the doctor's problem to confirm — platforms are silent | Medical Regulations 2017 (see [regulations §2.1](../10-market-intelligence/malaysia-regulations.md)) |

### 4.1 The MC-ban episode as a timeline

| Date | Event | Doctor-side consequence |
|---|---|---|
| 2022 | MMC FAQ position: an MC requires appropriate consultation including physical examination | Largely unenforced; platforms scale digital-MC funnels |
| Feb 2025 | MOH publicly considering digital MCs and e-prescriptions in its digitalisation agenda (see [regulations §3.4](../10-market-intelligence/malaysia-regulations.md)) | Doctors read the direction of travel as permissive |
| 23 Sep 2025 | MMC notification: **no MCs after teleconsultation-only encounters**[^17] | Overnight, a routine platform task becomes a disciplinable act |
| Nov 2025 | MMA backs the ban (duty of care "personal, non-transferable"); ADHM demands an evidence-based teleconsultation guideline instead; Doctor Anywhere announces compliance[^18][^20][^21] | Platforms rewire flows; consult volumes drop; doctors absorb patient anger |

The episode is the defining case study: platforms had built consumer funnels on a service (digital MCs) the regulator then declared unethical overnight, leaving individual doctors holding the professional risk for encounters the platforms had productised. Every Malaysian doctor watching learned the lesson: *the platform's business model is not your safe harbour.*[^17][^18][^20]

### 4.2 Documentation as the quiet burden

Across every modality, the record is the doctor's only defence in an MMC complaint — and Malaysian platform architecture works against the doctor on three counts. First, records live in platform systems the doctor cannot export when they leave the panel. Second, chat consults produce sprawling threads that no one summarises into a clinical note, so the effective record quality is worse than a two-line paper entry. Third, care that migrates to personal WhatsApp after the consult (the standard Malaysian follow-up pattern — see [doctor-workflows.md §7](doctor-workflows.md)) generates clinically material exchanges that never reach any record at all.[^19] International evidence identifies documentation growth as a primary mechanism of telehealth burnout;[^25] in Malaysia the same hours are spent producing records that still fail the doctor medico-legally. AI-drafted structured notes from the full message thread, with doctor sign-off and guaranteed export rights, fix the burden and the exposure in one move. *(analyst assessment)*

**Implications for Welltech.** Welltech's clinical governance must be visibly doctor-protective: published clinical protocols, in-person initiation for GLP-1s, no MC-from-teleconsult ever, platform-paid indemnity top-cover, and a medical director who owns protocol risk. This flips the market's core anxiety into a recruiting message (developed in [clinician-pain-points.md §6](clinician-pain-points.md)).

---

## 5. Global best-practice benchmark: what a well-designed teleconsult looks like

The international literature converges on a three-phase design — preparation, consult, post-consult — with most quality (and most clinician-time savings) created *outside* the live encounter:

1. **Preparation phase.** Delphi consensus criteria for good video consultation practice put structured pre-visit preparation first: appropriateness triage, tech check, agenda-setting, records available.[^22] US multi-centre qualitative work: having staff contact patients pre-visit to reconcile medications and collect history "allows physicians to utilize their valuable time for clinical evaluation, counseling, and patient support" — i.e., intake work should never be done live by the doctor.[^6]
2. **The encounter.** "Webside manner" is a trainable skill set — eye contact via camera, verbalising actions, structured safety-netting; professional environment and freedom from home distractions measurably affect consult quality.[^23][^24]
3. **Post-consult.** Documentation, prescription, follow-up scheduling and asynchronous message handling are where telemedicine silently *adds* clinician workload: increased documentation, poor interoperability and growth in portal/asynchronous messages are the three identified mechanisms by which telehealth worsens burnout.[^25] International cross-sectional data (primary-care physicians, multiple countries): 50% dissatisfied with administrative tasks; digital-health use correlates with workload dissatisfaction; hybrid/remote physicians report somewhat lower burnout than fully in-person peers — telemedicine helps only when the workflow around it is engineered.[^26][^27]
4. **System design.** Systematic reviews find teleconsultation reduces waiting times and unnecessary appointments when embedded in a coordinated pathway, not as a standalone transaction.[^28][^29]

Summary of the global design principles against their Malaysian status:

| Principle (global literature) | Source | Malaysian market status |
|---|---|---|
| Pre-visit preparation is where quality is made | Delphi consensus[^22] | Absent — free-text complaint straight to doctor |
| Intake/med-reconciliation should be staff (or system) work, never live doctor time | Multi-centre qualitative[^6] | Absent — doctor does intake inside the paid minutes |
| Webside manner is a trainable competency, not a personality trait | Webside-manner guidance[^23] | Ad hoc — limited onboarding beyond credential checks |
| Environment and distraction control materially affect consult quality | Systematic review[^24] | Unmanaged on both sides (doctor moonlighting from home; patient in public/family settings) |
| Documentation/async load must be engineered down or it becomes the burnout vector | Burnout mechanism literature[^25][^26] | Unengineered — doctors type own notes; async unpaid |
| Telemedicine embedded in coordinated pathways beats standalone transactions | Systematic reviews[^28][^29] | Standalone-transaction model dominates B2C |

### 5.1 Malaysian practice vs the benchmark

| Best-practice element | Malaysian platform norm (2026) | Gap |
|---|---|---|
| Staff/AI pre-visit intake | Minimal; patient types free-text complaint | Doctor does intake live, unpaid |
| Appropriateness triage before booking | Weak; MC-seeking demand dominated B2C | Post-MC-ban, triage is now existential |
| Named-doctor continuity | None — next-available routing | Kills follow-up quality and doctor satisfaction |
| Structured documentation support | Doctor types own notes in platform CMS | Documentation burden on lowest-paid minutes |
| Post-consult monitoring | Patient-initiated only | Chronic/GLP-1 care impossible without it |
| Fee for asynchronous care | No construct anywhere in market | Unpaid WhatsApp work (see [doctor-workflows.md §7](doctor-workflows.md)) |

**Implications for Welltech.** The teleconsult Welltech sells doctors should be: AI-prepared (structured intake, vitals/labs surfaced, draft note pre-written), 10–15 protected minutes, named-panel continuity, zero live administrative typing, paid asynchronous follow-up bundles, and hard triage rules that keep out encounters telemedicine cannot ethically serve. Every element is directly responsive to a documented failure of the incumbent model — and to the global evidence on what makes teleconsultation work.

## 6. The Welltech teleconsult blueprint

Synthesising §1–§5 into an operating specification *(analyst design; pilot-validate)*:

**Stage 0 — Triage gate (AI, WhatsApp).**
- Structured symptom intake; hard exclusions routed out immediately (emergencies → ED guidance; MC requests → in-person clinic booking, never teleconsult; psychotropic requests → declined per [prescribing-models.md §6](prescribing-models.md)).
- Identity verification and consent per OHS 2025 expectations; PDPA notices delivered in-channel.[^19]

**Stage 1 — Preparation (AI + ops, before doctor sees anything).**
- History structured into a one-screen pre-read: complaint, red-flag screen, medication list, prior Welltech encounters, relevant labs/vitals from the programme record.
- Delphi-consensus preparation criteria (appropriateness, tech check, agenda) executed by the system, not the doctor.[^22]
- Booking into a protected 10–15-minute slot with the patient's **named panel doctor**; chat-first by default, voice/video escalation one tap away.

**Stage 2 — The encounter (doctor).**
- Doctor opens with the pre-read already absorbed — the first minute is clinical, not clerical.
- Webside-manner standards trained at onboarding (verbalised examination substitutes, structured safety-netting language).[^23]
- Prescribing decisions inside protocol rails; anything off-protocol flags to the medical director asynchronously.

**Stage 3 — Post-consult (AI, doctor signs).**
- Draft SOAP note generated from the full thread within seconds; doctor edits/signs; note is exportable by the doctor permanently.
- Prescription issued via the digitally signed e-Rx rail ([prescribing-models.md §3](prescribing-models.md)); fulfilment tracked in-channel.
- Follow-up plan instantiated as scheduled WhatsApp touchpoints; asynchronous questions between touchpoints answered by AI within protocol, batched to the doctor otherwise — and the batching time is paid.

**Stage 4 — Measurement.**
- Per-encounter metrics: preparation completeness, consult duration, note turnaround, escalation rate, patient-reported resolution.
- Per-doctor metrics: effective RM/clinical hour, message load, after-hours touches — reviewed monthly as clinical-safety indicators (targets in [clinician-pain-points.md §4](clinician-pain-points.md)).

This blueprint prices the doctor's synchronous time correctly, converts asynchronous care from unpaid leakage into a compensated product, and produces — as a by-product — the consult-duration, satisfaction and churn dataset that the Malaysian literature currently lacks (§2). Publishing selected metrics would simultaneously build regulator trust (ADHM's demanded "evidence-based teleconsultation guideline" needs exactly this evidence[^18]) and set a recruiting benchmark competitors cannot match without re-architecting.

## 7. Bottom line

Three facts organise everything above:

1. **The Malaysian teleconsult, as currently sold, is a phone call or chat priced at RM15–30 with the doctor's payout undisclosed and their medico-legal exposure undiminished** — a product doctors serve reluctantly and regulators have begun to prune (the MC ban being the first cut).[^1][^7][^17]
2. **Everything the global literature says makes teleconsultation work — preparation, continuity, engineered documentation, pathway embedding — is absent from the Malaysian incumbent model.**[^6][^22][^25]
3. **Therefore the consult itself is the open competitive surface.** Not price, not app features: the redesign of the encounter around the doctor's prepared, protected, paid time. The operator that treats the teleconsult as a manufactured product with quality specifications — rather than a marketplace transaction — takes the doctors, and the doctors bring the patients.

Doctor-side economics are benchmarked in [doctor-workflows.md](doctor-workflows.md); prescribing rails in [prescribing-models.md](prescribing-models.md); the full recruiting synthesis in [clinician-pain-points.md](clinician-pain-points.md).

---

## References

[^1]: Lee W.L. et al., "Assessing the Availability of Teleconsultation and the Extent of Its Use in Malaysian Public Primary Care Clinics: Cross-sectional Study", JMIR Formative Research 6(5):e34485 (2022), https://formative.jmir.org/2022/5/e34485 (accessed July 2026).
[^2]: CodeBlue, "Getting Doctors' Consultations, Medicine Without Leaving Home In A Pandemic" (Dec 2020; DoctorOnCall model, GP consults from RM15, pays doctors and pharmacies), https://codeblue.galencentre.org/2020/12/getting-doctors-consultations-medicine-without-leaving-home-in-a-pandemic/ (accessed July 2026).
[^3]: DOC2US (chat-first telemedicine and e-prescription), https://www.doc2us.com/newsroom/doc2us---the-first-to-launch-digital-signature-enhanced-e-prescription-in-malaysia (accessed July 2026).
[^4]: Doctor Anywhere Malaysia, https://www.doctoranywhere.my/ (accessed July 2026).
[^5]: Speedoc Malaysia, "Telemedicine — Online Doctors" (teleconsult from RM30), https://my.speedoc.com/en/services/telemedicine-online-doctors (accessed July 2026).
[^6]: "Patient and Provider Recommendations for Improved Telemedicine User Experience in Primary Care: A Multi-Center Qualitative Study", J Gen Intern Med / PMC (2023), https://pmc.ncbi.nlm.nih.gov/articles/PMC10027343/ (accessed July 2026).
[^7]: "Perception of telemedicine among medical practitioners in Malaysia during COVID-19", Medicine/PMC (2021) — barriers: medico-legal 80.6%, billing 66.7%, insurance 62.5%, technical 62.5%, https://pmc.ncbi.nlm.nih.gov/articles/PMC8485382/ (accessed July 2026).
[^8]: Same study, PubMed record, https://pubmed.ncbi.nlm.nih.gov/34621369/ (accessed July 2026).
[^9]: "Adoption of Virtual Care in a Malaysian Government Hospital: A Qualitative Study of Healthcare Providers' Perceptions, Barriers, and Facilitating Conditions", Malaysian Journal of Public Health Medicine, https://mjphm.org/index.php/mjphm/article/view/3570 (accessed July 2026).
[^10]: Tan S.H., Wong C.K., Yap Y.Y., Tan S.K., "Factors influencing telemedicine adoption among physicians in the Malaysian healthcare system: A revisit", Digital Health 10 (2024), https://journals.sagepub.com/doi/full/10.1177/20552076241257050 (accessed July 2026).
[^11]: "Teleconsultations and their implications for health care: A qualitative study on patients' and physicians' perceptions", International Journal of Medical Informatics (2022), https://www.sciencedirect.com/science/article/pii/S138650562200065X (accessed July 2026).
[^12]: DoctorOnCall — Wikipedia (founding, model, doctor network >200 GPs/specialists, payment to doctors and pharmacies), https://en.wikipedia.org/wiki/DoctorOnCall (accessed July 2026).
[^13]: Doctor Anywhere, "Doctors and Specialists: We want you" (fixed payout per completed consultation), https://doctoranywhere.com/doctor-application/ (accessed July 2026).
[^14]: Lowyat forum, "DoctorOnCall" thread (consumer/doctor discussion of platform model and pricing), https://forum.lowyat.net/topic/4002288/all (accessed July 2026).
[^15]: DoctorOnCall Help Centre and platform documentation (doctor credentialing: MMC registration, APC, experience, supervised training calls), https://help.doctoroncall.com.my/faq/are-consultation-fees-and-healthcare-packages-subject-to-service-tax-sst/ and https://www.doctoroncall.com.my/find-doctor (accessed July 2026).
[^16]: Ab Majid H. et al., "Job satisfaction of public and private primary care physicians in Malaysia: analysis of findings from QUALICO-PC", Human Resources for Health 17:82 (2019), https://human-resources-health.biomedcentral.com/articles/10.1186/s12960-019-0410-4 (accessed July 2026).
[^17]: CodeBlue, "MMC Bans Medical Sick Certs Issued After Teleconsults" (Nov 2025), https://codeblue.galencentre.org/2025/11/mmc-bans-medical-sick-certs-issued-after-teleconsults/ (accessed July 2026).
[^18]: CodeBlue, "Develop Teleconsultation Guideline, Not Ban Digital MCs — Association Of Digital Health Malaysia" (Nov 2025), https://codeblue.galencentre.org/2025/11/develop-teleconsultation-guideline-not-ban-digital-mcs-association-of-digital-health-malaysia/ (accessed July 2026).
[^19]: MMC Guideline on Telemedicine and OHS Guideline 2025 — primary-source analysis in [malaysia-regulations.md](../10-market-intelligence/malaysia-regulations.md), §3.
[^20]: CodeBlue, "Ban On Digital MCs Shows MMC's Stance On Duty Of Care — MMA" (Nov 2025), https://codeblue.galencentre.org/2025/11/ban-on-digital-mcs-shows-mmcs-stance-on-duty-of-care-mma/ (accessed July 2026); Bernama, "MC Through Teleconsultation: Ethics, Patient Safety Must Remain At Core — MMA", https://bernama.com/en/news.php?id=2494172 (accessed July 2026).
[^21]: Doctor Anywhere Malaysia (LinkedIn), compliance statement on the MMC directive on teleconsultation MCs, https://www.linkedin.com/posts/doctor-anywhere-malaysia_in-response-to-the-malaysian-medical-council-activity-7397134399219298305-jNAS (accessed July 2026).
[^22]: "Consensus on Criteria for Good Practices in Video Consultation: A Delphi Study", Int J Environ Res Public Health / PMC (2020), https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7432677/ (accessed July 2026).
[^23]: "Conducting a Professional Telemedicine Visit Using High-Quality Webside Manner", PMC (2021), https://pmc.ncbi.nlm.nih.gov/articles/PMC8785697/ (accessed July 2026).
[^24]: Almathami H.K.Y. et al., "Barriers and Facilitators That Influence Telemedicine-Based, Real-Time, Online Consultation at Patients' Homes: Systematic Literature Review", J Med Internet Res 22(2):e16407 (2020), https://www.jmir.org/2020/2/e16407/ (accessed July 2026).
[^25]: Rutgers NJ State Policy Lab, "Telehealth May Worsen Physician Burnout: How to Avoid It" (documentation, interoperability, asynchronous-message mechanisms), https://policylab.rutgers.edu/publication/telehealth-may-worsen-physician-burnout-how-to-avoid-it/ (accessed July 2026).
[^26]: "Primary care physician digital health profile and burnout: an international cross-sectional study", European Journal of Public Health 35(6) (2025), https://academic.oup.com/eurpub/article/35/6/1162/8203018 (accessed July 2026).
[^27]: Residency Advisor, "Remote Work and Physician Burnout: What Telehealth Surveys Actually Report" (hybrid/remote vs in-person burnout ranges), https://residencyadvisor.com/resources/telemedicine-careers/remote-work-and-physician-burnout-what-telehealth-surveys-actually-report (accessed July 2026).
[^28]: "Review of Systematic Reviews in the Field of Telemedicine", PMC (2022), https://pmc.ncbi.nlm.nih.gov/articles/PMC9391764/ (accessed July 2026).
[^29]: "Telemedicine for healthcare: Capabilities, features, barriers, and applications", Sensors International / PMC (2021), https://pmc.ncbi.nlm.nih.gov/articles/PMC8590973/ (accessed July 2026).
[^30]: Malay Mail, "Health minister says doctors working overtime to get locum allowance immediately, at RM80 an hour" (Feb 2024), https://www.malaymail.com/news/malaysia/2024/02/23/health-minister-says-doctors-working-overtime-to-get-locum-allowance-immediately-at-rm80-an-hour/119618 (accessed July 2026).
[^31]: LocumLah (RM40–50/hour listings), https://portal.locumlah.com/ ; Malaysian Medical Resources, "Calling all doctors and nurses – get Locum Apps now!" (RM40/hour floor), https://new.medicine.com.my/2020/05/calling-all-doctors-and-nurses-locumapps/ (accessed July 2026).
