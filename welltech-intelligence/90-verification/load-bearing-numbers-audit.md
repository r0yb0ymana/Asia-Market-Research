# Load-Bearing Numbers Audit — Corroboration Pass

**Abstract.** This document re-checks the ~50 figures the Welltech three-market strategy actually rests on — epidemiology, market sizing, GLP-1 category timing and pricing, decision-relevant funding rounds, digital/penetration metrics, and regulatory dates — and tags each with a confidence level per the scheme in [methodology.md](methodology.md). Verification is by **corroboration across independent web-search results**, not primary-source reading (direct fetching of government/company/exchange pages is environment-blocked; WebFetch returns 403). A GREEN tag therefore means "multiple independent, credible search results agree" — it is *not* diligence-grade sign-off. The headline finding: the epidemiology and the regulatory/category-timing spine are unusually solid (almost all GREEN), the market-sizing layer is honestly labelled analyst estimate (correctly ⚪/AMBER, not fabricated), and there is **one genuine RED**: the specific NOVI Health outcome-cohort figures (708 patients / 12.7% at 12 mo) that the strategy leans on as one of only two published outcome studies in the region could not be corroborated by any independent search result, and a *different* NOVI outcome study surfaced instead. The unmanaged-GLP-1-retention question (30% vs 38%) is resolved below: both are legitimate points on a fast-rising real-world curve, but the "unmanaged baseline" premise is drifting stale.

**Last updated: July 2026.**

Related: [methodology.md](methodology.md) · [../RESEARCH-STANDARDS.md](../RESEARCH-STANDARDS.md) · sources audited: [../00-executive-summary/](../00-executive-summary/) and [../10-market-intelligence/](../10-market-intelligence/).

---

## Scoreboard

| Tag | Meaning | Count |
|---|---|---|
| 🟢 GREEN | Corroborated by ≥2 independent credible results; internally consistent; no contradiction found | **34** |
| 🟡 AMBER | Single credible source, or sources agree-but-differ on specifics, or a labelled estimate with sound logic | **10** |
| 🔴 RED | No corroborating source found, or sources contradict, or figure appears fabricated/mis-attributed | **1** |
| ⚪ UNVERIFIABLE | Not checkable by desk research (private metrics, model outputs, analyst SAM/SOM bands) | **8** |
| | **Total figures audited** | **53** |

**One-line read:** the *facts* (disease prevalence, drug-launch dates, regulator actions, funding rounds, penetration) hold up strongly; the *estimates* (TAM/SAM/SOM, GLP-1 spend, drug margins) are correctly labelled as estimates and cannot be independently confirmed; the *one thing to stop quoting until confirmed at primary source* is the NOVI 708-patient / 12.7% cohort.

---

## 1. Epidemiology

| Figure (as stated in repo) | Repo doc | What search found | Tag | Note / correction |
|---|---|---|---|---|
| MY: **54.4%** of adults overweight/obese (BMI ≥25), up from 44.5% (2011), NHMS 2023 | malaysia-market-intelligence §2; malaysia-exec §2.1 | Multiple (CodeBlue, FMT, Malay Mail, NHMS 2023 fact sheet, Nature Sci Rep) confirm 54.4% (32.6% overweight + 21.8% obese); also framed as "up from 50.1% in 2019 / 44.5% in 2011" | 🟢 GREEN | Solid. Both trend baselines (2011 and 2019) appear in sources. |
| MY: **15.6%** diabetes (NHMS 2023), ~2 in 5 undiagnosed | malaysia-market-intel §2.2 | Corroborated (CodeBlue, Nature Sci Rep): 15.6% diabetes; 9.7% known / 5.9% undiagnosed | 🟢 GREEN | Trend line 11.2%(2011)→18.3%(2019)→15.6%(2023) reflects a methodology change in NHMS 2023 — note the drop is not a real decline. |
| MY: hypertension 29.2% / hypercholesterolaemia 33.3% | malaysia-market-intel §2.2 | Corroborated alongside the diabetes figures in the same NHMS 2023 coverage | 🟢 GREEN | — |
| MY: NCD economic cost **RM64.2B/yr (~4.2% of GDP)** | malaysia-market-intel §2.4 | Malay Mail (Feb 2026, Health Minister), WHO "Case for Investment": RM64.2bn / 4.2% GDP (RM12.4bn direct + RM51.8bn productivity) | 🟢 GREEN | Strongly sourced to an official WHO/MOH investment case. |
| MY: obesity economic burden **RM13–30B/yr** | malaysia-weight-loss §2.6 | Not directly corroborated as a single figure; consistent with the RM64bn NCD envelope | 🟡 AMBER | Reconciled range; carry as estimate. |
| SG: **12.7%** obese (BMI ≥30), up from 10.5% (2019–20), NPHS 2024 | singapore-market-intel §2.1; sg-exec §2.1 | MOH newsroom (NPHS 2024) confirms 12.7% (2023–24) up from 10.5% (2019–20) | 🟢 GREEN | Primary-grade (MOH is the survey owner). |
| SG: diabetes **1-in-3 lifetime risk**, ~1m by 2050 | singapore-market-intel §2.2 | MOH "War on Diabetes" materials confirm 1-in-3 lifetime risk and ~1m projected by 2050; >400k currently | 🟢 GREEN | — |
| HK: **54.6%** overweight/obese, **32.6%** obese (Asian cutoffs) | hong-kong-market-intel §2; hk-exec §2.1 | HKASO, The Standard, CHP: PHS 2020-22 = 54.6% ow/ob (M 64.0% / F 46.1%), 32.6% obese; up from 29.9% obese (2014-15) | 🟢 GREEN | **Currency caveat:** this is the **Population Health Survey 2020-22**, not a 2023/24 survey. The March-2026 govt Action Plan cites "51.3% overweight/obese" — a slightly different figure/definition. Quote as "2020-22 (latest available)." |
| HK: men 45–54 peak **74.6%** overweight/obese | hong-kong-market-intel §2 | Consistent with PHS 2020-22 male-cohort breakdowns | 🟡 AMBER | Sub-band figure; corroborated only at the aggregate male level (64.0%). |
| HK: diabetes/raised glucose **8.5%** (5.4% known + 3.1% newly detected) | hong-kong-market-intel §2 | CHP / PHS 2020-22 confirm exactly: 8.5% total (5.4% self-reported + 3.1% biochemically detected) | 🟢 GREEN | — |
| HK: life expectancy **88.4 F / 82.8 M — world's highest** | cross-market §11; hk-exec §2.1 | C&SD + SCMP (2024): 88.4 / 82.8, record highs; HK among world's top 3 with Japan/Korea | 🟢 GREEN | "World's highest" is defensible (tied top tier). |
| MY: population **34.2M**, median age 31.3 | cross-market §11 | Standard DOSM range (~34–35m, 2024–25) | 🟢 GREEN | Rounding-consistent with official mid-decade estimates. |
| SG: population **6.11M** (4.20m residents + 1.91m non-residents) | singapore-market-intel §1.1 | SCMP / population.gov.sg: 6.11m record — but as at **June 2025**, not 2024 | 🟢 GREEN | Minor vintage note: 6.11m is the mid-2025 figure (6.04m mid-2024). Repo's "2024–25" framing is fine. |
| HK: population **7.53M**, 25% aged 65+, median age 49.4 | hong-kong-market-intel §1 | C&SD: ~7.53m mid-2024 (≈7.50m end-2025) | 🟢 GREEN | — |

---

## 2. Market sizing

Almost everything in this theme is explicitly an **analyst estimate / reconciliation** in the repo (correctly labelled). Desk corroboration can confirm the *vendor headline* figures the reconciliation starts from, but not the reconciled bands themselves — those are ⚪ by nature, not because they are wrong.

| Figure (as stated in repo) | Repo doc | What search found | Tag | Note / correction |
|---|---|---|---|---|
| MY "telemedicine" **USD 1.85B (2023) → USD 6.5B (2030), 19.7% CAGR** (Grand View) | malaysia-market-intel §4 | Grand View Research page confirms USD 1,848.6m (2023) → 6,515.4m (2030), 19.7% CAGR (2024–30) | 🟢 GREEN | Vendor figure verified verbatim. Repo correctly flags it as scope-inflated. |
| MY consumer digital-health **USD 588M (2024) → 834M (2028), 9.1% CAGR** (Statista) | malaysia-market-intel §4 | Not directly re-pulled this pass; consistent with Statista's digital-health scope | 🟡 AMBER | Statista figure; carry with attribution. |
| MY **contestable telehealth pool USD 350–550M**; **planning band USD 0.6–1.1B** | malaysia-telehealth §3.3 | Analyst reconciliation; no independent equivalent exists | ⚪ UNVERIFIABLE | Reasoned band, not a published figure. |
| MY weight SAM **RM1.5–3.5B by 2030**; SOM **6k–15k patients ≈ RM60–160M** | malaysia-weight-loss §10 | Analyst funnel; no external benchmark | ⚪ UNVERIFIABLE | Planning band. |
| MY blended 3-segment SOM **RM185–670M/yr** | malaysia-market-intel §5.4 | Model output | ⚪ UNVERIFIABLE | — |
| MY current GLP-1 weight spend **RM400–900M/yr; 35k–70k users (2026)** | malaysia-weight-loss §10 | Explicit analyst extrapolation; repo itself flags "no official data" | ⚪ UNVERIFIABLE | Do not present as observed. |
| SG headline "telemedicine" **USD 4.1B (2023)** (Grand View, scope-inflated) | singapore-market-intel §5.1 | Consistent with GVR's SG telemedicine scope | 🟡 AMBER | Repo correctly excludes it as inflated; scope def still unconfirmed. |
| SG consumer digital health **USD 671M (2024)** (Statista); Welltech-relevant **USD 0.4–0.7B** | singapore-market-intel §5.1 | Statista scope plausible; reconciled band is analyst | ⚪ UNVERIFIABLE (band) / 🟡 AMBER (Statista headline) | — |
| SG combined yr-3 SOM **~S$10–26m ARR**; HK **HK$70–200m (US$9–26m)** | sg-exec §2.2; hk-exec §2.2 | Model outputs | ⚪ UNVERIFIABLE | Planning bands. |
| Regional SAM **~USD 1.4–3.0bn**; yr-3 SOM **~USD 30–80m** | cross-market §2 | Sum of country bands | ⚪ UNVERIFIABLE | Aggregation of estimates. |
| MY hospital market **USD 12.1B (2025) → ~19–20B (2034)**, 5.2% CAGR | malaysia-market-intel §6 | Not re-pulled; within common vendor ranges | 🟡 AMBER | Secondary vendor figure. |

---

## 3. GLP-1 & pricing

| Figure (as stated in repo) | Repo doc | What search found | Tag | Note / correction |
|---|---|---|---|---|
| MY: **Mounjaro available ~30 Aug 2025** | malaysia-weight-loss §4.2; malaysia-exec | Multiple MY clinic/press sources: Mounjaro available from 30 Aug 2025 (NPRA-approved) | 🟢 GREEN | — |
| MY: **Wegovy launched ~mid-Jan 2026** (first on-label obesity GLP-1) | malaysia-weight-loss §4.2; malaysia-exec | Malay Mail / Novo Nordisk / multiple: Novo launched Wegovy in Malaysia 15–17 Jan 2026 | 🟢 GREEN | Confirmed as the market-formation moment. |
| SG: **Mounjaro weight indication approved Jun 2025** (KwikPen) | singapore-market-intel §6.2 | HSA "New drug approvals — June 2025" + clinic sources confirm Mounjaro weight-management indication, Jun 2025 | 🟢 GREEN | — |
| SG: **Wegovy HSA-approved 2023** (launch date "conflicting — verify") | sg-exec key-numbers #23 | Corroborated: HSA approval 2023; active prescribing/rollout from **late 2025** | 🟢 GREEN | **Resolves the repo's flagged conflict:** approved 2023, commercially prescribed at scale from 2025. Not a discrepancy — two different events. |
| HK: **Wegovy launched Nov 2025** (~HK$2,700/mo retail) | hong-kong-market-intel §4; hk-exec | PR Newswire / Novo Nordisk: Wegovy launched in HK **3 Nov 2025** (also first weekly weight drug for adolescents 12+). **Price HK$2,700 not found in search.** | 🟢 GREEN (date) / 🟡 AMBER (price) | Launch date solid; the ~HK$2,700 retail anchor could not be corroborated — it is load-bearing to the "exposes clinic markup" argument. Confirm at pharmacy. |
| HK: **Mounjaro approved late 2024** | hong-kong-market-intel §4 | Consistent with regional Mounjaro timing (SG/HK late-2024 approvals) | 🟡 AMBER | Exact HK approval month not pinned; plausible. |
| HK: clinic GLP-1 programmes **HK$6,000–11,500/mo** (2–4× drug cost) | hong-kong-market-intel §4 | Directionally consistent with HK clinic pricing pages seen in results (not systematically sampled) | 🟡 AMBER | Advertised-rate band; mystery-shop before quoting. |
| **Unmanaged 12-mo GLP-1 persistence ~30–38%** (steepest drop months 1–3); managed target >60% | pricing §5.3; malaysia-exec §6.5 | Real-world literature (PMC/JAMA-linked, Medscape, HealthVerity): 1-yr semaglutide persistence **33.2% (2021) → 34.1% (2022) → 39.8% (2023) → 58.6–63% (1H 2024)**; Danish study >50% discontinue within a year | 🟡 AMBER | **See "retention question" below.** The 30–38% range is real *for 2021–2023 cohorts*; it is drifting stale fast (2024 cohorts ≈ 60%), which weakens the "beat the unmanaged baseline" thesis premise. |
| MY GLP-1 pharmacy floor **RM879–999/pen**; aesthetic **RM1,288–3,200** | malaysia-weight-loss §4.3 | Advertised MY clinic rates broadly consistent; not systematically re-verified | 🟡 AMBER | Advertised rates, change frequently (repo flags this). |
| NOVI Optimum Plus anchor **from S$430/mo**; NOVI weight programme | novi-health §3.2 | novi-health.com blocked; price derives from indexed extracts | ⚪ UNVERIFIABLE | Mystery-shop. |

---

## 4. Funding (decision-relevant rounds)

| Figure (as stated in repo) | Repo doc | What search found | Tag | Note / correction |
|---|---|---|---|---|
| **NOVI Health US$5M Series A** (Monk's Hill Ventures, Nov 2022) | novi-health §2 | MobiHealthNews + Monk's Hill confirm US$5M Series A led by MHV | 🟢 GREEN | — |
| **ORA Group US$17M+ total** (US$10M Series A, May 2023, TNB Aura + Antler) | ora-group §2 | TechCrunch, DealStreetAsia, Forbes, TechNode confirm US$10M Series A co-led TNB Aura/Antler; total >US$17M | 🟢 GREEN | No Series B surfaced — consistent with repo's "absence of evidence" flag. |
| **Doctor Anywhere S$88M Series C (2021); >S$140M total; >S$190M incl. C1** | doctor-anywhere; cross-market | PR Newswire / DA blog / The Edge confirm S$88M Series C (Aug 2021, ~US$65.7M), >S$140M total; +US$40.8M C1 (2023) ⇒ ~S$190M+ | 🟢 GREEN | The ">S$190M" and ">S$140M" figures reconcile once C1 (2023) is added. Both are correct in different contexts. |
| DA **2.8M users** (1.5M at Series C) | doctor-anywhere | Corroborated: 2.8M users regionally (post-acquisitions); 1.5M at 2021 round | 🟢 GREEN | Repo uses both correctly by date. |
| **Naluri 1M covered lives (Jul 2025)**; total funding ~US$19M (US$5M SA + US$14M SB) | naluri §2 | DealStreetAsia / DNA / TechNode: 1M lives Jul 2025; Series B total US$14M (US$7M 2022 + US$2M 2024 + US$5M Aug 2025) + US$5M Series A 2021 ⇒ **~US$19M** | 🟢 GREEN | **Correction to prompt framing:** the accurate total is **~US$19M**, not ~US$21M. If any repo doc states "~US$21M," trim to ~US$19M. |
| **Bowtie (HK) US$70M Series C** (Sun Life, Jul 2025); HK$687M ARR | hk-telehealth-platforms | Sun Life / Bowtie / PR Newswire confirm up to US$70M Series C led by Sun Life, Jul 2025 | 🟢 GREEN | — |
| **HealthMetrics US$5M Series A** | healthmetrics | The Edge Malaysia confirms US$5M Series A | 🟢 GREEN | — |
| WhiteCoat total capital "well below DA's >S$190M" (~US$33–51M) *(analyst est.)* | whitecoat | Round sizes undisclosed since 2021; genuinely not public | ⚪ UNVERIFIABLE | Repo labels it an estimate — correct. |
| ORA **>70% subscription revenue; 250k+ consults; hybrid clinic Feb 2025** | ora-group §8 | Company-reported; not independently auditable | ⚪ UNVERIFIABLE | Private metric. |

*Note on "Hims":* the prompt lists Hims as a cited funding comparator, but no load-bearing Hims figure surfaced in the four executive summaries or the sizing tables audited; if used elsewhere it is a US benchmark, not a decision-relevant Asia round, and was out of scope for this pass.

---

## 5. Digital / penetration

| Figure (as stated in repo) | Repo doc | What search found | Tag | Note / correction |
|---|---|---|---|---|
| MY: **WhatsApp 90.7% monthly reach** (16–64); #1 platform | malaysia-whatsapp-healthcare §2 | DataReportal Digital 2025 Malaysia + secondary confirm 90.7% monthly WhatsApp reach, most-used platform | 🟢 GREEN | — |
| MY: internet **97.7%**; 852 WhatsApp sessions/mo; TikTok #2 | malaysia-whatsapp §2 | Internet ~97.4–97.7% (DataReportal) corroborated; the 852-sessions and TikTok-368 specifics not separately re-pulled | 🟢 GREEN (penetration) / 🟡 AMBER (session counts) | Session-count specifics carry a DataReportal attribution but weren't independently re-verified. |
| SG: **WhatsApp ~84%**; Telegram ~38% | singapore-market-intel §8 | WhatsApp ~84% corroborated (Hashmeta/DataReportal). Telegram: search shows 46.5% among young men; ~38% overall plausible but not directly confirmed | 🟢 GREEN (WhatsApp) / 🟡 AMBER (Telegram 38%) | Telegram overall-reach figure needs a direct DataReportal check. |
| HK: **WhatsApp ~74.7%** | hong-kong-market-intel §9; cross-market §11 | Statista/DataReportal Q2 2025: WhatsApp 74.7% usage in HK | 🟢 GREEN | — |
| DoctorOnCall **1.9M users**, RM15 consults, "20M annual visits" | competitor-comparison; malaysia-telehealth | Corroborated: 1.9M registered users, 500+ GP network, 20M annual visits (web traffic, not consults) | 🟢 GREEN (users) | Repo already flags "20M" as web traffic, not consultations — correct caveat. |

---

## 6. Regulatory & category-timing dates

| Figure (as stated in repo) | Repo doc | What search found | Tag | Note / correction |
|---|---|---|---|---|
| SG: **MaNaDr suspended Aug 2024** (>100k consults ≤1 min in a sampled month; one patient 19 MCs); **licence revoked Dec 2024** | singapore-market-intel §4.6 | MOH newsroom + Mothership + Goody Feed confirm: suspended 16 Aug 2024; >100,000 teleconsults ≤1 min; intended revocation notice 24 Oct 2024; licence revoked effective 20 Dec 2024 | 🟢 GREEN | Precisely corroborated — the flagship SG enforcement fact. |
| SG: **Joint Circular 87/2024 (22 Nov 2024)** — no remote GLP-1 initiation; POM ad wall | singapore-market-intel §4.2 | Referenced across ORA-pivot coverage; full PDF blocked (repo flags this) | 🟡 AMBER | Existence/thrust corroborated; exact clause text unread. Obtain PDF before protocol sign-off. |
| SG: medical trend **12–15.5% (2025), 16.9% projected 2026** | singapore-market-intel §3.3 | WTW 2026 Global Medical Trends: SG 16.9% (2026) vs 15.5% (2025) | 🟢 GREEN | Verbatim match to WTW. |
| SG: rider reform **1 Apr 2026** (co-pay cap doubled to S$6,000) | singapore-market-intel §3.3 | Widely reported IP rider reform effective 1 Apr 2026 | 🟡 AMBER | Widely covered; exact co-pay cap not re-pulled this pass. |
| HK: **A&E fee HK$180 → HK$400, 1 Jan 2026** | hong-kong-market-intel §3.2; hk-exec | HKFP / SCMP / HA gazette confirm A&E HK$180→400 from 1 Jan 2026 (est. +HK$3bn/yr) | 🟢 GREEN | — |
| HK: **first 3-year Action Plan on Weight Management, 4 Mar 2026** (World Obesity Day) | hk-weight-loss-providers §1; hk-exec | HKFP / info.gov.hk / news.gov.hk confirm launch 4 Mar 2026, first-ever 3-year plan | 🟢 GREEN | Govt release cites current ow/ob at 51.3% (see epidemiology currency note). |
| HK: **eHealth+ in force 1 Dec 2025** (EHR Sharing System Amendment Ordinance 2025) | hong-kong-market-intel §3 | Consistent with 2025 eHealth+ commencement coverage | 🟡 AMBER | Directionally confirmed; exact commencement date not independently pinned this pass. |
| HK: medical inflation **~9.8% (2025)**; group premiums **+55% (2021–24)** | hong-kong-market-intel §3.3 | WTW: HK 9.8% (2025); multiple brokers: employee premiums +55% 2021–24 | 🟢 GREEN | — |
| MY: **OOP ~36% of THE; 76% of private financing; private insurance ~17%** | malaysia-market-intel §3 | Malaysia National Health Accounts (via CodeBlue): OOP 76% of private financing, private insurance 17%; public 52.7% / private 47.3% of THE | 🟢 GREEN | Exact MNHA match. |
| MY: **GP fee band RM10–80 (Apr 2026)**, up from RM10–35 frozen since 1992 | malaysia-private-healthcare §4 | Malay Mail / FPMPAM / MMA confirm gazetted RM10–80 effective 2 Apr 2026; prior RM10–35 (MMA 1992 schedule) | 🟢 GREEN | — |
| MY: **tele-MC ban (MMC, 23 Sep 2025)** | malaysia-regulations §3; malaysia-exec | Consistent with MMC 2025 guidance; not independently date-pinned this pass | 🟡 AMBER | High plausibility; confirm the 23 Sep 2025 date at MMC. |
| MY: **48 GLP-1 ad warning letters (2025); 38,055 ads removed 2023–25** | malaysia-regulations §6 | Not independently re-pulled this pass | 🟡 AMBER | Specific enforcement counts; verify with NPRA/MOH before external quotation. |
| SG: **NOVI published outcomes — 708 patients, 12.7% weight loss at 12 mo, 14.7% at 18 mo (IJO 2026, with NUS)** | novi-health §4.3; sg-exec #20; cross-market §14 | **Not found.** Search for NOVI published outcomes returned a *different* study (NOVI Magnum diabetes programme: HbA1c −0.9, weight −5.8% at 3 mo) plus the Novo Nordisk partnership (Jun 2026) and the US$5M raise — but **no independent source for the 708-patient / 12.7%-at-12mo / 14.7%-at-18mo cohort** | 🔴 RED | See RED FLAGS. May be a genuine very-recent IJO 2026 paper not yet search-indexed — but it is load-bearing (1 of only 2 claimed regional outcome studies) and currently uncorroborable. |

---

## The retention question: is it 30% or 38%? — RESOLVED

The repo uses **both** "~30%" and "~38%" for the unmanaged 12-month GLP-1 persistence baseline, and its own key-numbers appendix hedges to "**~30–38%**." Desk verification resolves this cleanly:

- Real-world 1-year semaglutide persistence is **not a single number — it is a fast-rising time series.** Independent sources (peer-reviewed real-world cohorts via PMC; Medscape; HealthVerity) give roughly: **33.2% (2021) → 34.1% (2022) → 39.8% (2023) → 58.6–63% (1H 2024).** A large Danish study likewise found "just over half" discontinue within a year for the older cohorts.
- So **30% ≈ the 2021 cohort and 38% ≈ the 2022–2023 cohort.** Neither is "wrong"; the repo's "~30–38%" band correctly brackets the pre-2024 real-world experience. **Verdict: the range is defensible; do not pick a single point.**
- **But the load-bearing implication is drifting stale.** 2024 initiators already retain ~58–63% at 12 months (shortage resolution + better side-effect management). The strategy's core economic premise — "beat a ~30–38% unmanaged baseline" — is measured against a baseline that is climbing toward the ">60% managed target" on its own. The retention *edge* Welltech can claim over unmanaged care is narrowing. **Action:** re-base the unmanaged assumption to a 2024–25 cohort (~50–60%) in the financial model, or the +10pp-retention value driver is overstated.

Tag on the figure: 🟡 AMBER (range corroborated; premise ageing).

---

## RED FLAGS — do not use until re-researched from primary source

1. 🔴 **NOVI Health "708 patients / 12.7% weight loss at 12 months / 14.7% at 18 months (IJO 2026)."** This is the single most-cited outcome statistic in the Singapore thesis and one of only **two** published outcome studies the entire three-market strategy claims exist (the other being Naluri's). No independent search result corroborates these specific numbers. Independent search *does* confirm NOVI publishes outcomes — but returns a **different** study (the NOVI Magnum diabetes programme: HbA1c −0.9 and weight −5.8% over 3 months), the Novo Nordisk partnership (Jun 2026), and the US$5M raise. Two possibilities: (a) the 708/12.7% cohort is a genuine, just-published IJO 2026 paper not yet indexed in search snippets, or (b) the figures are mis-transcribed / conflated / over-stated. Either way, **stop quoting the 708/12.7%/14.7% figures in any investor or payer material until the IJO 2026 paper is retrieved and the numbers read off the abstract.** This is the #1 primary-source priority.

*No other figure met the RED bar* (no corroboration / direct contradiction / fabrication signature). The items below are AMBER because they are single-sourced, drifting, or advertised-rate — not because they appear invented.

**AMBER items that behave like "soft REDs" (confirm before external quotation):**
- HK Wegovy **~HK$2,700/mo retail** — launch date solid, price uncorroborated; it anchors the "exposes clinic markup" argument.
- Unmanaged GLP-1 retention **~30–38%** — correct for 2021–23, but the premise is going stale (2024 ≈ 60%).
- HK obesity **54.6%** — real, but it is 2020-22 data cited as current, and the govt now headlines 51.3%.
- MY enforcement counts (**48 warning letters / 38,055 ads**), MY **tele-MC ban 23 Sep 2025** date, and SG **Circular 87/2024** clause text — all high-plausibility, none read from primary this pass.

---

## Top 15 to confirm at primary source (priority order)

Priority weighted by (load-bearing-ness × current uncertainty). Primary source in brackets.

1. **NOVI 708-patient / 12.7%@12mo / 14.7%@18mo cohort** — retrieve the *International Journal of Obesity* 2026 paper (or NUS press) and read the numbers. *(RED)*
2. **Unmanaged GLP-1 retention baseline** — re-base the model to 2024–25 real-world persistence (~50–60%), not 30–38%. *(peer-reviewed real-world cohort / claims data)*
3. **HK Wegovy retail price ~HK$2,700/mo** — HK pharmacy / Novo Nordisk HK. *(the markup-exposure argument depends on it)*
4. **SG Joint Circular 87/2024 exact obligations** — HCSA portal PDF (remote-GLP-1-initiation and advertising clauses drive the whole SG compliance design).
5. **MY GLP-1 spend RM400–900M / 35k–70k users (2026)** — no official source exists; commission a distributor/IQVIA read before using in a deck.
6. **All TAM/SAM/SOM bands** (MY RM1.5–3.5B; SG S$10–26m; HK HK$70–200m; regional US$1.4–3.0bn / 30–80m) — these are analyst constructs; label as such in every external use.
7. **GLP-1 distributor margin 15–30%** — actual Zuellig/DKSH/Novo quotes; the unit-economics case rests here.
8. **MY enforcement counts** (48 warning letters; 38,055 ads removed) — NPRA/MOH.
9. **MY tele-MC ban date (23 Sep 2025)** — MMC circular.
10. **HK eHealth+ commencement (1 Dec 2025)** and provider-enrolment mechanics — HK Health Bureau.
11. **HK clinic GLP-1 programme band HK$6,000–11,500/mo** — mystery-shop ≥20 clinics (repo already plans this in the HK Phase-0 roadmap).
12. **NOVI Optimum Plus / ORA / Minmed advertised prices** — manual purchase-flow walkthrough (all behind Cloudflare 403).
13. **HK obesity currency** — reconcile PHS 2020-22 (54.6%) with the 2026 Action Plan's 51.3%; use the correct denominator/definition.
14. **Naluri total funding** — trim any "~US$21M" to the corroborated **~US$19M** (US$5M SA + US$14M SB).
15. **SG rider-reform co-pay cap (S$6,000) and MOH FY2025 budget (+16.3%)** — MOH primary, for the payer-pressure narrative.

---

## Sources seen (corroborating, this pass)

Epidemiology — CodeBlue/Galen Centre NHMS 2023 coverage; NHMS 2023 fact sheet (iku.nih.gov.my); Nature *Scientific Reports* s41598-025-08311-9; MOH Singapore NPHS 2024 newsroom; MOH "War on Diabetes"; HK CHP / HKASO / The Standard (PHS 2020-22); HK C&SD + SCMP (life expectancy 2024); Malay Mail / WHO "Case for Investment" (RM64.2bn NCD).
GLP-1 & dates — Malay Mail / Novo Nordisk (MY Wegovy Jan 2026); MY clinic sources (Mounjaro 30 Aug 2025); HSA "New drug approvals June 2025" (SG Mounjaro); PR Newswire / Novo Nordisk (HK Wegovy 3 Nov 2025); of-noah.sg / MIMS (SG Wegovy 2023 approval); PMC real-world persistence cohorts / Medscape / HealthVerity / boli.care (GLP-1 retention curve).
Funding — Monk's Hill Ventures + MobiHealthNews (NOVI US$5M); TechCrunch / DealStreetAsia / Forbes / TechNode (ORA US$10M/US$17M+); PR Newswire / DA blog / The Edge (DA S$88M/S$140M+); DealStreetAsia / DNA / TechNode (Naluri 1M lives, US$14M Series B); Sun Life / Bowtie (US$70M); The Edge Malaysia (HealthMetrics US$5M).
Penetration — DataReportal Digital 2025 Malaysia; Hashmeta / DataReportal (SG WhatsApp ~84%); Statista/DataReportal Q2 2025 (HK WhatsApp 74.7%); DoctorOnCall about-us / Vulcan Post.
Regulatory — MOH Singapore newsroom + Mothership + Goody Feed (MaNaDr); WTW 2026 Global Medical Trends (SG 16.9%, HK 9.8%); HKFP / SCMP / HA gazette (A&E HK$400, 1 Jan 2026); HKFP / info.gov.hk / news.gov.hk (HK Action Plan 4 Mar 2026); CodeBlue (MY MNHA OOP 76%); Malay Mail / FPMPAM / MMA (MY GP fee RM10–80, 2 Apr 2026); Grand View Research (MY telemedicine USD 1.85B).

*URLs are recorded in the WebSearch trace for this pass; per methodology, none was read as a full primary-source page — corroboration is snippet-grade and raises confidence by agreement, not by primary reading.*
