# US Reference Company: Medvi — the Marketing-Led, Compounding-Dependent Cautionary Case

**Abstract.** Medvi (MEDVi, LLC; Newark, Delaware) is a direct-to-consumer telehealth brand that sells **compounded** semaglutide and tirzepatide on a cash-pay monthly subscription. It is the near-perfect negative of Welltech's intended model, and the single most useful "what-not-to-do" case in this repository. Founded in **September 2024** by solo entrepreneur **Matthew Gallagher** with reportedly **US$20,000** and off-the-shelf AI tools, and staffed by effectively **two people** (Gallagher and his brother), Medvi reported **~US$401M in 2025 revenue** and claimed a **US$1.8B run-rate** for 2026 — a story a glowing April 2026 *New York Times* profile amplified before the paper issued substantial corrections.[^1][^2] Medvi owns no pharmacy, employs no physicians, and holds no drug licenses; everything clinical is outsourced.[^3] It grew on **AI-generated, fake-doctor affiliate advertising**, drew a **35-state-attorneys-general** rebuke of the category, received an **FDA warning letter (20 Feb 2026)** for misbranding, faces **spam/TCPA class litigation**, and is entangled in an **OpenLoop data breach** affecting ~1.6M patients.[^4][^5][^6][^7] Its reputation record is bimodal — an implausibly high Trustpilot score alongside an **F BBB rating** and a "no refunds" subscription policy.[^8][^9] Depth here is deliberately light: Medvi's value to Welltech is entirely as a catalogue of failure modes to avoid.

Last updated: July 2026

Related documents: [US market overview](us-market-overview.md) · [Lessons for Welltech](lessons-for-welltech.md) · [Hims & Hers](hims-hers.md) · [Research standards](../RESEARCH-STANDARDS.md)

**Method note.** Direct page retrieval (WebFetch) was blocked at the network level during this research pass; primary documents (the FDA warning letter, court filings) could not be opened directly. Evidence is drawn from ~12 web searches over the FDA (via trade-press reproduction), business and health-trade press (Morning Brew, Forbes, Forrester, Techdirt, Drug Discovery & Development, eMarketer), review platforms (Trustpilot, BBB, ConsumerAffairs), and analyst commentary, cited per source. **Transparency caveat:** Medvi is a private, opaque, two-person entity; several headline figures are self-reported run-rates, not audited, and are flagged as such. Where the record is thin or a name-collision exists, that is stated as a finding.

---

## 1. Why this company is in the repository

Welltech's thesis is outcome-accountable, retention-led, compliance-first, branded-drug, clinician-anchored care. Medvi is the inverse on every axis: outcome-indifferent, acquisition-led, compliance-last, compounded-drug, clinician-outsourced. It is included precisely because it demonstrates, in one entity, how far a marketing-led compounded-GLP-1 operator can scale in the US regulatory gaps — and how fast the exposure accumulates once the gaps close. Every "Con" below is a lesson Welltech can bank without paying for it.

## 2. Identity and structure — what Medvi actually is

| Item | Detail | Confidence |
|---|---|---|
| Legal entity | MEDVi, LLC, dba MEDVi; Newark, Delaware[^4][^5] | High |
| Founded | September 2024[^1] | High |
| Founder / owner | Matthew Gallagher (~41, LA-based); reportedly owns 100%[^1] | Medium (self-reported) |
| Staff | Effectively two: Gallagher + his brother Elliot; AI does the rest ("vibe-coded" site, AI customer service, Midjourney ad creative)[^1][^2] | Medium |
| Funding | None raised externally; ~US$20,000 self-funded start; **no official valuation**[^1][^2] | Medium |
| 2025 revenue | ~US$401M (first full year, self-reported)[^1] | Low–Medium (unaudited) |
| 2026 claim | ~US$1.8B run-rate (extrapolated, not a valuation)[^2] | Low (run-rate, self-reported) |
| Coverage geography | All US states except North Dakota[^10] | High |
| Pharmacy / physicians / licenses | **None owned** — all clinical and dispensing outsourced (CareValidate, OpenLoop Health, Beluga Health, Belmar Pharma Solutions)[^3] | High |

**Finding — opacity is the story.** Medvi has no audited accounts, no institutional investors, no board, and a two-person headcount. The "US$1.8B company" framing is a self-reported revenue **run-rate**, not a financed valuation — a distinction multiple analysts stressed after the NYT profile.[^2][^11] For an intelligence file, the thinness and self-reporting of the record is itself a red flag: this is a marketing entity wrapped around outsourced clinical infrastructure, not an integrated care company.

### 2.1 Timeline

| Date | Event |
|---|---|
| Sep 2024 | Medvi founded; ~US$20k, AI tooling, two people[^1] |
| Feb 2025 | FDA declares semaglutide shortage resolved; compounding wind-down begins[^14] |
| 2025 (FY) | Reports ~US$401M revenue (first full year)[^1] |
| Dec 2025 | 35 state AGs write to Meta over deceptive AI weight-loss ads (the category Medvi typifies)[^13] |
| Jan 2026 | Outsourced partner OpenLoop discloses breach (~1.6M patients)[^7] |
| 20 Feb 2026 | FDA warning letter #721455 to MEDVi, LLC (misbranding)[^4] |
| 20 Mar 2026 | Class action filed (C.D. Cal.) over affiliate spam / spoofed emails[^11] |
| 2 Apr 2026 | Glowing NYT profile; ~US$1.8B run-rate claim goes viral[^2] |
| Apr 2026 | NYT issues substantial corrections after criticism[^16] |

## 3. Model and pricing

Medvi is a **cash-pay, no-insurance** subscription. The monthly fee bundles the medication with unlimited async messaging and telehealth access; HSA/FSA is accepted.[^10] It is a classic intro-price-then-step-up funnel:

| Product | Intro (month 1) | Ongoing | Source |
|---|---|---|---|
| Compounded semaglutide injection | US$179 | US$299 | [^10] |
| Compounded semaglutide tablet | US$249 | US$369 | [^10] |
| Compounded tirzepatide (inj./tablet) | US$279 | US$399 | [^10] |
| Branded Zepbound / Wegovy | — | ~US$1,999/mo + US$99 membership | [^10] |

The commercial engine is the **~US$179 → US$299 step-up** and the friction on exit (see §6). The economics are pure drug-retail arbitrage: buy compounded API-based product from a 503A/503B compounder (Belmar), wrap it in a subscription, and spend the margin on paid acquisition.

## 4. Marketing approach and compliance posture

Marketing *is* the company. Medvi's growth was manufactured through **AI-generated affiliate advertising**:

- **Fake/deepfaked doctor personas** and AI-generated testimonials in Facebook/Instagram ads; reporting cites on the order of **~5,000 ad campaigns** in Meta's ad library tied to the brand/affiliates.[^4][^12]
- Claims that documented experts called dangerous — e.g. an Instagram ad guaranteeing **"no side effects, just real results"** for drugs with well-documented GI and other side effects.[^12]
- AI-fabricated **before/after** comparison images. In December 2025 a bipartisan coalition of **35 state attorneys general** wrote to Meta warning that fabricated AI images, spokespeople, and medical claims "cross a line" — the category Medvi typifies.[^12][^13]

**Compliance posture: reactive and deflecting.** After the FDA warning letter, founder Gallagher's public line was that doctor portrayals in advertising are "longstanding," that the site carries disclaimers, and that the FDA letter "was sent to an affiliate" and the issue "has since been resolved."[^12] The affiliate-distancing defense is itself a structural tell: growth is subcontracted to affiliates whose conduct the brand then disowns when regulators arrive.

### 4.1 The AI-operations layer — impressive and hollow

The genuinely novel thing about Medvi is how little company sits behind the revenue. The website was "vibe-coded" with AI; customer service is run by AI agents; ad creative (images, personas, testimonials) is generated with tools like Midjourney; and the clinical and pharmacy work is entirely subcontracted.[^1][^3] The result is a business with almost **no operational substance of its own** — a marketing and billing wrapper around third-party infrastructure.

For Welltech the double-edged reading matters. On one edge, it is a real benchmark for how cheap a DTC telehealth funnel now is to stand up — the tooling advantage is genuine. On the other, Medvi shows the **failure mode of the same tooling**: when the creative layer is AI-generated and the accountability layer is outsourced, deception scales as easily as growth, and there is no internal function that owns safety, quality, or truth. The lesson is that AI should compress Welltech's **cost**, never its **accountability**.

## 5. The compounding-loophole dependence and the 2025 shortage cliff

Medvi was **founded in September 2024 — inside the compounding window** — and its entire product is compounded GLP-1. That window was already closing as the company launched:

- The FDA **declared the semaglutide shortage resolved in February 2025**; 503A compounders had to stop by **~22 April 2025**, and the same resolution applied to tirzepatide earlier.[^14][^15]
- Post-resolution, operators (Medvi included) rely on the **"personalization" exemption**, adding B-vitamins or altering dose/form to argue the product is not "essentially a copy." Reporting indicates ~80% of compounded semaglutide/tirzepatide scripts now carry supplemental ingredients purely to sustain that argument — a legally brittle basis.[^15]
- Quality is a live safety concern across the compounded category: Novo Nordisk reported that some compounded injectable semaglutide contained **up to 86% impurities**.[^15]

Medvi therefore sits directly on the **shortage-resolution cliff**: its single product line depends on an exemption regulators are actively working to close, with no branded supply relationship, no manufacturing control, and no clinical moat to fall back on.

## 6. Reputation and complaints — the themes

The review record is **bimodal and should be read skeptically.**

| Source | Rating | Note |
|---|---|---|
| Trustpilot (medvi.org) | ~4.4 / 5 from **11,000+** reviews[^8] | Implausibly high volume/score for the complaint pattern; solicitation/curation suspected |
| ConsumerAffairs | ~3.6 from ~1,600 reviews[^8] | Billing the dominant complaint |
| BBB (Newark, DE) | **F rating**, not accredited[^9] | Billing and subscription complaints |

**Name-collision caveat (a finding, not a defense).** A separate company, **MEDvidi** (medvidi.com, a San Jose mental-health platform), is frequently confused with Medvi in complaint databases; some aggregated "Medvi" complaints belong to MEDvidi. Analysts should not over-count.[^9]

**Recurring complaint themes (evidence-backed):**

1. **Subscription-trap / no-refund policy.** Medvi's stated terms include, in capitals, *"IN NO EVENT SHALL YOU BE ISSUED A REFUND UPON CANCELLATION OF THE SUBSCRIPTION SERVICES,"* with 72-hour pre-billing cancellation notice; once medication is ordered for the cycle, the charge is final.[^8]
2. **Moving-goalpost guarantee.** Users report the money-back "guarantee" period shifting from 3 to 5 months, and any weight fluctuation (even ~1 lb) disqualifying a refund, minus a **25% doctor-consultation fee**.[^8]
3. **Surprise / duplicate charges.** Reports of an additional ~US$299/month from OpenLoop Healthcare on top of the medication charge, without clear disclosure.[^8]
4. **Customer-service friction.** Repeated reports of dozens of unanswered contacts around cancellation and refunds.[^8]
5. **Product/clinical praise coexists.** Medication and clinical support often score well; the negatives cluster almost entirely on **billing, refunds, and cancellation** — the signature of a funnel optimised for acquisition and retention-by-friction, not outcomes.[^8]

## 7. Regulatory and legal exposure

For a two-person, two-year-old company, the exposure is remarkably dense:

- **FDA warning letter #721455 (20 Feb 2026)** to MEDVi, LLC: the site displayed compounded products bearing a **"MEDVi" label**, implying Medvi is the compounder (it is not) — **misbranding**; and used claims such as *"Same active ingredient as Wegovy® and Ozempic®"* / *"…as Mounjaro® and Zepbound®"* that falsely imply FDA approval or evaluation.[^4][^5]
- **Spam / consumer-protection litigation:** a class action filed **20 March 2026 (C.D. Cal.)** alleging Medvi uses affiliate marketers to send deceptive spam emails with spoofed domains and falsified headers (CAN-SPAM/TCPA theories); Medvi denies wrongdoing.[^11]
- **OpenLoop data breach:** Medvi's outsourced clinical partner OpenLoop Health disclosed a breach (**Jan 2026**) affecting **~1.6M patients**; OpenLoop notified the Texas AG (**Mar 2026**, 68,160 TX residents) and faces class actions — Medvi patients' data is in scope by virtue of the outsourcing.[^7]
- **Media reversal:** a laudatory **NYT profile (2 Apr 2026)** omitted the FDA letter and lawsuits; after criticism (Techdirt: "got played by a telehealth scam"; Forrester: "beware the magical two-person US$1B AI-driven startup"), the NYT made **substantial corrections**, conceding the piece "should have included that information."[^2][^11][^16]

### 7.1 Medvi vs Hims — same category, opposite ends

Read alongside [Hims & Hers](hims-hers.md), Medvi maps the far, disreputable end of the compounded-GLP-1 spectrum. The contrast is the lesson:

| Dimension | Hims & Hers | Medvi |
|---|---|---|
| Structure | Public, audited, integrated (owns brand, some clinical) | Private, unaudited, two people, all outsourced |
| Supply | Attempted branded partnership (Novo) | Compounded only, no manufacturer relationship |
| Marketing | Aggressive but human/celebrity-led | AI-fabricated fake doctors, fake testimonials |
| Regulatory response | Senate letters, manufacturer dispute | FDA warning letter, AG scrutiny, class actions |
| Reputation | Mixed but transparent | Bimodal, F BBB, no-refund policy |
| Accountability | A public company with a board | A marketing shell with a disclaimer |

Both sit on the same compounding cliff. The difference is that Hims has scale, capital, and a diversification path off the cliff; Medvi has a run-rate claim, an FDA letter, and nowhere to land. For Welltech, Hims is "copy the platform, avoid the loophole"; Medvi is "avoid the whole posture."

## 8. Pros — the (narrow) positives

1. **Capital efficiency proof-point.** A two-person, AI-tooled operator reaching hundreds of millions in reported sales shows how low the cost of standing up a DTC telehealth funnel now is — the demand and the tooling are real, even if the business is fragile.[^1]
2. **Funnel and pricing clarity.** The transparent cash-pay, medication-inclusive, intro-priced subscription is a clean, legible offer that converts — the mechanic (not the ethics) is worth studying.[^10]
3. **AI-native operations.** Vibe-coded site, AI customer service, AI creative — a live demonstration of how thin the operational layer can be, useful as a build-cost benchmark.[^1]

## 9. Cons — the failure catalogue

1. **Single-product, loophole-dependent** with no branded supply, no manufacturing, no clinical moat — maximally exposed to the shortage-resolution cliff.[^14][^15]
2. **Deceptive, AI-fabricated marketing** (fake doctors, "no side effects," fake before/afters) — the direct cause of the FDA letter and AG scrutiny.[^4][^12]
3. **Everything clinical outsourced** (CareValidate/OpenLoop/Beluga/Belmar) — no control over quality, and inherited breach liability.[^3][^7]
4. **Subscription-trap economics** — no-refund terms, moving guarantee goalposts, surprise charges — retention by friction, not outcomes.[^8]
5. **Regulatory/legal density** — FDA warning, spam class action, data-breach exposure — for a company barely 18 months old.[^4][^7][^11]
6. **Opacity** — unaudited self-reported run-rates dressed as a valuation; a marketing shell over outsourced infrastructure.[^2][^11]

## 10. Lessons for Welltech

The full mapping lives in [lessons-for-welltech.md](lessons-for-welltech.md). Medvi's payload is almost entirely cautionary:

1. **Do not build on the compounding loophole.** Medvi is what "loophole-native" looks like when the loophole closes: a single-product company with no branded supply and no fallback. Welltech's branded-drug, manufacturer-partnered stance is the correct opposite — and Asia's compounding rules are far tighter than the US window Medvi exploited, so this route is not even available.
2. **Marketing that lies is a liability that compounds.** Fake-doctor and "no side effects" advertising bought Medvi growth *and* an FDA letter, an AG rebuke, and class litigation. In MY/SG/HK, medical-advertising law (MOH/HSA/DoH, PDPA) is stricter and enforced; the same tactics would be existential. Welltech's edge is **compliant, clinician-fronted, honest** marketing — slower, but durable.
3. **Own (or tightly govern) the clinical and data layer.** Medvi outsourced everything and inherited OpenLoop's 1.6M-patient breach and quality risk it could not control. Welltech should keep clinical accountability and data governance **in-house or under enforceable control**, especially under Asia's PDPA/PDPO regimes.
4. **Retention by outcomes, not by friction.** Medvi's complaint record is a masterclass in what erodes trust: no-refund terms, moving guarantees, surprise charges, unreachable support. Welltech should compete on the exact opposite — transparent cancellation, outcome-linked guarantees, responsive care — because trust is the moat commodity drug-retail lacks.
5. **Beware your own growth story.** The NYT episode shows how a marketing-led operator can manufacture a narrative that outruns its substance — until the corrections land. Welltech should let audited outcomes, not run-rate theatrics, tell its story to investors and regulators.

---

## References

[^1]: Forbes (Josipa Majić), "AI And $20,000 Helped One Man Build A $1.8 Billion Telehealth Startup" (founded Sept 2024; ~US$20k start; Gallagher owns 100%; brother Elliot only employee; US$401M 2025 sales; vibe-coded site, AI customer service, Midjourney creative), https://www.forbes.com/sites/josipamajic/2026/04/02/ai-and-20000-helped-one-man-build-a-18-billion-telehealth-startup/ (accessed July 2026).
[^2]: Techdirt, "The New York Times Got Played By A Telehealth Scam And Called It The Future Of AI" (US$1.8B is a run-rate not a valuation; no outside funding; FDA/lawsuit omissions), https://www.techdirt.com/2026/04/07/the-new-york-times-got-played-by-a-telehealth-scam-and-called-it-the-future-of-ai/ (accessed July 2026).
[^3]: Drug Discovery & Development, "Fake testimonials, no pharmacy and an FDA warning: how MEDVi built a $1.8 billion telehealth company in the gaps between regulators" (Medvi owns no pharmacy, employs no physicians, holds no drug licenses; clinical outsourced to CareValidate, OpenLoop Health, Beluga Health, Belmar Pharma Solutions), https://www.drugdiscoverytrends.com/fake-testimonials-no-pharmacy-and-an-fda-warning-how-medvi-built-a-1-8-billion-telehealth-company-in-the-gaps-between-regulators/ (accessed July 2026).
[^4]: FDA, "MEDVi, LLC dba MEDVi - 721455 - 02/20/2026" warning letter (misbranding; "MEDVi" label implies it is the compounder; "Same active ingredient as Wegovy®/Ozempic®" and "…Mounjaro®/Zepbound®" imply FDA approval/evaluation), https://www.fda.gov/inspections-compliance-enforcement-and-criminal-investigations/warning-letters/medvi-llc-dba-medvi-721455-02202026 (accessed July 2026).
[^5]: Drug Discovery & Development, "The New York Times spotlighted MEDVi. The FDA had already warned the self-proclaimed 'fastest growing company in history.'" (FDA warning letter dated 20 Feb 2026; misbranding and false-equivalence claims; NYT omissions), https://www.drugdiscoverytrends.com/the-new-york-times-spotlighted-medvi-the-fda-had-already-warned-the-self-proclaimed-fastest-growing-company-in-history/ (accessed July 2026).
[^6]: eMarketer, "Fake doctor ads fuel scrutiny of GLP-1 marketer" (Medvi affiliate ads with fake doctors/AI testimonials; regulatory scrutiny), https://www.emarketer.com/content/fake-doctor-ads-fuel-scrutiny-of-glp-1-marketer (accessed July 2026).
[^7]: Medical Foundation of NC, "MEDVi Scam or Legit? FDA Warning Letter, Lawsuits, Data Breach, and Verified Facts — A 2026 Fact Check" (OpenLoop Health breach disclosed Jan 2026, ~1.6M patients; Texas AG notified Mar 2026, 68,160 TX residents; class actions), https://medicalfoundationofnc.org/medvi-in-2026/ (accessed July 2026).
[^8]: The RX Index, "MEDVi Reviews (2026): Costs, Complaints & Verdict" and Trustpilot (medvi.org) / ConsumerAffairs data (Trustpilot ~4.4/5 from 11,000+; ConsumerAffairs ~3.6/1,600; no-refund policy quote; 72-hour cancellation; guarantee 3→5 months; 25% consult fee; duplicate OpenLoop US$299 charge), https://therxindex.com/guides/medvi-reviews/ (accessed July 2026); Trustpilot, https://www.trustpilot.com/review/medvi.org (accessed July 2026).
[^9]: BBB, "MEDVi | Better Business Bureau" (Newark, DE profile; F rating, not accredited; MEDvidi name-collision caveat), https://www.bbb.org/us/de/newark/profile/medical-consultants/medvi-0251-92034163/customer-reviews (accessed July 2026).
[^10]: ConsumerAffairs / U.S. News, "MEDVi Reviews" (cash-pay, no insurance; medication-inclusive membership; injections US$179→US$299, tablets US$249→US$369; tirzepatide US$279→US$399; branded ~US$1,999/mo + US$99; all states except North Dakota; HSA/FSA), https://www.consumeraffairs.com/health/medvi.html (accessed July 2026).
[^11]: Moneywise, "A $1.8 billion startup with just 2 employees was hailed as the future. Now, the negative allegations are piling up" (run-rate vs valuation; class action filed 20 Mar 2026 in C.D. Cal. over spam/spoofed emails; Medvi denies), https://moneywise.com/news/top-stories/a-18-billion-startup-with-just-2-employees-was-hailed-as-the-future-now-the-negative-allegations-are-piling-up (accessed July 2026).
[^12]: eMarketer / Morning Brew, "One guy built an AI telehealth startup with a lot of red flags" (fake/deepfaked doctors; AI testimonials; ~5,000 Meta ad campaigns; "no side effects, just real results" claim; Gallagher's affiliate-distancing defense), https://www.morningbrew.com/stories/one-guy-built-ai-telehealth-startup-red-flags (accessed July 2026).
[^13]: eMarketer, "Meta faces scrutiny over misleading weight loss drug ads" (35 state attorneys general letter to Meta, Dec 2025, on deceptive AI before/after weight-loss ads), https://www.emarketer.com/content/meta-faces-scrutiny-over-misleading-weight-loss-drug-ads (accessed July 2026).
[^14]: FDA, "FDA clarifies policies for compounders as national GLP-1 supply begins to stabilize" (semaglutide shortage resolved Feb 2025; 503A stop-date ~22 Apr 2025), https://www.fda.gov/drugs/drug-alerts-and-statements/fda-clarifies-policies-compounders-national-glp-1-supply-begins-stabilize (accessed July 2026).
[^15]: Healthcare Brew, "Despite FDA crackdown, unapproved GLP-1s still threaten the industry" (~80% of compounded scripts add supplemental ingredients to sustain personalization; Novo finding of up to 86% impurities in some compounded semaglutide), https://www.healthcare-brew.com/stories/2026/03/23/fda-crackdown-unapproved-glp-1s (accessed July 2026).
[^16]: Futurism, "New York Times Makes Substantial Changes to Article That Glazed a Sleazy AI Startup: 'Our Piece Should Have Included That Information'" (NYT corrections to the Medvi profile), https://futurism.com/artificial-intelligence/new-york-times-edits-medvi-article (accessed July 2026).
