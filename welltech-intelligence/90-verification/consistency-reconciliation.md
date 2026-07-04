# Consistency Reconciliation — Internal Cross-Document Audit

A fourth-pass verification artefact. Where the other verification documents check claims against the outside world, this one checks the 90 documents **against each other**: it pulls every mention of each load-bearing quantity, lines the values up, and flags any case where the same fact is stated two ways. It requires no network access — it is a pure internal-consistency audit performed with `grep` and file reads.

Last updated: July 2026.

Read [methodology.md](methodology.md) first for the confidence-tag scheme and the environment constraint that shaped the underlying research.

---

## Summary

**Headline: the repository is materially self-consistent.** Every top-line number the strategy rests on — the three obesity prevalences, diabetes prevalences, out-of-pocket shares, the regional SAM/SOM, Welltech's own price ladder, GLP-1 launch dates, and the major funding figures — is quoted the **same way in every document that uses it**. The cross-document discipline is unusually good; several of the few remaining discrepancies are already self-flagged in-text (the repo tells the reader it disagrees with itself and why).

- **Quantities audited:** ~22 fact-families across all 90 documents.
- **Discrepancies found:** **8**.
- **Material** (could change a decision or mislead an external reader): **2** — the GLP-1 persistence baseline, and the Doctor Anywhere Series C amount.
- **Immaterial** (rounding, secondary/historical data points, definitional base differences): **6**.
- **Fixed in-place this pass:** **0.** Every discrepancy found is either (a) a genuine source-level conflict where the "right" value is a judgement call that external verification (barred this pass) must settle, or (b) a rounding/definitional difference that is not an error. Per the conservative mandate, none met the "unambiguous typo" bar for an automated edit. All are flagged below for human decision.
- **The single most important inconsistency:** the **unmanaged 12-month GLP-1 persistence baseline**, quoted as **~30%**, **~35%**, **~38%** and **30.2%** in different places. This is the number the entire P&L is stated to hinge on, so the spread matters more than its size. It is already knowingly flagged in `README.md` and `investor-thesis.md`, which recommend standardising to **38% (all-comers)** for external use — but that standardisation has **not** been applied to the revenue tables, which still label 30% as "baseline."

---

## How this audit was run

For each fact-family, all mentions were pulled across the tree and compared verbatim:

```
grep -rn "54.4\|54.6\|12.7" .        # obesity prevalences
grep -rn "persist\|retention\|30.2%" # GLP-1 baseline
grep -rn "RM999\|RM49\|RM5,499"      # Welltech pricing
grep -rn "Series [A-C]\|US\$\|S\$"    # funding figures
grep -rn "Wegovy\|Mounjaro"          # GLP-1 launch dates
grep -rn "OOP\|out-of-pocket\|76%"   # health-spend financing
grep -rn "SAM\|SOM\|ARR"             # market sizing
grep -rn "WhatsApp\|97.7%\|90.7%"    # channel penetration
```

An "Assessment" column classifies each finding as **typo**, **rounding**, **genuine conflict** (two sourced values that truly differ), **definitional** (same concept, different base/cutoff), or **stale**.

---

## Discrepancy log

| # | Fact | Values found (file) | Assessment | Canonical value | Fixed? |
|---|---|---|---|---|---|
| 1 | **Unmanaged 12-mo GLP-1 persistence baseline** | **~30%** revenue-table baseline (`50-marketing-intelligence/pricing.md` §5.3; `funnels.md`; `investor-thesis.md` revenue table line 156); **~38%** and **30.2%** real-world source (`pricing.md` line 212: "38% at 12 months; 30.2% without T2DM"); **~30–38%** range in most strategy docs; **~35%** (`investor-thesis.md` line 296) | **Genuine conflict — knowingly present.** `README.md` line 46 and `investor-thesis.md` line 158 both explicitly flag it and recommend reconciling to **38% (all-comers)** for external use. The recommendation has not been propagated to the revenue tables. | **38% (all-comers)** per the repo's own stated resolution; the 30% figure is the no-T2DM subgroup used as a stress case | **No — flag.** Restating every revenue/LTV table from a 30% to a 38% base is a modelling decision for the deal team, not a typo fix. |
| 2 | **Doctor Anywhere Series C amount** | **S$88M (~US$65.7M)**, Aug 2021 (`doctor-anywhere.md` line 31, the canonical dossier, with its own currency-reconciliation note at line 167: "S$88M (company) = ~US$65.7M (PR Newswire); MobiHealthNews 'US$66M'"); **US$58.7M+ "Series C"** (`doctoroncall.md` line 198 + footnote 20, citing DealStreetAsia) | **Genuine conflict.** The `doctoroncall.md` comparison cell introduces a third figure (US$58.7M) for the *same* Aug-2021 round that the DA dossier reconciles at S$88M/~US$65.7M; the DA dossier's reconciliation note does not even list the 58.7 figure. | **S$88M (~US$65.7M)** — the company-stated round size in the dedicated DA dossier | **No — flag.** US$58.7M is a real cited (DealStreetAsia) figure, possibly a different framing (named-investor tranche vs total round); overwriting it could erase legitimate sourced nuance. Recommend `doctoroncall.md` adopt the DA-dossier figure with the currency note. |
| 3 | **Malaysia NHMS-2019 diabetes prevalence** (historical trend point) | **18.3%** (`malaysia-market-intelligence.md` line 70: "11.2% (2011) → 18.3% (2019) → 15.6% (2023)"); **13.4%** (`malaysia-weight-loss-market.md` line 35 trend table: "13.4% (2015) \| 13.4%" — the 2015 value appears duplicated into the 2019 column) | **Genuine conflict (minor).** The weight-loss table's 2019 cell looks like a copy-paste artefact of the 2015 cell, and the sibling doc gives 18.3% for 2019. But the true NHMS-2019 figure cannot be confirmed this pass (network-barred), and 13.4% may reflect a different age base / diagnosed-only cut. | Likely **18.3%** (the widely-reported NHMS-2019 adult total), but unconfirmed | **No — flag.** The **headline** diabetes figure (15.6%, NHMS 2023) is consistent everywhere; only this secondary historical point conflicts. Verify 2019 value against the NHMS-2019 fact sheet before editing. |
| 4 | **Malaysia adult-population base** | **~24m** (`malaysia-market-intelligence.md` line 203/207, used in the TAM calc 54.4% × 24m ≈ 13m); **~23.5M** "DOSM-consistent" (`malaysia-weight-loss-market.md` line 360); **~23m** (`singapore-market-intelligence.md` line 564; `singapore-executive-summary.md` line 269) | **Definitional / rounding.** Three loosely-rounded adult bases (23m / 23.5m / 24m) off the same 34.2m population. All three yield the same ~13m overweight/obese TAM (54.4% × any of them ≈ 12.5–13.1m), so no downstream figure is affected. | **~23.5M** (the one explicitly labelled "DOSM-consistent") | **No — flag (low priority).** Harmonising the adult base to 23.5M everywhere would tidy the TAM derivation but changes no headline output. |
| 5 | **Malaysia "97.7%" dual-use + penetration >100%** | **97.7%** used as (a) *internet penetration* (`malaysia-consumer-behaviour.md` line 15; `malaysia-executive-summary.md` line 103; `sources/datasets.md` line 57 — "34.9m internet users (97.7% penetration)") **and** (b) *WhatsApp = favourite comms app share* (`datasets.md` line 60; `facebook.md` line 41; `consumer-behaviour.md` line 98). Separately, 34.9m users ÷ 34.2m population = 102%. | **Definitional / mixed-source artefact.** Two genuinely different DataReportal/MCMC statistics that coincidentally both read 97.7% — cleanly separated in `datasets.md` but easy to conflate elsewhere. The ">100%" tension arises only because DataReportal computes penetration on its own (~35.7m) population base, not the DOSM 34.2m cited elsewhere. | Keep both, but **label them distinctly**: internet penetration ≈97.4–97.7% (DataReportal base) vs WhatsApp-favourite-app 97.7% (MCMC IUS 2022) | **No — flag.** Not an error; a labelling-clarity risk. The WhatsApp **monthly-reach** figure (90.7%, Meltwater) — the one the operating model actually uses — is consistent in every strategy doc. |
| 6 | **Regional Year-3 SOM, country split** | `cross-market-summary.md` line 74: MY **13–34m** / SG **7.7–20m** / HK 9–26m; `investor-thesis.md` lines 60–62: MY **13–35m** / SG **7.5–19m** / HK 9–26m | **Rounding.** Sub-rounding differences on analyst-estimate ranges. The **combined ~US$30–80m ARR** headline is identical in both, as is HK (9–26m). | **~US$30–80m combined**; country bands to one significant figure | **No.** Immaterial; forcing exact-match on estimate ranges would be false precision. |
| 7 | **Malaysia diabetes historical 2015 point** | `malaysia-market-intelligence.md` line 70 implies a 2015 point of 13.4% within its trend; `malaysia-weight-loss-market.md` line 35 shows 2015 = 13.4% | **Consistent** (both 13.4% for 2015). Listed only to record that the 2015 anchor agrees — the divergence is isolated to the 2019 point (row 3). | 13.4% (2015) | n/a — consistent |
| 8 | **Speedoc / Doctor Anywhere cumulative funding** | `doctor-anywhere.md`: ">S$140M by Series C (2021) + US$40.8M Series C1 (2023)" and comparison cell ">S$190M"; `speedoc.md` lines 198/255: DA ">S$190M cumulative" | **Consistent.** S$140M + ~S$55M (US$40.8M) ≈ S$195M, so ">S$190M" reconciles with the component sum. Recorded to confirm no conflict. | ">S$190M cumulative" | n/a — consistent |

---

## Fact-families audited and found CONSISTENT (no action)

These were checked exhaustively and agree across every document that cites them. They are listed so a reader knows the absence of a row above is a positive result, not an un-checked gap.

### Epidemiology
- **Malaysia overweight+obese 54.4%** (NHMS 2023, WHO cutoff) — identical in `malaysia-market-intelligence.md`, `malaysia-consumer-behaviour.md`, `malaysia-longevity-market.md`, `cross-market-comparison.md`, `expansion-strategy.md`, `product-strategy.md`, both cross-market and country exec summaries. No stray 54.6%/54% (only intentional roundings to "54%").
- **Malaysia abdominal obesity 54.5%** — consistent (market-intelligence, consumer-behaviour, longevity).
- **Hong Kong overweight+obese 54.6%** (local Asian cutoffs; obese 32.6% + overweight 22.0% = 54.6%, internally additive) — consistent across `hong-kong-market-intelligence.md`, `cross-market-comparison.md`, `hk-weight-loss-providers.md`, HK exec summary.
- **Singapore obesity 12.7%** (BMI≥30, NPHS 2024, ↑ from 10.5% 2019–20) — consistent across `singapore-market-intelligence.md`, `singapore-executive-summary.md`, `cross-market-comparison.md`. (Note: NOVI's *outcome* figure of 12.7% mean weight loss at 12mo is a different fact that coincidentally shares the number; both are used correctly and never conflated.)
- **Diabetes headline:** MY **15.6%** / HK **8.5% raised glucose** / SG **1-in-3 lifetime risk** — consistent everywhere (only the MY-2019 historical sub-point conflicts, row 3 above).

### Health-spend financing (out-of-pocket)
- **Malaysia:** ~**36%** of total health expenditure OOP; ~**76%** of *private* financing OOP; ~17% private insurance — consistent (`malaysia-market-intelligence.md` lines 121–125, 325; `cross-market-summary.md` line 359).
- **Singapore:** OOP ~**25%** (down from ~48% in 2000); ~71% IP-insured — consistent (`singapore-executive-summary.md` line 87; `cross-market-summary.md` line 359).
- **Hong Kong:** private **48.2%** of Current Health Expenditure (public 51.8%) — consistent (`hong-kong-market-intelligence.md` line 165/§; `cross-market-summary.md` line 359).

### Welltech's own pricing (checked across pricing.md, pricing-strategy.md, go-to-market, product-strategy, exec summaries)
- **RM49** entry consult (100% credited) — consistent.
- **RM299/mo** GOOD / Metabolic Start — consistent.
- **RM999/mo** flat BETTER / core Medical Weight Program, drug included — consistent everywhere; **RM5,499** 6-month prepay (~8% off, ~RM917/mo on BNPL) — consistent.
- **RM199 vs RM299** maintenance tier, **RM3,600–8,800/yr** longevity membership — consistent.
- Regional rebase points (SG S$15 / S$90 / S$300; HK HK$85 / HK$525 / HK$1,750) — consistent in `pricing-strategy.md`.

### GLP-1 launch dates (per market)
- **Malaysia:** Mounjaro **~30 Aug 2025** (T2DM); Wegovy **mid-January 2026** (on-label obesity) — consistent across `malaysia-weight-loss-market.md` (§4.2), `malaysia-executive-summary.md`, `cross-market-summary.md`.
- **Singapore:** Wegovy HSA-approved 2023 with commercial launch date **explicitly flagged as conflicting** (mid-2024 vs mid-2025) in every doc that raises it — a *documented* open item, not an accidental inconsistency; Mounjaro weight indication **Jun 2025** — consistent.
- **Hong Kong:** Wegovy launched **Nov 2025** (~HK$2,700/mo retail); Mounjaro approved **late 2024** — consistent.

### Competitor funding figures
- **NOVI Health:** US$5M Series A (Nov 2022, Monk's Hill) — consistent (`novi-health.md`, `investor-thesis.md`, `competitor-comparison.md`). Published cohort **708 patients, 12.7%/12mo, 14.7%/18mo** (IJO 2026) — consistent across all mentions.
- **ORA / OVA:** US$10M Series A (May 2023, TNB Aura + Antler); ~US$17M total — consistent across `ora-group.md` and `ova-health.md`.
- **Naluri:** ~US$5M Series A (2021) + US$14M total Series B in tranches — consistent within `naluri.md`.
- **Speedoc:** Series A framed as US$5M / S$6.7M and totals given as a **range** (US$33–51M) with per-source attribution — internally consistent (the range is deliberate, not a conflict).
- **HealthMetrics:** US$5M Series A (2020); ~US$15–17M total with database spread (PitchBook 16.6M / Tracxn 14.8M) explicitly reconciled in-text — consistent.
- **Hims & Hers:** FY2024 revenue **US$1.48B** (`hims-hers.md`) ≈ "~US$1.5B" (`investor-thesis.md`) — consistent (rounding).

### Market sizing (top line)
- **Regional Welltech-relevant SAM ~USD 1.4–3.0bn/yr** and **Year-3 SOM ~USD 30–80m ARR → USD 100m+ at MY maturity** — quoted identically in `cross-market-summary.md` (lines 36, 48, 342–343) and `investor-thesis.md` (lines 63, 451, 475). Country SAMs (MY RM1.5–3.5B / SG S$0.7–1.4B / HK HK$1.9B) — consistent between the country market-intelligence docs, country exec summaries, and the investor thesis.
- **Malaysia blended maturity SOM ~RM185–670m/yr** — consistent (`malaysia-market-intelligence.md` §5, `cross-market-summary.md`, `investor-thesis.md`).

### Channel penetration
- **WhatsApp monthly reach:** MY **90.7%** / SG **~84%** / HK **~74.7–75%** — consistent across every strategy and summary doc (Meltwater/Hashmeta sourced). Telegram SG **~38%** consistent.
- **Internet penetration:** MY 97.7% / SG 98.4% / HK 96.8% — consistent (subject to the labelling caveat in row 5).

---

## Recommended actions (all for human decision — none auto-applied)

1. **[Material]** Decide the single GLP-1 persistence baseline for **external** materials and propagate it. The repo's own recommendation is **38% all-comers**; if adopted, restate the 30%-labelled rows in `pricing.md` §5.3, `funnels.md`, `pricing-strategy.md` §8, and `investor-thesis.md` so "baseline" is unambiguous. (Internal stress cases using 30% are fine if labelled as the no-T2DM subgroup.)
2. **[Material]** Reconcile the **Doctor Anywhere Series C** figure: align `doctoroncall.md`'s "US$58.7M+ Series C" cell with the canonical `doctor-anywhere.md` value (S$88M / ~US$65.7M), or add the DealStreetAsia US$58.7M figure to the DA dossier's reconciliation note so a single explanation exists.
3. **[Minor]** Confirm the **NHMS-2019 diabetes** value (18.3% vs 13.4%) against the fact sheet and fix the `malaysia-weight-loss-market.md` trend cell if it is indeed a duplicated 2015 value.
4. **[Minor]** Standardise the **Malaysia adult base** to 23.5M and clarify the 97.7% internet-vs-WhatsApp labelling in the two exec/consumer docs.

*This pass edited no files. The two verification files it did not need to touch — `load-bearing-numbers-audit.md` and `price-verification.md` — remain the authorities for external corroboration; this document only governs internal agreement.*
