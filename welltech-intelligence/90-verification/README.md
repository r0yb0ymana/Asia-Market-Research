# 90 — Verification

A second-pass verification of the repository's factual claims and the construction of the financial model. Read [methodology.md](methodology.md) first — it states the environment constraint (primary-source pages are egress-blocked in this environment, so this pass verifies by **multi-source search corroboration**, not by reading source PDFs) and the confidence-tag scheme (🟢 / 🟡 / 🔴 / ⚪).

Last updated: July 2026.

## What was checked, and how it came out

| Workstream | Document | Items | Result |
|---|---|---|---|
| Load-bearing numbers | [load-bearing-numbers-audit.md](load-bearing-numbers-audit.md) | 53 | 🟢 34 · 🟡 10 · 🔴 1 · ⚪ 8 |
| Competitor prices | [price-verification.md](price-verification.md) | 45 | 🟢 17 · 🟡 17 · 🔴 0 · ⚪ 11 |
| Regulatory instruments | [regulatory-verification.md](regulatory-verification.md) | 34 | 🟢 24 · 🟡 8 · 🔴 0 · ⚪ 2 |
| Cross-document consistency | [consistency-reconciliation.md](consistency-reconciliation.md) | 90 docs | 8 discrepancies (2 material), 0 fabrications |
| Financial model | [../70-welltech-blueprint/financial-model.md](../70-welltech-blueprint/financial-model.md) | — | Built; retention is the #1 sensitivity |

**Aggregate across the three tagged workstreams (132 discrete claims): 🟢 75 (57%) · 🟡 35 (27%) · 🔴 1 (<1%) · ⚪ 21 (16%).**

## The headline

The repository's *facts hold up unusually well.* Epidemiology, GLP-1 launch dates, regulator actions and dates, payer figures, digital-penetration figures, and every decision-relevant funding round corroborated cleanly. No fabricated instruments or prices were found; the one 🔴 is a single (important) outcome statistic, and the internal-consistency audit found the 90 documents quote the same facts consistently across market-intelligence, executive-summary, and blueprint layers. The soft spots are concentrated and known: analyst-estimated market sizing (correctly labelled), transaction-gated competitor prices (opacity that is itself a finding), and a handful of dates worth a manufacturer confirmation.

## The things that must be resolved before external use

1. 🔴 **The NOVI Health outcome study** ("708 patients, 12.7% weight loss at 12 months, 14.7% at 18 months, IJO 2026") — the single most-cited outcome claim in the competitive thesis — **could not be independently corroborated.** A *different* NOVI study (Magnum diabetes) was found instead. Do not quote the 708/12.7% figures externally until the paper is pulled. See load-bearing-numbers-audit.md §RED FLAGS.
2. 🟡 **The unmanaged GLP-1 retention baseline is drifting stale.** 30% and 38% are both defensible historical points, but 2024 initiators already retain ~60% unmanaged — which, if true, materially weakens the "+10pp retention = RM900–1,000/patient" value driver. The financial model exposes this as the #1 sensitivity; the baseline should be re-based (~50–60%) or the moat maths re-argued. See consistency-reconciliation.md and financial-model.md.
3. 🟡 **Wegovy launch dates.** Malaysia ("Jan 2026" in the repo vs Jan 2025 availability / 2023 approval in search) and Singapore both need direct confirmation from Novo Nordisk before anchoring the "market-formation moment" narrative.
4. 🟡 **Two HK price anchors** — Wegovy ~HK$2,700/mo retail, and hospital Wegovy programs (HKSH HK$9,500–12,500) trace to a single buyer's-guide aggregator. Confirm by direct provider quote before they anchor the "clinic markup" argument.
5. **Legal sign-off** (regulatory-verification.md §"Requires healthcare-lawyer sign-off"): e-prescription validity for Group B poisons in Malaysia; virtual-clinic licensability (MY forbearance + HK PHFO grey zone); GLP-1 advertising/influencer clearance; cross-border prescribing; PDPA/PDPO cross-border transfer.
6. **Clinical sign-off** (regulatory-verification.md §"Requires medical-director sign-off"): GLP-1 titration schedules against *current* product labels (the repo cites a clinic blog, not the label); the red-flag/stop-rule escalation matrix and its SLAs; peri-operative GLP-1 hold; BMI initiation threshold + contraindication screen; the SaMD human-review gate on any titration engine.

## What still requires field/primary research (not doable from the desk)

- Primary confirmation of any 🟢 figure before a financing, filing, or pricing commitment (search corroboration ≠ diligence grade).
- A **mystery-shop / enquiry pass** on the 11 transaction-gated ⚪ prices (aesthetic-clinic programs, hospital screening, HK hospital Wegovy quotes, storefront ladders).
- The financial model's ⚪ inputs — drug-distributor terms, SG/HK willingness-to-pay, and the retention *level* — need primary validation before the model informs a round.

## Corrections applied

- No in-place figure edits were made: the consistency pass found no unambiguous typo, and every flagged discrepancy is either a sourced reporting difference (e.g. Doctor Anywhere's round reported as S$88M vs US$58.7M — the same raise) or a modelling judgement call left for the deal team. Conservative-by-design: flag, don't silently overwrite.
- Naluri total funding noted as ~US$19M (US$5M A + US$14M B), a minor correction to a brief reference.
