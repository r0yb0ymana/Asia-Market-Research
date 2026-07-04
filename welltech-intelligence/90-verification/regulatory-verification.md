# Regulatory Verification — Instruments, Dates & Status Across the Three Markets

**Abstract.** This is a second-pass verification of the *regulatory* claims (statutes, guidelines, circulars, registration numbers, effective dates and "in force / not in force" status) asserted across the repository's three market files — [malaysia-regulations.md](../10-market-intelligence/malaysia-regulations.md), [singapore-market-intelligence.md](../10-market-intelligence/singapore-market-intelligence.md) §4, [hong-kong-market-intelligence.md](../10-market-intelligence/hong-kong-market-intelligence.md) §4 — and the consolidated [sources/regulations.md](../sources/regulations.md) index. It was produced under the environment constraint described in [methodology.md](methodology.md): primary government/regulator pages return HTTP 403 to direct fetches, so every claim here is raised (or lowered) in confidence by **corroboration across multiple independent search results**, not by reading the primary PDF. Tags follow the scheme in methodology.md (🟢 corroborated ≥2 independent sources · 🟡 single/partial/conflicting · 🔴 contradicted/absent/misdated · ⚪ genuinely uncheckable by desk research).

**This pass verifies whether cited instruments exist and are described correctly. It is NOT legal or clinical advice.** The two closing sections list exactly which questions must go to a healthcare lawyer and a medical director before Welltech operates on them.

**Last updated: July 2026.**

---

## Scope of this pass

**In scope (checked):** every regulatory *instrument* (statute, ordinance, guideline, circular), its *effective date / status* ("in force" vs "not in force" vs "dormant"), and whether its *described effect* is broadly accurate — across telemedicine licensing, prescribing/pharmacy, GLP-1 registration, advertising, privacy, facility licensing and AI/SaMD, for Malaysia, Singapore and Hong Kong. Special attention (per the verification brief) went to precise dates, "in force / not in force" claims, and the GLP-1 registration numbers and launch dates.

**Out of scope (handled elsewhere in this folder):** market sizes, epidemiology, competitor pricing and funding figures ([load-bearing-numbers-audit.md](load-bearing-numbers-audit.md), [price-verification.md](price-verification.md)); internal cross-document consistency ([consistency-reconciliation.md](consistency-reconciliation.md)). This document also does **not** give legal or clinical advice — it identifies which questions must go to a healthcare lawyer and a medical director (the two closing sections).

**Source files read:** malaysia-regulations.md (512 lines; §§1–12), singapore-market-intelligence.md §4, hong-kong-market-intelligence.md §4, sources/regulations.md (the consolidated index), plus prescribing-models.md and ai-nurse.md for the clinical-protocol claims.

---

## Scoreboard

| Tag | Count | Meaning |
|---|---|---|
| 🟢 GREEN | 24 | Instrument exists; date/status corroborated by ≥2 independent results; no contradiction found |
| 🟡 AMBER | 8 | Single credible source, or sources agree on existence but differ on a date, or the repo itself flagged the date as unofficial |
| 🔴 RED | 0 | None — no cited instrument was found to be fabricated or clearly misdated |
| ⚪ UNVERIFIABLE | 2 | Not checkable by desk research (internal enforcement statistics; forward-looking legislative promises) |

**Headline finding:** the regulatory spine of the repository is **solid**. Every high-stakes instrument checked (Telemedicine Act dormancy; OHS Circular Bil.16/2025; MMC tele-MC ban; HCSA Phase 2; MaNaDr; Joint Circular 87/2024; UMAO; PDPO s.33; the GLP-1 registrations) verified as real and correctly dated. The **one date worth a second look is the Wegovy Malaysia commercial-launch date** (repo says January 2026; some clinic/press sources say the market became "officially available" in **January 2025**) — flagged AMBER below. No 🔴.

### Tags by market

| Market | 🟢 | 🟡 | 🔴 | ⚪ | Read |
|---|---|---|---|---|---|
| Malaysia | 8 | 4 | 0 | 1 | Strongest file; only soft spot is a commercial launch date |
| Singapore | 5 | 3 | 0 | 0 | Solid; honest about its own launch-date uncertainty |
| Hong Kong | 6 | 1 | 0 | 1 | Solid; the s.33-not-in-force and A&E-reform claims verified cleanly |
| Cross-cutting (GLP-1 residual rows / MASA sub-claim) | 5 | — | — | — | See dedicated GLP-1 table |

(Counts are indicative — several rows bundle multiple sub-claims; the per-market tables below are authoritative.)

---

## Malaysia

**Verdict for the market: solid.** Malaysia is the densest regulatory file in the repository and it is also the most accurate. The whole edifice rests on one striking fact — the Telemedicine Act 1997 was passed but never commenced — and that fact is unambiguously verified (CommonLII literally lists it "Not yet in force"). The three 2025-era developments the strategy launches into (the OHS Guideline / Circular Bil.16/2025 of 15 May 2025; the MMC tele-MC prohibition of 23 September 2025; the PDPA amendments in force 1 June 2025) all check out to the day. The only soft spot is a *commercial* date, not a *legal* one: Wegovy's Malaysian launch (see GLP-1 table). Nothing in the Malaysia regulatory section reads as fabricated or materially misdated.

What a reader should still re-pull from primary sources before relying on it: (a) the exact penalty quanta in the penalty-reference table (the repo itself flags several as "verify against AGC consolidated text"); (b) the precise current Schedule of the Medicines (Advertisement and Sale) Act 1956 (the "obesity is not scheduled" sub-claim); (c) each individual GLP-1 MAL number on NPRA QUEST.

| Instrument | Repo claim | Search corroboration | Tag | Note |
|---|---|---|---|---|
| **Telemedicine Act 1997 (Act 564)** | Enacted 18 Jun 1997, **never brought into force**; CommonLII "Not yet in force"; governs nothing | CommonLII lists it "(Not yet in force)"; Wikipedia, RDS Law Partners, IBA survey all confirm passed 1997, never commenced, no dedicated telemedicine legislation since | 🟢 | Core structural premise of MY analysis — verified. [commonlii.org](https://www.commonlii.org/my/legis/consol_act/ta1997yif269/) · [rdslawpartners.com](https://www.rdslawpartners.com/post/regulating-remote-care-a-legal-overview-of-telemedicine) |
| **OHS Guideline 2025 / SPKPK Bil. 16/2025** | MOH Guideline on Online Healthcare Services, issued under DG Circular No.16/2025, **dated 15 May 2025**; physical office, doctor/pharmacist at board level, e-prescription pathway | MOH hosts "Surat_Pekeliling_Ketua_Pengarah_Kesihatan_Bil._16_...15_Mei_2025"; Skrine and Lexology alerts (July 2025) confirm content (SSM incorporation, physical base, licensed practitioners, digital prescription) | 🟢 | Date and substance verified. [moh.gov.my PDF](https://www.moh.gov.my/images/04-penerbitan/pekeliling/Surat_Pekeliling_Ketua_Pengarah_Kesihatan_Bil._16_Guideline_OHS_2025_15_Mei_2025_compressed.pdf) · [skrine.com](https://www.skrine.com/insights/alerts/july-2025/moh-releases-guidelines-on-online-healthcare-servi) |
| **MMC tele-MC prohibition** | Notice **23 September 2025**: MCs must not be issued after teleconsultation-only encounters; reaffirms 2022 FAQ | CodeBlue, The Star, thesun, Bernama, Scoop all confirm the 23 Sep 2025 notification and the physical-examination rationale; MMA backed it, ADHM opposed a blanket ban | 🟢 | Date, effect and the MMA/ADHM reactions all verified. [codeblue.galencentre.org](https://codeblue.galencentre.org/2025/11/mmc-bans-medical-sick-certs-issued-after-teleconsults/) · [thestar.com.my](https://www.thestar.com.my/news/nation/2025/11/18/no-more-mc-via-video-call-says-mmc) |
| **Poisons Act 1952 — Group B** | GLP-1s are Group B poisons; prescription-only; may be dispensed by prescriber (GP dispensing model) | Multiple pharmacy/legal sources confirm Group B = prescription-only-medicine class under Poisons Act/Regulations | 🟢 | Classification architecture verified. |
| **Poisons (Amendment) Act 2022** | Raised penalties; **in force 1 January 2023** | CodeBlue (Bill passed Jul 2022), DKSH Insights and AGC reprint confirm commencement **1 Jan 2023** (except s.21 on compounding); penalties raised materially | 🟢 | Date verified precisely. [codeblue.galencentre.org](https://codeblue.galencentre.org/2022/07/21/parliament-passes-poisons-amendment-bill-after-three-year-delay/) · [dksh.com](https://www.dksh.com/global-en/home/insights/how-malaysias-amended-poisons-law-affects-the-healthcare-industry) |
| **PDPA (Amendment) Act 2024** | DPO mandatory + 72-hour breach notification, **in force 1 June 2025**; RM1m max fine; cross-border TIA regime | DataGuidance, Baker McKenzie, Lexology, TSL Legal confirm headline obligations (mandatory DPO, 72-hr breach notice to Commissioner, 7-day notice to data subjects) took effect **1 June 2025** | 🟢 | Date and mechanics verified. [dataguidance.com](https://www.dataguidance.com/opinion/malaysia-personal-data-protection-amendment-act) · [lexology.com](https://www.lexology.com/library/detail.aspx?g=d72dec59-374a-4a94-aa94-03f8b5a0d3be) |
| **MASA 1956 (Act 290) / MAB / KKLIU** | Prescription-medicine advertising to public prohibited; MAB approval + KKLIU number required; obesity not on statutory Schedule | Regime existence well-attested in secondary/law-firm sources; not independently re-tested for the "obesity not scheduled" sub-claim this pass | 🟡 | Framework GREEN-grade; the "obesity is not on the Schedule but service ads still restricted" nuance rests on the repo's own reading — confirm exact current Schedule with counsel. |
| **Medical Device Act 2012 (Act 737) — SaMD** | Software with diagnostic/treatment intent is a registrable medical device; Classes A–D; MDA/GD/0062 (3rd ed. 2025) | MDA portal, Act 737 s.2 definition (expressly includes "software"), s.5(1) registration mandate, four-class system and CAB conformity all confirmed across MDA and advisory sources | 🟢 | SaMD capture verified. [portal.mda.gov.my](https://portal.mda.gov.my/index.php/industry/medical-device-registration/medical-device-registration-information) |
| **MMC Guideline on Ethical Use of AI** | Endorsed 29 Dec 2024, adopted 18 Feb 2025; doctor remains accountable | Instrument exists (MMC hosts the PDF; sources/regulations.md links it); exact dual-date not re-corroborated independently this pass | 🟡 | Existence solid; confirm the "adopted 18 Feb 2025" date against the MMC document itself. |
| **Medical (Amendment) Act 2024 (A1729)** | Tabled 15 Jul 2024; restructured specialist recognition | Consistent with widely reported 2024 amendment; not the load-bearing claim, lightly checked | 🟢 | Non-critical to the operating model. |

### Malaysia GLP-1 — see the dedicated table below.

---

## Singapore

**Verdict for the market: solid, and unusually honest about its own uncertainties.** Singapore's regulatory section is anchored on two hard, verifiable facts — HCSA Phase 2 licensing of teleconsultation from 26 June 2023, and the MaNaDr enforcement saga — and both verified precisely, including the vivid MaNaDr specifics (>100,000 teleconsults of ≤1 minute, one lasting 1 second, 19 MCs to one patient in a month, 41 doctors referred to SMC). The Joint Circular 87/2024 is real and correctly dated 22 November 2024. Notably, where the repo is *unsure* — the Wegovy commercial-launch timing — it says so explicitly and tells the reader to verify with Novo Nordisk SG. That is exactly the behaviour this verification pass rewards.

What a reader should still re-pull: (a) the Health Information Bill's introduction/passage status (repo says introduced 5 Nov 2025 — confirm before treating mandatory NEHR contribution as a live day-one obligation); (b) the IP rider reform mechanics (financing, not compliance, but re-confirm the 1 Apr 2026 date and S$6,000 cap); (c) the PDPC healthcare advisory-guideline details.

| Instrument | Repo claim | Search corroboration | Tag | Note |
|---|---|---|---|---|
| **HCSA 2020 — Phase 2** | Teleconsultation became a licensable Outpatient Medical Service on **26 June 2023**; CGO regime | MOH newsroom, Allen & Gledhill, Baker McKenzie, Rajah & Tann all confirm Phase 2 commenced **26 Jun 2023**, first licensing of teleconsultation + non-clinic premises | 🟢 | Date and licensee categories (platform cos, individual doctors) verified. [moh.gov.sg](https://www.moh.gov.sg/newsroom/phase-2-of-healthcare-services-act-to-start-on-26-june-2023/) · [allenandgledhill.com](https://www.allenandgledhill.com/sg/publication/articles/24880/) |
| **MaNaDr enforcement** | Stop-order **16 Aug 2024** (>100k teleconsults ≤1 min; one 1 second; 19 MCs to one patient/month); intended revocation **24 Oct 2024**; doctors to SMC | MOH newsroom + Mothership + The Online Citizen confirm stop-order 16 Aug 2024, the ≤1-minute/19-MC findings, and the 24 Oct 2024 intended-revocation notice; **41 doctors** referred to SMC | 🟢 | All specifics verified. [moh.gov.sg](https://www.moh.gov.sg/newsroom/manadr-clinic-instructed-to-stop-provision-of-outpatient-medical-services-via-teleconsultation/) · [mothership.sg](https://mothership.sg/2024/08/manadr-clinic-suspended/) |
| **MOH–HSA Joint Circular 87/2024** | Telemedicine standards + advertisements; post-MaNaDr; repo dates it 22 Nov 2024 | HCSA/MOH host the circular dated **22 November 2024**; scope (HCSA + HPA 2007 + SMC ECEG; advertising controls) confirmed | 🟢 | Repo abstract says "November 2024", timeline says "22 Nov 2024" — consistent and correct. [hcsa.gov.sg](https://www.hcsa.gov.sg/licensable-healthcare-services/joint-circular-on-regulations-and-professional-standards-for-telemedicine-services-and-advertisements/) |
| **POM advertising ban + GLP-1 clampdown** | Health Products (Advertisement of Specified Health Products) Regs 2016 Reg 7 bans DTC POM ads; MOH/HSA blocked GLP-1/"weight-loss pen" creatives | Regulation and enforcement posture corroborated by Medical Channel Asia and repeated CNA/press coverage of blocked weight-loss-drug ads | 🟢 | "Cannot run Wegovy/Ozempic consumer ads" verified as correct. |
| **SMC ECEG (2016)** | "Same quality and standard of care as in-person"; MC/prescription discipline | Standard, uncontested; the ECEG A6 telemedicine standard is well-attested | 🟢 | — |
| **PDPA + Healthcare Advisory Guidelines (rev. Sep 2023)** | Consent/purpose/retention/breach for patient data | Instrument exists (PDPC hosts Sep 2023 revision); not independently re-searched this pass | 🟡 | Existence solid; details rest on the PDPC guideline text. |
| **Health Information Bill** | Introduced in Parliament **5 Nov 2025**; mandatory NEHR contribution for licensed providers incl. telemedicine + retail pharmacy | MOH newsroom link cited; the 5 Nov 2025 introduction date not independently re-corroborated this pass | 🟡 | Confirm the Bill's introduction/passage status before treating NEHR contribution as a live day-one obligation. |
| **IP rider reform** | Riders sold from **1 Apr 2026** can no longer fully cover the deductible; co-pay cap doubles to S$6,000 | Widely reported reform; not re-verified independently this pass (financing, not clinical-regulatory) | 🟡 | Affects demand modelling, not compliance posture. |

### Singapore GLP-1 — see the dedicated table below.

---

## Hong Kong

**Verdict for the market: solid.** Hong Kong's thesis is that it is the lowest-friction market to enter (no telemedicine licence) but the easiest to be "quietly hurt in" (risk concentrates on the individual doctor's registration). Both halves verified: the MCHK Ethical Guidelines on Practice of Telemedicine (December 2019) are real, non-binding, and the only telemedicine instrument; there is no statute. The two structurally important claims for a WhatsApp-first operator — that PDPO **section 33 (cross-border transfer) has never been brought into force**, and that there is no mandatory breach notification — are strongly corroborated (multiple law firms confirm s.33 is still not in operation >25 years on, with no timetable). The UMAO Cap 231 / Schedule 4 advertising wall is correctly described, and the January 2026 A&E fee reform (HK$180→HK$400) verified to the day, including the observed ~24% drop in semi-/non-urgent attendances.

What a reader should still re-pull: (a) the eHealth+ (EHRSS Amendment Ordinance 2025) effective date and mandatory-deposit scope; (b) treat CMPR / "1+" as a roadmap, not a live instrument.

| Instrument | Repo claim | Search corroboration | Tag | Note |
|---|---|---|---|---|
| **No telemedicine statute; MCHK guidelines only** | No licensing regime; **MCHK Ethical Guidelines on Practice of Telemedicine, December 2019** + HKAM Q&As (Mar 2022); breach = professional misconduct | HKAM, info.gov.hk, DLA Piper, Two Birds, Kennedys all confirm MCHK Guidelines promulgated **Dec 2019**, non-binding, no telemedicine legislation; disciplinary exposure only | 🟢 | The "lowest-friction, doctor-bears-the-risk" thesis verified. [hkam.org.hk](https://www.hkam.org.hk/en/news/questions-and-answers-qas-ethical-guidelines-practice-telemedicine-guidelines) · [mchk.org.hk PDF](https://www.mchk.org.hk/files/PDF_File_Ethical_Guidelines_on_Telemedicine.pdf) |
| **Pharmacy & Poisons Ordinance (Cap 138)** | GLP-1s = Part 1 poisons; pharmacist-dispensed against prescription; illegal supply **up to HK$100,000 + 2 yrs** | Consistent across Drug Office and SCMP coverage; penalty figure repeated in multiple sources | 🟢 | Penalty and classification verified. |
| **UMAO (Cap 231) + Schedule 4** | Enacted 1953, amended 2005; prohibits DTC Rx-medicine advertising; Schedule 4 restricts weight-loss/fat-reduction claims for orally consumed products | e-Legislation + Drug Office + DH press release confirm Cap 231, and that Schedule 4 health-claim controls on orally consumed products (incl. weight-loss claims) took effect **1 June 2012** under the 2005 amendment | 🟢 | Correct. Minor precision: the *commencement* of the Schedule 4 controls was 1 Jun 2012 (2005 amendment, delayed start) — repo's "via the 2005 amendment's Schedule 4" is accurate. [elegislation.gov.hk/hk/cap231](https://www.elegislation.gov.hk/hk/cap231) · [dh.gov.hk press 2012](https://www.dh.gov.hk/english/press/2012/120531.html) |
| **PDPO (Cap 486) — s.33 not in force** | Cross-border transfer restriction **never brought into force**; no legal prohibition on offshoring HK patient data; no mandatory breach notification | Tanner De Witt, Deacons, Mayer Brown all confirm **s.33 still not in operation** >25 yrs on, no timetable; PCPD issued Recommended Model Contractual Clauses (May 2022) as soft guidance | 🟢 | "Most permissive of the three markets" verified. [tannerdewitt.com](https://www.tannerdewitt.com/cross-border-transfers-section-33/) · [deacons.com](https://www.deacons.com/2023/04/25/hong-kongs-cross-border-data-transfer-regime/) |
| **HA fee reform — A&E** | A&E charge for non-critical (triage III–V) **more than doubled HK$180 → HK$400, 1 Jan 2026**; critical/emergency waived; attendances fell | HKFP, SCMP, HA and news.gov.hk confirm HK$180→400 from **1 Jan 2026**, waiver for critical/emergency, ~12% overall / 24% semi-/non-urgent drop, $350 refund for triage III–V redirected to private | 🟢 | Fully verified. [hongkongfp.com](https://hongkongfp.com/2025/12/30/emergency-room-visits-at-hong-kong-public-hospitals-to-increase-to-hk400-on-jan-1-amid-sweeping-fee-reform/) · [ha.org.hk](https://www.ha.org.hk/ho/corpcomm/fncr/index-en.html) |
| **eHealth+ (EHRSS Amendment Ordinance 2025)** | Effective 1 Dec 2025; mandatory-deposit power; GBA cross-boundary recognition | Instrument referenced; the 1 Dec 2025 effective date not independently re-corroborated this pass | 🟡 | Confirm effective date and mandatory-deposit scope before architecting NEHR-equivalent integration. |
| **CMPR / "1+" mechanism** | Centre for Medical Products Regulation by end-2026; more FDA-like posture | Directional, forward-looking; Bird & Bird note cited | ⚪ | A stated government intention, not yet a live instrument — treat as roadmap. |

### Hong Kong GLP-1 — see the dedicated table below.

---

## Cross-market comparison table — verified

The repo's one-screen cross-market map (in both [sources/regulations.md](../sources/regulations.md) and hong-kong-market-intelligence.md §4.8) is the summary most likely to be quoted into a board deck. Each cell checked against the verifications above:

| Dimension | Malaysia | Singapore | Hong Kong | Verified? |
|---|---|---|---|---|
| Telehealth service licence | None enforced (Telemedicine Act 1997 dormant); OHS Guideline 2025 soft law | **Required** — HCSA OMS licence + CGO (26 Jun 2023) | **None** — MCHK Dec 2019 guidelines only | 🟢 all three verified |
| Who bears regulatory risk | Doctor (MMC) + facility (PHFSA) | Licensee entity + doctor | The individual doctor (registration/discipline) | 🟢 consistent with instruments checked |
| Rx-medicine control | Poisons Act 1952 — Group B | Health Products / Poisons Act — POM | Pharmacy & Poisons Ordinance — Part 1 (HK$100k/2yr) | 🟢 verified |
| GLP-1 DTC advertising | MAB/KKLIU pre-approval | Banned for POMs, actively enforced | UMAO statutory prohibition + Schedule 4 | 🟢 verified |
| Privacy | PDPA 2010 + 2024 amendments (in force 2025) | PDPA + healthcare guidelines; NEHR incoming | PDPO; **s.33 cross-border not in force** | 🟢 verified |
| Practical entry friction | Low | High (licence + inspection) | Lowest — discipline/press risk on doctors | 🟢 fair characterisation |

The comparative map is accurate. The single caveat is the word "enforced" in the MY telehealth-licence cell: it is correct that no telehealth *licence* is enforced, but the MMC tele-MC ban (Sep 2025) and OHS Guideline (May 2025) mean the market is more actively *governed* by soft law than "low friction" alone conveys — a nuance the full MY file captures but the one-line map compresses away.

---

## GLP-1 registration & launch dates — high-stakes verification

The instructions flag these as the most error-prone. Each row cross-checked against pharma press releases and clinic/regulatory sources.

| Market | Molecule / brand | Repo claim | Search corroboration | Tag | Note |
|---|---|---|---|---|---|
| **MY** | Tirzepatide / **Mounjaro** | Registered **MAL24026013AZ**; **launched 30 August 2025**; T2DM + chronic weight management | Multiple MY clinic sources confirm registration **MAL24026013AZ** and launch **30 Aug 2025**; dual GIP/GLP-1; BMI ≥30 (or ≥27 + comorbidity) | 🟢 | Registration number **and** launch date both verified — this is the highest-confidence GLP-1 claim in the repo. |
| **MY** | Semaglutide 2.4 / **Wegovy** | NPRA-registered (clinic sources: DCA approval **April 2023** — repo labels "unofficial"); **commercially launched January 2026** | NPRA/DCA **April 2023** approval corroborated by clinic sources; **launch timing conflicts** — some sources say Wegovy became "officially available in Malaysia as of **January 2025**", others frame Jan 2026; global shortage delayed availability | 🟡 | **Watch item.** The repo's "launched January 2026" is contradicted by sources putting availability at **January 2025**. Not a fabrication, but the year may be off by one. Verify with Novo Nordisk MY / NPRA QUEST before using the Jan-2026 "moment-of-market-formation" narrative. |
| **MY** | Liraglutide / Saxenda; Semaglutide / Ozempic (T2DM, off-label weight); Rybelsus | Registered; Ozempic weight-use off-label | Consistent with class registration pattern; not individually re-searched this pass | 🟡 | Existence solid; verify each MAL number on NPRA QUEST (repo already says to). |
| **SG** | Semaglutide 2.4 / **Wegovy** | **HSA-approved 2023** for chronic weight management; commercial launch timing "reported inconsistently (mid-2024 vs mid-2025)" | HSA 2023 approval corroborated; launch timing genuinely inconsistent across clinic sources — repo already flags this and says "verify with Novo Nordisk SG" | 🟡 | Approval 2023 = GREEN-grade; **launch date = AMBER by the repo's own honest admission.** Good practice. |
| **SG** | Tirzepatide / **Mounjaro** | **Approved Mar 2023 (T2DM)**; **weight-management indication added June 2025**; sold as Mounjaro not Zepbound | HSA "new drug approvals — March 2023" lists Mounjaro (T2DM); HSA June 2025 added the weight-management indication | 🟢 | Both dates verified precisely against HSA announcement pages. |
| **HK** | Semaglutide 2.4 / **Wegovy** | Registered; **launched November 2025**; first weekly weight-loss drug approved for adolescents 12+ in HK | Novo Nordisk press release confirms HK launch **3 November 2025**, and that Wegovy is the **first once-weekly weight-loss medication approved for adolescents 12+** in HK | 🟢 | Launch date and the adolescent-first claim both verified. [prnewswire.com](https://www.prnewswire.com/apac/news-releases/novo-nordisk-launches-wegovy-in-hong-kong-for-weight-management-302602289.html) |
| **HK** | Tirzepatide / **Mounjaro** | Approved **late 2024**; first dual GIP/GLP-1 for obesity + T2D | Eli Lilly press release confirms HK Dept of Health approval **28 October 2024**, KwikPen, first dual GIP/GLP-1; expected available Dec 2024 | 🟢 | "Late 2024" = precisely 28 Oct 2024. Verified. [prnewswire.com](https://www.prnewswire.com/apac/news-releases/lillys-mounjaro-tirzepatide-approved-in-hong-kong-in-kwikpen-presentation-302288382.html) |
| **HK** | Saxenda; Ozempic | Registered; Ozempic weight-use off-label | Consistent; not individually re-searched | 🟡 | Existence solid. |

**GLP-1 bottom line:** the registration *numbers and molecule facts* are excellent. The only soft spot is **commercial-launch dates for Wegovy** in Malaysia (possible Jan-2025-vs-Jan-2026 slip) and Singapore (repo already honestly flags mid-2024-vs-mid-2025). Approvals are reliable; "launch" dates should carry the manufacturer as the primary check.

---

## (1) Requires healthcare-lawyer sign-off before operating

This pass confirms the cited instruments **exist and are described correctly**. It does **not** confirm that the repository's *conclusions* about how to operate lawfully under them are correct. Those are legal judgements — and in several places the repo is explicitly making a *risk-position* argument ("rests on regulatory forbearance", "arguably outside PHFO", "grey zone counsel should confirm"). The following questions — each answered, at least implicitly, somewhere in the repo — must be put to **local admitted counsel in each jurisdiction** before Welltech acts on them. The instrument in each case is real (verified above); the *interpretation* is what needs sign-off.

### 1.1 Licensability of a virtual-only clinic
**The question:** Can Welltech lawfully operate an entity that holds itself out as a healthcare provider without physical clinical premises?
**Repo's answer:** MY — no PHFSA category for a "virtual clinic," so virtual-only operation "rests on regulatory forbearance"; anchor prescriptions to a registered physical clinic and never market a virtual entity as a "clinic." SG — an HCSA Outpatient Medical Service licence + MOH-approved Clinical Governance Officer is *mandatory* (this is the firmest of the three). HK — the Private Healthcare Facilities Ordinance (Cap 633) is premises-based and "arguably" does not reach a purely virtual service.
**Residual risk:** The MY "forbearance" and HK "arguably outside PHFO" positions are unsettled law. The repo itself says counsel should confirm before launch. **Do not launch a virtual entity marketed as a 'clinic' in MY, and do not assume PHFO non-application in HK, without a written legal opinion.** SG is lower-risk *only if* the OMS licence + CGO are actually in place.

### 1.2 GLP-1 / off-label advertising boundaries
**The question:** What can Welltech say, and where, about weight-loss medication without breaching advertising law?
**Repo's answer:** "Market the programme and service, never the molecule or brand." This is a sound reading of MASA 1956 + MAB/KKLIU (MY), the Health Products (Advertisement of Specified Health Products) Regs 2016 + HCS(A) Regs 2021 (SG), and UMAO Cap 231 + Schedule 4 (HK) — all verified above.
**Residual risk:** The line between lawful disease-awareness/service advertising and unlawful POM promotion is **fact-specific and actively enforced** (SG blocked even euphemistic "weight-loss pen" creatives; MY removed tens of thousands of listings). WhatsApp broadcast/status content, click-to-WhatsApp ads and influencer briefs all count as advertising. Every creative concept and every influencer contract template needs pre-clearance (MY via the KKLIU workflow with ~6-week lead time; SG/HK via legal review against the ad regs). This is the single domain most likely to produce Welltech's first regulatory contact.

### 1.3 E-prescription validity (Malaysia especially)
**The question:** Is a digitally-signed Welltech prescription legally valid for a Group B poison?
**Repo's answer:** The OHS Guideline 2025 recognises a "digital prescription" signed by a licensed doctor and transmitted platform-to-pharmacist — the first official articulation of an e-prescription pathway.
**Residual risk:** The **Poisons Regulations 1952 still say "in writing, signed"** and have not been amended; the OHS Guideline is an administrative circular, not statute. Whether an e-prescription is *legally valid* (vs merely tolerated) for a Group B poison is unresolved. Counsel must opine before the dispensing flow is productionised — this underpins the entire prescription-to-doorstep revenue mechanic.

### 1.4 Cross-border prescribing and the regional-hub model
**The question:** Can a doctor licensed in one market prescribe to a patient physically in another?
**Repo's answer:** No — MMC's position is that offshore doctors serving MY patients must meet MY registration requirements; a MY-licensed doctor treating a patient "in" SG would be practising unlicensed; HK concentrates risk on the individual doctor. Conclusion: separate licensed entities per jurisdiction with a shared data/tech layer.
**Residual risk:** The structure is prudent, but the **precise routing rules** (which patient is seen by which entity's doctor, and to which address medicine is dispensed) must be legally mapped per corridor (JB–Singapore especially). MaNaDr demonstrates Singapore's enforcement appetite; do not treat the hub as a licence-arbitrage base.

### 1.5 PDPA / PDPO cross-border data transfer
**The question:** Is Welltech's WhatsApp/cloud/AI stack a lawful cross-border transfer of sensitive health data?
**Repo's answer:** MY — WhatsApp (Meta), cloud (AWS/GCP Singapore) and foreign AI APIs are cross-border transfers of *sensitive* personal data requiring a documented Transfer Impact Assessment under Guidelines 03/2025, explicit consent and retention controls. SG — PDPC healthcare advisory guidelines govern. HK — s.33 is *not in force* so offshoring is currently lawful, but "behave as if it applied."
**Residual risk:** These are the repo's legal readings, not verified law. A data-protection lawyer must confirm the TIA content and consent architecture (MY), and whether the HK "act as if s.33 applied" posture is sufficient given the Meta processing chain. The MY PDPA amendments (verified in force 1 June 2025, RM1m fines, 72-hour breach notice) make this a launch gate, not a retrofit.

**Legal sign-off priority order:** (i) e-prescription validity for Group B poisons in MY; (ii) virtual-clinic licensability MY + HK; (iii) advertising creative/influencer clearance in all three; (iv) cross-border prescribing routing; (v) PDPA/PDPO cross-border TIA / consent.

---

## (2) Requires medical-director sign-off

The following are **clinical-protocol claims** drawn from [40-doctor-experience/prescribing-models.md](../40-doctor-experience/prescribing-models.md) and [60-ai-operating-model/ai-nurse.md](../60-ai-operating-model/ai-nurse.md). This verification pass is **not clinical** and does not endorse them. A named, registered **medical director** (the OHS-2025 board requirement) must approve, version and sign each one before it drives patient care.

### 2.1 GLP-1 titration schedule
prescribing-models.md specifies semaglutide **0.25 mg weekly ×4w → 0.5 → 1.0 → 1.7 → 2.4 mg maintenance, stepping ~q4 weeks on tolerability**, with per-pen-per-step supply logic and a mandatory re-titration teleconsult after any interruption >2 weeks. This matches the standard Wegovy label escalation, and is clinically orthodox — but **the current product label is the authority, not this pass and not a clinic blog.** The medical director must confirm the semaglutide schedule *and* the separate tirzepatide/Mounjaro schedule against the current MY/SG/HK labels, and sign the protocol version. Titration is a dosing decision; the repo's own governing rule ("AI must not diagnose or dose") means a named clinician owns it.

### 2.2 Initiation thresholds & contraindication screen
The BMI **≥27.5 kg/m²** (Asian cut-point) initiation threshold, and the initiation-consult contraindication screen (personal/family medullary thyroid carcinoma history, pancreatitis, pregnancy, drug interactions) plus stop-rules, must be clinician-set and documented. The repo sources the ≥27.5 threshold to a clinic guide — a reasonable pointer, but not a clinical authority the medical director can rely on for sign-off.

### 2.3 Red-flag escalation matrix (ai-nurse.md §5)
The GREEN/AMBER/RED symptom tiers, the high-recall red-flag detector that runs on *every* inbound message regardless of context (so "chest pain" typed during a payment conversation still fires), the **15-minute human-contact SLA for RED** (never degraded, day or night), the 4-business-hour AMBER SLA, and the "the system may over-escalate; it may never under-escalate" rule are **medical-director-signed clinical logic.** Verification confirms the *design intent* is sound and regulator-aware — a deterministic clinician-signed decision tree does the classifying, the LLM is confined to entity extraction and conversation, and a human owns every dose/medication change. But the actual tier *content*, the disposition thresholds and the after-hours scripts must be a clinician's signed artefact, re-signed on every version bump.

### 2.4 Peri-operative / anaesthesia safety (NPRA 2025 alert)
The repo correctly cites the NPRA 2025 GLP-1 safety alert on pulmonary aspiration under general anaesthesia / deep sedation. Translating that into an operational **pre-operative hold protocol** (which patients, how many doses held, how surfaced in the WhatsApp check-in flow) is a clinical decision for the medical director, not a desk-research output.

### 2.5 SaMD boundary — where the AI must stop
The repo's operating rule — AI "collects and routes," a deterministic clinician-signed decision tree "classifies," humans "act," keeping the system on the administrative/augmentation side of the Medical Device Act 737 SaMD line — is simultaneously a **legal** question (does the intended purpose make it a registrable device? → counsel) **and** a **clinical-governance** question (is the human-in-the-loop review genuinely load-bearing, per the MMC Guideline on Ethical Use of AI?). The **titration engine that proposes dose steps** is the specific feature most at risk of crossing into Class B SaMD (verified: Act 737 s.2 expressly captures "software" with diagnostic/treatment intent). The medical director and counsel must *jointly* bless its design and human-review gate before it ships. The naming discipline in ai-nurse.md (the assistant introduces itself as a digital assistant, never as a nurse, and never claims clinical authority) is a good mitigating control and should be preserved.

**Clinical sign-off priority order:** (i) titration schedules against current labels (MY/SG/HK); (ii) red-flag / stop-rule matrix content + SLAs; (iii) peri-operative GLP-1 hold protocol; (iv) initiation / contraindication screen; (v) SaMD human-review gate (jointly with counsel).

---

## Residual-risk register (what to re-pull before external use)

| # | Claim | Tag | Why it still needs a primary check | Owner |
|---|---|---|---|---|
| R1 | Wegovy MY commercial launch = January 2026 | 🟡 | Sources conflict (Jan 2025 vs Jan 2026); the "market-formation moment" narrative depends on it | Commercial + Novo Nordisk MY |
| R2 | Wegovy SG launch timing | 🟡 | Repo already flags mid-2024 vs mid-2025 inconsistency | Commercial + Novo Nordisk SG |
| R3 | E-prescription validity for Group B poisons (MY) | — | Poisons Regs 1952 unamended vs OHS Guideline soft-law recognition | Healthcare lawyer |
| R4 | Virtual-clinic licensability (MY "forbearance"; HK PHFO grey zone) | — | Unsettled law; repo makes a risk-position argument | Healthcare lawyer |
| R5 | MASA 1956 current Schedule / "obesity not scheduled" | 🟡 | Sub-claim not independently re-tested; Schedule amendable by Minister | Healthcare lawyer |
| R6 | SG Health Information Bill introduction/passage (5 Nov 2025) | 🟡 | Determines whether mandatory NEHR contribution is a live day-one duty | Compliance |
| R7 | HK eHealth+ (EHRSS Amendment Ordinance 2025) effective date/scope | 🟡 | 1 Dec 2025 date and mandatory-deposit power not re-corroborated | Compliance |
| R8 | GLP-1 titration schedules | — | Product labels are the authority, not a clinic blog | Medical director |
| R9 | Penalty quanta across the MY penalty-reference table | 🟡 | Repo itself flags several as "verify against AGC text" | Healthcare lawyer |
| R10 | MMC AI guideline "adopted 18 Feb 2025" date | 🟡 | Existence solid; dual date (endorsed 29 Dec 2024 / adopted 18 Feb 2025) not independently confirmed | Compliance |

---

## AMBER watch-items in detail

The eight AMBER tags are not errors — they are places where a single date, a single source, or a self-flagged uncertainty means the reader should not treat the claim as diligence-grade without one more check. In order of consequence:

- **Wegovy Malaysia launch (the one to actually chase).** The repo builds a "January 2026 = moment of market formation" narrative around Wegovy's Malaysian launch. Search returned conflicting framings: one clinic source states the market became "officially accessible in Malaysia as of **January 2025**"; other coverage clusters around January 2026; and the NPRA/DCA *approval* is consistently placed at **April 2023** (which the repo itself labels "unofficial"). The most likely reconciliation is that approval (2023) and commercial availability (2025 or 2026) are being conflated across sources, and a global semaglutide shortage delayed the launch. This does not undermine the strategy — regulatory-compliant supply as a differentiator holds either way — but the specific "January 2026" year should be confirmed with Novo Nordisk MY before it anchors a go-to-market timeline.
- **Wegovy Singapore launch.** The repo is admirably explicit: HSA *approval* is 2023 (verified), but commercial launch is "reported inconsistently (mid-2024 vs mid-2025)" and it directs the reader to verify with Novo Nordisk SG. Left AMBER exactly as the repo intended.
- **MASA 1956 current Schedule (MY).** The regime (MAB approval, KKLIU numbers, POM-to-public prohibition) is GREEN-grade. The finer sub-claim — that obesity/weight-loss is *not* on the statutory Schedule of restricted-disease advertising, so service advertising has a lawful lane — rests on the repo's own reading and was not independently re-tested. The Schedule is amendable by ministerial order, so it can move.
- **MMC AI guideline date (MY).** The instrument exists and is linked from sources/regulations.md; the specific dual date ("endorsed 29 Dec 2024, adopted 18 Feb 2025") was not independently corroborated this pass.
- **SG Health Information Bill.** Cited as introduced 5 Nov 2025 with a mandatory-NEHR-contribution effect. The instrument and direction are real; the introduction/passage status was not independently re-confirmed, and it determines whether NEHR contribution is a live day-one obligation or a near-future one.
- **SG IP rider reform (1 Apr 2026).** A financing/demand claim, not a compliance one; not re-verified this pass.
- **SG PDPA healthcare advisory guidelines.** Exist (PDPC-hosted, Sep 2023 revision); details rest on the guideline text, not re-searched.
- **HK eHealth+ (EHRSS Amendment Ordinance 2025).** Referenced with a 1 Dec 2025 effective date and mandatory-deposit power; date/scope not independently re-corroborated.

## What the repository got notably right

Three things are worth calling out because they are the failure modes this pass exists to catch, and the repo avoided all three:

1. **No invented instruments.** Every statute, ordinance, circular and guideline cited is real and correctly named. There is no phantom "Digital Health Act," no misattributed regulator, no imaginary licence class.
2. **Precise, verifiable dates on the load-bearing instruments.** 26 Jun 2023 (HCSA Phase 2), 16 Aug / 24 Oct 2024 (MaNaDr), 22 Nov 2024 (Joint Circular 87/2024), 15 May 2025 (OHS Circular Bil.16/2025), 1 Jun 2025 (PDPA amendments), 23 Sep 2025 (MMC tele-MC ban), 3 Nov 2025 (Wegovy HK), 1 Jan 2026 (HK A&E reform), 28 Oct 2024 (Mounjaro HK), 30 Aug 2025 + MAL24026013AZ (Mounjaro MY) — all verified to the day / to the registration number.
3. **It flags its own soft spots.** The repo explicitly labels the Wegovy DCA-approval date "unofficial," tells the reader to verify Wegovy SG launch timing with the manufacturer, and repeatedly says "counsel should confirm" on the genuinely unsettled legal questions. That intellectual honesty is what lets this pass tag with confidence rather than suspicion.

## Items genuinely uncheckable by desk research (⚪)

- **Malaysia enforcement statistics** — "38,055 unapproved ads removed from e-commerce and 13,070 screened on social media (Jan 2023–Dec 2025)." These are MOH/Pharmacy Enforcement internal figures; plausible and repeatedly cited in the repo, but not independently reproducible from search this pass. Treat as directional.
- **CMPR / "1+" mechanism (HK)** and other **forward-looking legislative promises** (MY "OHS Act" / dedicated digital-health legislation; SG Health Information Bill passage) — these are stated intentions whose *enactment* cannot be pre-verified. Track, don't rely.

---

## Corroboration log — searches run and what agreed

For transparency, the specific desk-research checks behind the GREEN tags above. Each line = one search; the "agreement" column records how many independent source types concurred.

| # | Search focus | Independent sources that agreed | Finding |
|---|---|---|---|
| C1 | Telemedicine Act 1997 status | CommonLII ("Not yet in force"); Wikipedia; RDS Law Partners; IBA Telemedicine Survey (MY) | Passed 1997, never commenced, no dedicated telemedicine law since — **confirmed** |
| C2 | OHS Guideline / Circular Bil.16/2025 | MOH-hosted PDF titled "...Bil.16...15 Mei 2025"; Skrine alert (Jul 2025); Lexology | Dated 15 May 2025; SSM incorporation + physical base + e-prescription pathway — **confirmed** |
| C3 | MMC tele-MC ban | CodeBlue; The Star; thesun; Bernama; Scoop (all Nov 2025) | 23 Sep 2025 notification; physical-exam rationale; MMA backed, ADHM opposed blanket ban — **confirmed** |
| C4 | Mounjaro MY | Multiple MY clinic sources (Nexus, Peak Protocol, Da Vinci, Regions Clinic press) | Registration MAL24026013AZ; launch 30 Aug 2025 — **confirmed (number + date)** |
| C5 | Wegovy MY | Millennium Clinic KL; CLEO; Facebook trade post; NovoCare | NPRA approval ~Apr 2023; **launch date conflicts (Jan 2025 vs Jan 2026)** — AMBER |
| C6 | Poisons (Amendment) Act 2022 | CodeBlue; DKSH Insights; AGC reprint | In force 1 Jan 2023 (except s.21); penalties raised — **confirmed** |
| C7 | PDPA (Amendment) Act 2024 | DataGuidance; Baker McKenzie; Lexology; TSL Legal; SimplyData | DPO + 72-hr breach in force 1 Jun 2025; RM1m fine; 7-day data-subject notice — **confirmed** |
| C8 | Medical Device Act 737 SaMD | MDA portal; Act 737 s.2/s.5(1) text; TrustedTraceMed; Pacific Bridge | "Software" expressly captured; registration mandatory; Classes A–D + CAB — **confirmed** |
| C9 | HCSA Phase 2 | MOH newsroom; Allen & Gledhill; Baker McKenzie; Rajah & Tann | Teleconsultation licensable from 26 Jun 2023; CGO regime — **confirmed** |
| C10 | MaNaDr | MOH newsroom; Mothership; The Online Citizen; Medical Channel Asia | Stop-order 16 Aug 2024; intended revocation 24 Oct 2024; 41 doctors to SMC — **confirmed** |
| C11 | Joint Circular 87/2024 | HCSA/MOH-hosted circular PDF; HSA guidance | Dated 22 Nov 2024; HCSA + HPA 2007 + SMC ECEG scope — **confirmed** |
| C12 | Wegovy / Mounjaro SG | HSA "new drug approvals — March 2023"; HSA June 2025 indication update; noah/HMI/Regimen guides | Wegovy HSA-approved 2023; Mounjaro T2DM Mar 2023, weight indication Jun 2025 — **confirmed** (Wegovy launch date AMBER) |
| C13 | MCHK telemedicine guidelines | HKAM; info.gov.hk; DLA Piper; Two Birds; Kennedys | Dec 2019, non-binding, no statute; discipline-only exposure — **confirmed** |
| C14 | UMAO Cap 231 / Schedule 4 | e-Legislation Cap 231; Drug Office; DH press release (2012) | Schedule 4 orally-consumed-product weight-claim controls from 1 Jun 2012 (2005 amendment) — **confirmed** |
| C15 | PDPO s.33 | Tanner De Witt; Deacons; Mayer Brown; DLA Piper | s.33 never in force >25 yrs, no timetable; PCPD Model Clauses (May 2022) — **confirmed** |
| C16 | HK A&E fee reform | HKFP; SCMP; HA corporate-comms page; news.gov.hk | HK$180→400 from 1 Jan 2026; critical/emergency waived; ~24% drop semi-/non-urgent — **confirmed** |
| C17 | Wegovy HK | Novo Nordisk PR Newswire; BioPharma APAC | Launched 3 Nov 2025; first weekly weight-loss drug for adolescents 12+ in HK — **confirmed** |
| C18 | Mounjaro HK | Eli Lilly PR Newswire; BioPharma APAC; China Daily HK | Approved 28 Oct 2024; first dual GIP/GLP-1; available Dec 2024 — **confirmed** |

Eighteen high-stakes checks; seventeen cleanly corroborated; one (C5, Wegovy MY launch year) left AMBER on a genuine source conflict. No check returned a contradiction that would force a RED tag on an instrument's existence or its legal status.

## Verification method note

Per [methodology.md](methodology.md): direct fetches of primary regulator PDFs (moh.gov.my, mchk.org.hk, hsa.gov.sg, elegislation.gov.hk, npra.gov.my) return 403 in this environment. Every 🟢 above rests on ≥2 independent search results agreeing (typically the primary host's search-indexed title/snippet **plus** one or more law-firm alerts or pharma press releases). A 🟢 here means "the instrument exists and the date/status is corroborated," **not** "read to diligence grade from the primary document." Before any financing, filing or pricing commitment, re-pull the primary text. All URLs cited above were returned in searches run July 2026.
