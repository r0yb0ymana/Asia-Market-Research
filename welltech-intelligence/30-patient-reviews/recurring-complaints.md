# Recurring Complaint Taxonomy — Malaysian Digital Health & Private Healthcare

**Abstract.** This document classifies the complaints that recur across Malaysian telehealth platforms, pharmacies, weight-loss/slimming operators and private hospitals into nine themes, each with provider-level evidence, characteristic patterns, and a frequency signal. It closes with a severity × frequency matrix and an exploitation map for Welltech. Evidence derives from the review research documented in [review-analysis.md](review-analysis.md) (methodology and limitations in §1 there); emotional interpretation is in [sentiment-analysis.md](sentiment-analysis.md); raw scores in [review-score-comparison.md](review-score-comparison.md).

Last updated: July 2026

---

## 0. How to read frequency and severity

- **Frequency signal** is a qualitative triangulation: how many independent platforms/providers the theme appears on, and whether it recurs across years. Remote research cannot produce true complaint counts for most providers (no scrapeable corpora; see limitations in [review-analysis.md](review-analysis.md) §1.2).
- **Severity** is graded by consumer harm: A = financial/clinical harm (lost thousands of ringgit, wrong medication), B = care denied or materially degraded, C = friction/annoyance.

**Theme index:** T1 pricing opacity · T2 communication failure · T3 prescription/medication · T4 delivery/logistics · T5 refunds · T6 waiting times · T7 hard sell · T8 doctor quality/rushed consults · T9 app/tech failures. Interactions in §10.1; root causes in §10.2; frequency summary in §12; anticipated new classes in §14.

---

## 1. Theme T1 — Pricing opacity & bill shock

**Definition.** Prices unknowable before commitment; charges appearing after service; final bills late or unexplained.

| Provider class | Pattern | Evidence |
|---|---|---|
| Gleneagles KL | "Too many hidden charges"; final bill released >10 days post-discharge | iBanding/Wupdoc review corpus[^1][^2] |
| Pantai KL | Bill exceeding RM700 with RM250 for a 10-minute specialist consult described as shock; billing office slow, complicating claims | Google-review roundups via aggregators[^3][^4] |
| Prince Court | Repeated payment/insurance questioning by multiple staff; specialist prices "almost double" other centres | Trustburn/Wupdoc/Foursquare corpus[^5][^6] |
| Doctor Anywhere | Medication priced well above retail pharmacy, discovered only at checkout | App Store review themes[^7] |
| Slimming centres | Package prices misrepresented; scope of package undisclosed until signed | ComplaintsBoard, sgforums[^8][^9] |

**Frequency signal:** appears on every hospital brand studied and the largest telehealth app — the most universal theme in the corpus. **Severity B** (A at slimming centres).

## 2. Theme T2 — Communication failures & unresponsive support

| Provider class | Pattern | Evidence |
|---|---|---|
| Doctor Anywhere | Tickets unanswered "after days of waiting"; "no communication or effort made to fix the problem"; still cited in Sep 2025 reviews | App Store / Play reviews[^7][^10] |
| DoctorOnCall | Unresponsive "virtual assistants"; unanswered follow-up emails | App review corpus per dossier, corroborated this cycle[^11] |
| Speedoc | Customer service unreachable after a wrong-medication delivery | Top-Rated.Online KL reviews[^12] |
| Sunway Velocity | Families without updates during surgery; labour-room understaffing at critical moments | Aggregated reviews[^13] |
| Pantai KL | Billing phone calls go unanswered | Aggregator corpus[^3] |

**Frequency signal:** cross-cutting; the default failure mode once anything goes wrong. **Severity B.**

## 3. Theme T3 — Prescription & medication issues

| Provider class | Pattern | Evidence |
|---|---|---|
| Doctor Anywhere | No prescription-letter option even for chronic hypertension — patients feel forced to buy marked-up meds on-platform | App Store reviews[^7] |
| Speedoc | Medication sent wrongly (isolated but severe) | Top-Rated.Online[^12] |
| Prince Court | Doctor insisted on ~USD200 Malarone over requested cheap doxycycline | Review corpus[^5] |
| E-marketplace sellers | 93.4% of prescription medicines sold on Malaysian e-marketplaces not registered with the Drug Control Authority; >90% of illegal online pharmacies supply POMs without prescription | MJPharm study; MOH advisories[^14][^15] |
| Slimming/beauty adjacents | Unregistered products and adulteration risk fuel authenticity anxiety | MOH Pharmaceutical Services warnings[^15][^16] |

**Frequency signal:** structural at DA; environmental (category-wide fear) for all online medicine. **Severity A** where wrong/unregistered products are involved; B for margin capture.

## 4. Theme T4 — Delivery & logistics failures

| Provider class | Pattern | Evidence |
|---|---|---|
| DoctorOnCall | Multi-day to 15-day order delays vs same-day marketing; praise when it works ("arrived in just 2 days") | App reviews and store listing[^11][^17] |
| Doctor Anywhere | Delivery delays cited alongside CS unresponsiveness (Sep 2025 review) | Play corpus[^10] |
| Doctor2U | Delivery flow generally respected (3h Klang Valley); complaints centre on app UX not logistics | AppGrooves review aggregation[^18] |
| Speedoc | Mostly praised (30-min medication runs) with a severe wrong-item tail | Reviews[^12][^19] |

**Frequency signal:** dominant complaint class for DoctorOnCall specifically; episodic elsewhere. **Severity B.**

## 5. Theme T5 — Refund & service-recovery failures

| Provider class | Pattern | Evidence |
|---|---|---|
| Gleneagles KL | Refund unresolved for 4 months | Review corpus[^1][^2] |
| London Weight Management | Refunds contractually limited to RM28 treatment fee, same-day request only; refusal then "negotiate a different package" | Refund-policy reporting and complaints[^8][^20] |
| Marie France Bodyline | Contested tribunal jurisdiction rather than refund (argued it was "healthcare services"); court rejected | IIUM consumer-law case notes[^21] |
| Prince Court | Refund desk flagged as the weak link for self-pay | Review corpus[^5] |
| DoctorOnCall | Return/refund policy exists; anecdotes centre on slow resolution | Dossier corpus corroborated[^11] |

**Frequency signal:** every provider that takes prepayment shows this theme. **Severity A at slimming centres** (four-figure packages), B elsewhere.

## 6. Theme T6 — Waiting times & queue integrity

| Provider class | Pattern | Evidence |
|---|---|---|
| KPJ flagships | ~3h emergency waits; GL counters single-staffed (1–2h); insurance verification up to ~5h | iBanding/PissedConsumer + KPJ's own disclosures[^22][^23][^24] |
| Pantai KL | 3h admission with approved GL; ~5h imaging round-trip; ~5h mammogram+consult day | Aggregator corpus[^3][^4] |
| Gleneagles KL | >6h intake-to-bed; A&E ~2h; discharge >3h | iBanding/Wupdoc[^1][^2] |
| Prince Court | 6–7h screening days; 1.5h queue for a simple test; VIP queue-cutting resented | Trustburn/Foursquare[^5][^6] |
| Sunway City | Appointment holders not prioritised; files misdelivered causing waits | iBanding + review corpus[^13][^25] |
| Doctor Anywhere | 15–20 min matching waits; doctor no-shows on scheduled slots | App Store reviews[^7] |

**Frequency signal:** the single most-mentioned hospital theme across all five brands; telehealth's equivalent is queue-for-a-doctor. **Severity C–B** (B when appointments/GLs are effectively voided).

## 7. Theme T7 — Hard-sell & predatory sales tactics

| Provider class | Pattern | Evidence |
|---|---|---|
| London Weight Management | Free-trial-to-hard-sell funnel; "very pushy" consultants; body-shaming to close ("ridiculed me with my body size"); guilt scripts about savings/deposits | ComplaintsBoard, sgforums, blogs[^8][^9][^20][^26] |
| Marie France / Dorra | Same funnel design; "sales assistants lied"; scale-integrity allegations at LWM | Blog/complaint corpus[^21][^27][^28] |
| Sector aggregate | 6,925 NCCC complaints against wellness/aesthetic centres (2015–2017); ~10 women lost >RM2M combined; TTPM handled 9,203 claims worth RM77.2M in 2025 YTD (all sectors) | NCCC/FOMCA, KPDN[^29][^30] |
| Pharmacy retail (watch item) | Employee reviews cite unrealistic KPIs/sales targets at Alpro — the pre-condition for counter-level upselling, though patient-side complaints are not yet visible | Glassdoor[^31] |

**Frequency signal:** concentrated but intense — defines the weight-loss category's public record. **Severity A.**

## 8. Theme T8 — Doctor quality & rushed consults

| Provider class | Pattern | Evidence |
|---|---|---|
| KPJ | Consultations under 2 minutes; results not walked through | Review corpus per dossier, corroborated[^22] |
| Doctor Anywhere | Video consults under 3 minutes; feels like a prescription vending transaction | App Store reviews[^7] |
| Pantai KL | 10-minute specialist consult at RM250 read as rushed for the price | Aggregators[^3] |
| Speedoc | One severe clinical-competence complaint (feeding-tube insertion by inexperienced MA) | Top-Rated.Online[^12] |
| Counterweight | Doctors/nursing are the most-praised element at Sunway, Prince Court, Gleneagles; complaints target process, not competence | Multiple corpora[^5][^13] |

**Frequency signal:** recurrent but secondary; Malaysians largely trust clinicians. **Severity B.**

## 9. Theme T9 — App & tech failures

| Provider class | Pattern | Evidence |
|---|---|---|
| Naluri | Crashes, blinking UI, disappearing keyboard — breaks the core chat loop; improvement noted in recent versions | Play reviews[^32][^33] |
| Doctor Anywhere | App-breaking bugs; charges taken despite UI errors | Play/App Store corpus[^7][^10] |
| Doctor2U | Forced app install to obtain medical reports; counter-intuitive UI | AppGrooves[^18] |
| DoctorOnCall | Web-first, fragmented low-download apps (26k installs, no aggregate rating) — weak owned-app surface rather than buggy one | AppBrain[^17] |

**Frequency signal:** universal for app-first providers; absent only where there is no app to fail. **Severity C** (B when payment is captured through a failing UI).

---

## 10. Severity × frequency matrix

| | **Low frequency** | **Medium frequency** | **High frequency** |
|---|---|---|---|
| **Severity A** (financial/clinical harm) | Wrong medication delivered (Speedoc); unregistered e-marketplace medicines (category)[^12][^14] | Slimming-centre hard-sell + refund refusal (LWM, Marie France)[^8][^21] | — |
| **Severity B** (care denied/degraded) | Clinical-competence lapses in home care[^12] | Prescription lock-in & med markups (DA)[^7]; refund delays (Gleneagles, PCMC)[^1][^5]; delivery failure (DoctorOnCall)[^11] | Support black holes after failure (DA, DoC, Speedoc)[^7][^11][^12]; GL/billing friction (all hospitals)[^1][^3][^22] |
| **Severity C** (friction) | App-store payment glitches[^7] | App bugs (Naluri, Doctor2U)[^18][^32] | Waiting times & queue integrity (all five hospital brands; telehealth matching waits)[^1][^3][^5][^13][^22] |

**Reading.** The high-frequency column is dominated by *operations* (queues, GLs, support), not medicine. The severity-A cell that matters strategically is slimming-centre conduct: it is the reputational landmine adjacent to Welltech's weight-loss category. The emptiest quadrant — high-frequency, severity-A — stays empty only because regulators and media police it; any entrant that drifts toward package-prepayment + weak refunds would fill it.

## 10.1 Theme interactions — how complaints compound

Complaints rarely arrive alone; the corpus shows characteristic chains. Understanding the chains matters more than the individual themes because the *second* failure is what converts a private annoyance into a public one-star review.

| Chain | Mechanism | Observed at |
|---|---|---|
| T4 → T2 → T5 | Delivery fails → support goes silent → refund stalls → patient posts publicly | DoctorOnCall, Doctor Anywhere[^7][^11] |
| T6 → T1 | Long GL/queue wait primes the patient → any billing surprise afterwards reads as exploitation | Pantai, KPJ, Gleneagles[^1][^3][^22] |
| T8 → T3 | Rushed consult (<3 min) → prescription decision feels sales-driven, not clinical | Doctor Anywhere, Prince Court[^5][^7] |
| T7 → T5 | Hard-sold package → buyer's remorse → refund refused by policy → tribunal/complaint board | LWM, Marie France[^8][^21] |
| T9 → T2 | App bug captures payment or blocks access → support cannot be reached in-app | Doctor Anywhere, Naluri[^7][^32] |

Design consequence: breaking any chain at link two (communication) suppresses most public complaints even when link one (the operational failure) still occurs. This is the cheapest complaint-management investment available to Welltech.

## 10.2 Root-cause classification *(analysis)*

| Root cause class | Themes it drives | Fixable by an entrant? |
|---|---|---|
| Margin architecture (medication markup as revenue engine) | T1, T3 | Yes — choose consult/programme revenue instead of dispensing spread |
| Understaffed exception-handling (tickets, GL counters, refunds) | T2, T5, T6 | Yes — AI-assisted ops + WhatsApp async absorb exception load cheaply |
| Incentive design (commissioned consultants, counter KPIs) | T7 | Yes — structural, not cultural: remove commissions from clinical roles |
| Throughput economics (consult-per-hour targets) | T8 | Partially — telehealth economics permit longer async touch at same cost |
| Under-invested consumer software | T9 | Yes — WhatsApp-first sidesteps the app-quality battle entirely |
| Regulatory vacuum (no OHS telemedicine rules; illegal e-pharmacies) | T3 ambient fear | No — but visible over-compliance converts the vacuum into advantage |

## 11. Exploitation map for Welltech

| Theme | Incumbent failure | Welltech counter-position (product requirement, not slogan) |
|---|---|---|
| T1 | Checkout-stage price reveals; late bills | All-in quoted price before booking; itemised digital bill at discharge/close of consult |
| T2 | Ticket black holes | WhatsApp-native support with response-time SLA visible to the patient |
| T3 | Rx lock-in (DA) | Prescription letter issued by default; buy-anywhere explicitly allowed |
| T4 | Same-day promises, 15-day reality (DoC) | Delivery promise = tracked commitment; proactive delay notification |
| T5 | 4-month refunds; RM28 refund caps | Published refund policy; auto-refund triggers on missed SLAs |
| T6 | Appointment ≠ priority | Booked slot honoured or compensated; no-queue model as core claim |
| T7 | Trial-to-hard-sell funnels | No packages sold in-session; cooling-off period by design; no commission on clinical staff |
| T8 | <3-minute consults | Minimum consult standards; async follow-up bundled |
| T9 | Buggy apps as the only door | WhatsApp-first pathway removes app-quality as a failure surface |

## 12. Frequency summary table

| # | Theme | Providers evidenced | Platforms evidenced | Persistence | Trend signal |
|---|---|---|---|---|---|
| T1 | Pricing opacity / bill shock | 5 hospitals + DA + slimming | Maps aggregators, App Store, ComplaintsBoard | Years (2017–2025 reviews) | Stable — no incumbent has restructured pricing |
| T2 | Communication failure | DA, DoC, Speedoc, Sunway, Pantai | App stores, aggregators | Years; Sep 2025 reviews current[^10] | Stable-worsening with scale |
| T3 | Prescription/medication | DA (structural), category-wide (illegal sellers) | App Store, MOH/MJPharm studies | Structural | Stable until regulation lands |
| T4 | Delivery/logistics | DoC (dominant), DA, Speedoc (tail) | App stores | Years | Unclear — no recent corpus large enough |
| T5 | Refund failure | Gleneagles, PCMC, LWM, Marie France, DoC | Aggregators, ComplaintsBoard, tribunal | Decade+ | Stable |
| T6 | Waiting/queue integrity | All 5 hospital brands + DA matching | Maps, iBanding, PissedConsumer | Decade+ | Stable — staffing-bound |
| T7 | Hard sell | LWM, Marie France, Dorra; latent at retail pharmacy | ComplaintsBoard, NCCC, forums, blogs | Two decades (2005–2008 NCCC archive → 2026 boards) | Migrating from salons toward aesthetic clinics *(inference)* |
| T8 | Rushed consults | KPJ, DA, Pantai | Maps corpora, App Store | Years | Stable |
| T9 | App/tech failure | Naluri, DA, Doctor2U | Play/App Store | Ongoing; Naluri improving[^32] | Improving where funded |

## 13. Monitoring plan (quarterly refresh)

1. Re-pull ComplaintsBoard/PissedConsumer counts for LWM, Marie France, KPJ pages — complaint velocity, not stock, is the leading indicator for T5/T7.[^8][^23]
2. Track TTPM annual claim statistics and any KPDN enforcement actions naming slimming/aesthetic operators.[^30]
3. Watch DA's App Store corpus for any prescription-letter policy change — it would close Welltech's T3 wedge.[^7]
4. Watch Alpro's Birdeye volumes as the benchmark for review-solicitation performance in Malaysian healthcare (per-outlet pages; see [review-score-comparison.md](review-score-comparison.md) §3).[^31]
5. Add Grab/foodpanda-style delivery-experience complaints to the T4 scan once Welltech's own logistics launch — the comparison set patients will actually use. *(analyst note)*

## 14. Forward view — complaint classes Welltech will face that incumbents don't *(analysis)*

The taxonomy above maps incumbent failure. A GLP-1/longevity/concierge entrant should expect four additional complaint classes with no Malaysian public precedent yet, and should pre-build responses:

| Anticipated class | Analogue evidence | Pre-emptive design |
|---|---|---|
| GLP-1 side-effect distress ("nobody warned me about the nausea") | Side-effect profiles are the core of international GLP-1 patient-experience literature; Malaysian clinic pages under-communicate them relative to price[^34] | Structured onboarding on side effects; day-3/day-7 proactive check-ins; documented consent |
| Supply interruption mid-treatment | Global semaglutide shortages; Malaysian price-tracker pages already log month-to-month availability/price shifts[^34] | Stock-visibility promise; therapeutic-switch protocol communicated before it's needed |
| Subscription/programme cancellation friction | The slimming-centre package-refund record shows exactly how prepaid-programme exits go wrong[^8][^21] | One-message cancellation; pro-rated refunds as published policy |
| Weight-regain disappointment after cessation | Qualitative obesity literature: repeated failed attempts are the segment's defining scar (see [sentiment-analysis.md](sentiment-analysis.md) §2.4) | Off-ramp programme and expectation-setting from month one |

The first provider whose complaint record shows *handled* versions of these four classes will define the category standard the way Sunway's feedback transparency defines the hospital standard.

---

## References

[^1]: iBanding, "Customer Reviews for Gleneagles Hospital Kuala Lumpur", https://review.ibanding.com/company/gleneagles-hospital-kuala-lumpur (accessed July 2026).
[^2]: Wupdoc, "Gleneagles Hospital Kuala Lumpur — 10 reviews", https://www.wupdoc.com/all-reviews/malaysia/gleneagles-hospital-kuala-lumpur-d-00000000349F (accessed July 2026).
[^3]: Top-Rated.Online, "Pantai Hospital Kuala Lumpur — reviews", https://www.top-rated.online/cities/Kuala+Lumpur/place/p/4295702/Pantai+Hospital+Kuala+Lumpur (accessed July 2026).
[^4]: MyMediTravel, "Pantai Hospital Kuala Lumpur", https://www.mymeditravel.com/medical-centers/malaysia/kuala-lumpur/kl-city/pantai-hospital-kuala-lumpur (accessed July 2026).
[^5]: Trustburn, "PRINCE COURT Reviews/Feedback", https://trustburn.com/reviews/prince-court (accessed July 2026).
[^6]: Foursquare, "Prince Court Medical Centre — 179 tips", https://foursquare.com/v/prince-court-medical-centre/4b374035f964a520264025e3 (accessed July 2026).
[^7]: Apple App Store (SG), "Doctor Anywhere: Healthcare — Ratings & Reviews", https://apps.apple.com/sg/app/doctor-anywhere-healthcare/id1273714922?see-all=reviews&platform=iphone (accessed July 2026).
[^8]: ComplaintsBoard, "London Weight Management Review: pushy sales consultants", https://www.complaintsboard.com/london-weight-management-pushy-sales-consultants-c483950 (accessed July 2026).
[^9]: sgforums, "London Weight Management Woes", https://sgforums.com/forums/8/topics/248313/2/ (accessed July 2026).
[^10]: Google Play, "Doctor Anywhere - Healthcare" listing, https://play.google.com/store/apps/details?id=com.doctoranywhere&hl=en_SG (accessed July 2026).
[^11]: Google Play, "DoctorOnCall: Online Pharmacy" listing, https://play.google.com/store/apps/details?id=com.doctoroncall.pharmacy (accessed July 2026); delivery-delay themes per [DoctorOnCall dossier](../20-competitor-dossiers/doctoroncall.md) §8.
[^12]: Top-Rated.Online, "Speedoc (Kuala Lumpur) Reviews", https://top-rated.online/cities/Kuala+Lumpur/place/p/9306855/Speedoc+(Kuala+Lumpur) (accessed July 2026).
[^13]: iBanding, "Customer Reviews for Sunway Medical Centre", https://review.ibanding.com/company/sunway-medical-centre (accessed July 2026).
[^14]: Malaysian Journal of Pharmacy, "Patterns of Prescription Medicines Sale Through E-Marketplace in Malaysia and Associating Factors", https://mjpharm.org/patterns-of-prescription-medicines-sale-through-e-marketplace-in-malaysia-and-associating-factors/ (accessed July 2026).
[^15]: MOH Pharmaceutical Services Programme, "Risk of purchasing medications via Internet", https://pharmacy.moh.gov.my/en/content/risk-purchasing-medications-internet.html (accessed July 2026).
[^16]: MOH Pharmaceutical Services Programme, "Tips on how to buy medicines online", https://pharmacy.moh.gov.my/en/content/tips-how-buy-medicines-online.html (accessed July 2026).
[^17]: AppBrain, "DoctorOnCall - Online Pharmacy (com.docmobile)", https://www.appbrain.com/app/doctoroncall-online-pharmacy/com.docmobile (accessed July 2026).
[^18]: AppGrooves, "Positive & Negative Reviews: Doctor2U — 3,594 reviews", https://appgrooves.com/android/my.doctor2u.client/doctor2u-your-one-stop-healthcare-app/bp-healthcare-group/negative (accessed July 2026).
[^19]: Apple App Store (SG), "Speedoc: Virtual Hospital App", https://apps.apple.com/sg/app/speedoc-care-comes-to-you/id1288838601 (accessed July 2026).
[^20]: London Weight Management Malaysia, "Promotion" page (RM28 first-treatment offer; refund terms reported in complaint coverage), https://londonweight.com.my/promotion/ (accessed July 2026).
[^21]: Studocu, IIUM Consumer Law notes citing Marie France Bodyline Sdn Bhd tribunal appeal, https://www.studocu.com/my/document/international-islamic-university-malaysia/consumer-law/consumer-midterm-notes/113786017 (accessed July 2026).
[^22]: iBanding, "Customer Reviews for KPJ Kajang Specialist Hospital", https://review.ibanding.com/company/kpj-kajang-specialist-hospital (accessed July 2026); complaint patterns per [KPJ dossier](../20-competitor-dossiers/kpj-healthcare.md) §5.
[^23]: PissedConsumer, "KPJ Puteri Specialist Hospital Reviews", https://kpj-puteri-specialist-hospital.pissedconsumer.com/review.html (accessed July 2026).
[^24]: KPJ Healthcare, "Guarantee Letter Application" (verification "may take up to around five hours"), https://kpjhealth.com.my/thc/gl-application (accessed July 2026).
[^25]: Wanderlog, "Sunway Medical Centre Damansara — reviews and ratings", https://wanderlog.com/place/details/15217965/sunway-medical-centre-damansara (accessed July 2026).
[^26]: SG Budget Babe, "Why I Will Never Sign Up With London Weight Management", https://sgbudgetbabe.com/why-i-will-never-sign-up-with-london-weight-management/ (accessed July 2026).
[^27]: My Dorra Slimming Personal Review, "Dorra slimming sales assistants lied", https://mydorraslimmingreview.wordpress.com/2012/03/06/dorra-slimming-sales-assistants-lied/ (accessed July 2026).
[^28]: ComplaintsBoard, "London Weight Management Review: they cheated on my scale", https://www.complaintsboard.com/london-weight-management-they-cheated-on-my-scale-c464920 (accessed July 2026).
[^29]: FOMCA/NST via NCCC, "Victims face financial ruin, emotional trauma and physical scars" (6,925 wellness/aesthetic complaints 2015–2017; >RM2M losses), https://www.fomca.org.my/v1/index.php/fomca-di-pentas-media/727-nst-victims-face-financial-ruin-emotional-trauma-and-physical-scars-shabana-naseer-ahmad-senior-legal-advisor-nccc (accessed July 2026).
[^30]: KPDN, "Consumer Complaints" and TTPM e-Tribunal portal (CCMC 11,426 complaints in 2023; 9,203 TTPM claims worth RM77.2M in 2025 to 14 Nov), https://www.kpdn.gov.my/en/consumerism/hak-pengguna/consumer-complaints and https://ttpm.kpdn.gov.my/ (accessed July 2026).
[^31]: Glassdoor, "Alpro Pharmacy Reviews", https://www.glassdoor.com/Reviews/%E2%80%8BAlpro-Pharmacy-Reviews-E1379925.htm (accessed July 2026).
[^32]: Google Play, "Naluri" listing and reviews, https://play.google.com/store/apps/details?id=life.naluriclientapp&hl=en_US (accessed July 2026).
[^33]: AppBrain, "Naluri (life.naluriclientapp)", https://www.appbrain.com/app/naluri/life.naluriclientapp (accessed July 2026).
[^34]: Peak Protocol, "Weight Loss Injection Prices Malaysia 2026 (updated monthly)", https://peakprotocolmy.com/glp-1/weight-loss-injection-prices-malaysia/ (accessed July 2026); PMC, "Patients' experiences with GLP1-RAs — a systematic review", https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12090293/ (accessed July 2026).
