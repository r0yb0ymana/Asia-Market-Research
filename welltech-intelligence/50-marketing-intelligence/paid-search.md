# Paid Search for Digital Health in Malaysia: Google Ads Policy, KKLIU Compliance, Advertiser Landscape, and a Launch Budget Model

**Abstract.** Paid Google acquisition for a Malaysian medical weight-loss and telehealth brand operates inside a double cage: Google's healthcare advertising policies (prescription-drug terms are barred from promotional use in ads, keywords, and landing pages for Malaysia-targeted campaigns; online-pharmacy promotion is not permitted in Malaysia; weight loss is a "sensitive interest category" with personalisation and remarketing bans) and Malaysian law (every consumer medicine/health-service advertisement requires prior MAB approval with a displayed KKLIU number; prescription medicines cannot be advertised to the public at all). The practical consequence is that Welltech cannot buy "Ozempic Malaysia" traffic — but can lawfully and profitably buy clinic/program/symptom/service demand ("weight loss clinic KL", "doktor online", "health screening package") and route it into WhatsApp via message assets. Malaysian search CPCs are low by global standards (agency-published range ~RM1.80–12.50 by industry; most SMEs pay RM3–6/click), which combined with consult-to-program pricing from the weight-loss market dossier yields modeled CACs of roughly RM250–750 per program start at realistic funnel rates — economics that work against a RM900+/month program but demand tight negative-keyword hygiene and compliant landing pages. This document details both policy stacks, maps the observed advertiser ecosystem, sets CPC/CPL expectations (labelled by evidence grade), designs the click-to-WhatsApp and Performance Max architecture, and builds an illustrative launch budget model with stated assumptions and a verification plan.

Last updated: July 2026

Related: [seo.md](seo.md) · [funnels.md](funnels.md) · [positioning.md](positioning.md) · [../10-market-intelligence/malaysia-regulations.md](../10-market-intelligence/malaysia-regulations.md) · [../10-market-intelligence/malaysia-weight-loss-market.md](../10-market-intelligence/malaysia-weight-loss-market.md) · [../10-market-intelligence/malaysia-whatsapp-healthcare.md](../10-market-intelligence/malaysia-whatsapp-healthcare.md)

---

## 1. Method and evidentiary limits

Remote desk research, July 2026: ~19 structured web searches (English + Bahasa Malaysia) across Google policy documentation, Malaysian regulator pages, agency benchmark publications, and case studies. Limits, stated plainly:

- **Live auction data is unverifiable remotely.** We did not observe Malaysian SERPs from a Malaysian IP, so "who is bidding on what" is inferred from the advertiser ecosystem's public footprint (agency case studies, clinic marketing pages, platform positioning), not from captured sponsored results. Verification path: Google Ads Transparency Center lookups per advertiser + geolocated SERP capture (§9).[^1]
- **No Malaysian healthcare-specific CPC dataset surfaced.** Published Malaysian CPC figures are cross-industry agency aggregates;[^2][^3] US healthcare benchmarks are directional only.[^4] All Welltech keyword CPCs in §6 are *(analyst estimates)* with reasoning; treat the first RM10–20K of spend as paid market research.
- Policy citations reflect Google documentation and reporting as of July 2026; Google's healthcare policy has changed materially twice since 2024 (restricted drug terms rework; October 2025 prescription-drug enforcement update),[^5][^6] so re-verify at campaign build.

## 2. Google's policy cage: what cannot be bought in Malaysia

Google's "Healthcare and medicines" policy governs everything below; advertisers must also comply with local law, and violations can suspend accounts without prior warning.[^7]

### 2.1 Prescription-drug terms — the hard wall

- Google **restricts prescription drug terms in ads, keywords, and landing pages**. Promotional use of these terms is allowed only for campaigns targeting **Canada, New Zealand, and the United States** (with certification required to keyword-target them even there). Campaigns targeting Malaysia **may not use prescription drug terms for promotional purposes at all**.[^5][^8]
- Practical meaning for Welltech: no ads or keywords containing "Ozempic", "Wegovy", "Mounjaro", "semaglutide", "tirzepatide", "Saxenda"; and — the trap most operators miss — **the ad's landing page must also avoid promotional use of those terms**. A "Wegovy price Malaysia" cost guide (an SEO asset — see [seo.md](seo.md)) cannot be the destination of a paid ad; paid traffic needs parallel, drug-name-free program pages.
- Non-promotional use (safety notices, regulatory warnings, genuinely educational content) is carved out,[^6][^8] but relying on that carve-out for commercial landing pages is an account-suspension gamble; do not.

### 2.2 Online pharmacy and telemedicine certification

- **Online-pharmacy promotion is permitted only in an enumerated country list — Malaysia is not on it.**[^9] Welltech must not present ad-linked pages as "buy medicine online"; medication is dispensed inside the clinical program, not advertised as e-commerce.
- Telemedicine providers that prescribe fall under Google's prescription-drug-services restriction and generally need certification (LegitScript) to advertise those services. Google-recognised LegitScript telemedicine certification exists for the US, UK, Indonesia, Philippines, New Zealand, Japan, Australia and others — **Malaysia is not a listed telemedicine-certification country**.[^10][^11] Consequence *(analysis)*: there is no certification lane to advertise "online prescription" services in Malaysia; Welltech's paid ads must be framed as **clinic/doctor-consultation services** (bookings, screenings, programs), which sit outside the restricted prescription-services frame. This matches how Malaysian telehealth incumbents present themselves publicly.
- Precedent that Google localises enforcement in Malaysia when regulators engage: from April 2026 Google requires Bank Negara/SC-verified status for Malaysian financial-services advertisers.[^12] A comparable healthcare verification regime for Malaysia is plausible mid-term *(inference)* — being the compliant operator early is cheap insurance.

### 2.3 Weight loss as a sensitive category

- Weight loss sits in Google's **sensitive interest categories / health-in-personalised-advertising** rules: no remarketing/retargeting off weight-loss interest, no advertiser-curated audiences built on health signals; predefined Google audiences remain usable.[^13][^14]
- Creative rules: no idealised/body-shaming imagery, no unrealistic-results claims, no before/after transformations, 18+ targeting.[^14][^15] Note the convergence: Malaysian MAB rules independently prohibit testimonials and before/after weight photos ([../10-market-intelligence/malaysia-regulations.md](../10-market-intelligence/malaysia-regulations.md) §6) — one conservative creative standard satisfies both regimes.
- Also relevant: birth-control/fertility ad content is prohibited in Malaysia specifically[^7][^9] — a boundary if Welltech later extends into women's-health adjacencies.
- Advertiser identity verification (business registration + ID) applies to Malaysian advertisers and surfaces Welltech's identity in the Ads Transparency Center.[^16][^1]

### 2.4 What CAN be bid on (the permitted lanes)

| Lane | Example keywords | Policy status |
|---|---|---|
| Clinic/service | weight loss clinic KL, klinik kurus badan, doctor consultation online | Allowed (standard healthcare service promotion)[^7] |
| Program | medical weight loss program, doctor-supervised weight loss, weight management program Malaysia | Allowed; strongest fit with MAB "service advertising" lane |
| Symptom/condition (non-scheduled) | can't lose weight, BMI check, always tired, snoring | Allowed; obesity is not on the MASA scheduled-disease list, but avoid treatment-outcome claims[^17] |
| Screening/diagnostics | health screening package, full body checkup KL, pakej pemeriksaan kesihatan | Allowed; hospital advertisers already normalise it |
| Telehealth access | online doctor Malaysia, doktor online, video consultation | Allowed if framed as consult service, not online prescribing (§2.2) |
| Brand | welltech, welltech clinic | Allowed; defensive necessity (§8) |
| **Prohibited** | any POM brand/generic name; "buy [drug] online"; compounded GLP-1 terms | Restricted drug terms + MASA POM-advertising prohibition[^5][^17] |

## 3. The Malaysian law layer: KKLIU/MAB applied to search ads

Full statutory analysis in [../10-market-intelligence/malaysia-regulations.md](../10-market-intelligence/malaysia-regulations.md) §6; the operational translation for paid search:

1. **Search ads are "advertisements" under MASA 1956.** The Act's definition covers any notice or announcement in any medium; MOH's enforcement practice explicitly covers internet platforms and social media, with engagement sessions to remove non-compliant listings and tens of thousands of takedowns.[^17][^18][^19]
2. **Medicine/medical-service ads require prior MAB approval, evidenced by a KKLIU number displayed on the creative.** Approval lead time runs ~4–6 weeks; approvals expire and MOH publishes expiry notices (LIU 2025 expiry list).[^17][^20] Text ads have no room for the number — the compliant pattern used by Malaysian healthcare marketers is to carry the KKLIU number on the **landing page** and keep ad copy service-descriptive rather than therapeutic *(practice reported by Malaysian healthcare-marketing specialists; regulator guidance does not spell out an RSA-specific rule — obtain written confirmation from BPF, §9)*.[^21][^22]
3. **Facility/service ads (PHFSA + MAB 3/2023 guideline): no comparative claims, no price-comparison ads, no testimonials, no misleading claims.**[^23] This kills "cheapest GLP-1 in KL"-style copy even where Google would allow it, and prohibits review-quote ad extensions.
4. **Enforcement is active and priced in RM millions**: RM120M in fines cited for unregistered-product violations; weight-loss promises are a flagged hallmark of illegal advertising; TikTok-live medicine selling is a named enforcement target.[^18][^19] Aesthetic-clinic competitors run non-compliant claims routinely; their ad accounts and creatives are structurally fragile — Welltech's compliance is a durable auction advantage *(analysis)*.
5. **Workflow rule**: every consumer-facing creative (ad copy variants, landing pages, WhatsApp broadcast used promotionally) passes one internal marketing-compliance review; KKLIU submissions batched monthly. Budget the 4–6 week approval lag into every campaign calendar.[^17]

## 4. Observed advertiser landscape (evidence-graded)

Who is spending on Malaysian health search demand — inferred from public footprint, not live SERP capture:

| Advertiser type | Evidence | Reading |
|---|---|---|
| Aesthetic/weight clinics (Nexus, Glojas, CLEO, Clique, Her Clinic, NextMed etc.) | Dense SEO/SEM-optimised price pages; agencies openly sell them Google Ads programs; a JB dermatology clinic's published Google Ads case study (103 leads → 57 patients, 55% lead-to-patient)[^24][^25] | The core auction competitors on weight/clinic terms; sophisticated on volume, weak on compliance |
| Telehealth platforms (DoctorOnCall, Doctor Anywhere, DOC2US, Speedoc) | Established consumer brands with promo pricing (RM19.90–30 consults) and app-install economics ([../10-market-intelligence/malaysia-telehealth.md](../10-market-intelligence/malaysia-telehealth.md)) | Likely bidders on telemedicine/online-doctor terms and their own brands *(inference)*; thin margins cap their bids |
| GLP-1 telehealth entrants (OVA, Seimbang, Roczen) | OVA's visible acquisition is Meta/Instagram-led (17K followers, celebrity content, email ads)[^26] | Social-first, search-light *(inference)* — paid search on program terms is comparatively uncontested |
| Hospitals (IHH, Sunway, Columbia Asia, Prince Court) | Heavy screening-package page infrastructure; health-tourism budgets | Bid on screening/specialist terms; unlikely to contest weight-program terms |
| Agencies/infrastructure (Lamanify, ZenWeb, MYSense, Omnicore) | Publish healthcare-specific Google Ads + KKLIU-compliance offerings and Malaysian CPC benchmarks[^2][^21][^25][^27] | A mature supply side exists; also a competitive-intelligence source |
| Grey-market sellers | MOH takedown volumes; Shopee/TikTok enforcement warnings[^18][^19] | Suppressed on Google by drug-term restrictions; migrate to social/e-commerce — Google SERPs are cleaner than Meta feeds for this category |

**US read-across, used cautiously:** the compounded-GLP-1 telehealth ad boom and FDA/HHS crackdown (55+ warning letters 2025; 30 more in Feb 2026; Novo v. Hims)[^28][^29] shows what regulator response looks like when GLP-1 advertising outruns rules. Malaysia's MAB regime is *stricter on paper* than the pre-crackdown US; expect enforcement attention to follow the money into this category *(inference)*.

## 5. CPC and CPL expectations

**Published Malaysian data (cross-industry):** Google Ads CPC in Malaysia runs ~RM1.80 (F&B) to ~RM12.50 (legal/professional); most SMEs pay RM3–6 per click; CPCs rising ~8–12%/year; healthcare sits mid-range and climbing.[^2][^3] Agency-advertised lead costs "from ~RM20+" per lead for SME campaigns.[^30] Global healthcare search CPC averages USD ~5.64 (LocaliQ/WordStream family, US-weighted) — an upper anchor, not a Malaysian expectation.[^4]

**Welltech keyword-level expectations** — *(analyst estimates)*: interpolated from the Malaysian cross-industry band, competitive density observed per cluster ([seo.md](seo.md) §3), and value-per-patient logic (GLP-1 program LTV supports aggressive bidding by clinics):

| Keyword cluster | Est. CPC (RM) | Est. CPL→WhatsApp convo (RM) | Reasoning |
|---|---|---|---|
| weight loss clinic KL / klinik kurus | 4–9 | 30–80 | Most contested commercial cluster; aesthetic clinics bid hard |
| medical weight loss program | 3–7 | 25–60 | Narrower, program-intent; fewer bidders |
| BM weight terms (cara kurus + qualifiers) | 1.5–4 | 15–45 | High volume, lower advertiser density in BM |
| online doctor / doktor online | 2–5 | 20–50 | Platform bidders present but low-ARPU economics cap bids |
| health screening package | 3–8 | 30–90 | Hospital budgets; higher basket values |
| longevity/biological age | 1.5–4 | 20–60 | Near-zero auction density; volume is the constraint |
| Brand (welltech) | 0.5–1.5 | <10 | Standard brand economics |

Evidence grade: C (modelled). First-month live data supersedes this table; publish actuals into [funnels.md](funnels.md).

## 6. Campaign architecture: click-to-WhatsApp as the primary conversion

Welltech's operating model is WhatsApp-first ([../10-market-intelligence/malaysia-whatsapp-healthcare.md](../10-market-intelligence/malaysia-whatsapp-healthcare.md)); paid search should be engineered so the *conversion event is a WhatsApp conversation*, not a form fill.

1. **Google message assets (click-to-WhatsApp).** Search and Performance Max ads can carry a message asset routing users into WhatsApp with a pre-filled starter message; Google logs a "conversation started" conversion.[^31][^32][^33] Caveat: message-asset availability excludes some restricted-content verticals including certain healthcare content — eligibility must be tested per account/campaign; where unavailable, fall back to landing pages with prominent `wa.me` CTAs and offline-conversion upload.[^31][^33]
2. **Conversion plumbing.** Track: (a) conversation started (message asset), (b) `wa.me` click on landing pages, (c) offline import of qualified-lead and consult-booked stages from the CRM back into Google Ads (enhanced conversions for leads) so Smart Bidding optimises to consults, not clicks.[^34] Per-campaign WhatsApp deep-link parameters preserve source attribution inside the chat thread.
3. **Structure (launch):**
   - Campaign 1 — Brand (exact, all languages). Campaign 2 — Weight EN (program + clinic terms, KL/Klang Valley geo). Campaign 3 — Weight BM. Campaign 4 — Telehealth/consult. Campaign 5 — Screening/longevity. Chinese ad groups inside 2/5 initially (zh ad copy, zh landing pages).
   - Geo: Klang Valley launch radius matching service coverage; Penang/JB expansions follow clinical capacity.
   - Schedule to staffed WhatsApp hours; message ads answered in >15 min burn trust and budget *(operational rule from WhatsApp-healthcare dossier)*.
4. **Performance Max.** Use only after Search proves conversion volume (PMax needs conversion history and clean lead-quality signals; healthcare practitioners report PMax working for bookings when fed CRM-qualified conversions — US case data: 37–55% CPA/CPL improvements — but also warn against unmanaged lead-gen use).[^35][^36] Sensitive-category rules strip most audience-signal advantages for weight loss (§2.3), so PMax's edge here is inventory reach (YouTube/Discover/Maps), not targeting *(analysis)*. Gate: ≥50–100 conversions/month tracked before enabling; asset groups per service line; brand exclusions on.
5. **Creative rules (both regimes, §2.3 + §3):** service-and-support framing ("doctor-supervised weight management, monitored weekly on WhatsApp"), no drug names, no guarantees, no before/after, no testimonials, no price-comparison superlatives; BM creatives written natively, not translated.

## 7. Landing-page compliance patterns

The landing page is where Google policy, MASA/MAB, PHFSA, and PDPA intersect; it is also the top disapproval source in healthcare accounts.[^7][^15]

**Required elements (paid-traffic pages):**
- KKLIU approval number for any medicine/service-promotional content; facility registration details; named MMC-registered doctors[^17][^21][^22]
- No POM brand/generic names anywhere on ad-linked pages (§2.1); class-level language only ("prescription weight-loss medication, where clinically appropriate, prescribed after doctor assessment")
- Risk balance: eligibility criteria (BMI thresholds), side-effect disclosure, "individual results vary" — mirrors what MAB approves and what Google's unrealistic-claims rules require[^14][^15][^23]
- PDPA: consent notice at the WhatsApp handoff (chat begins a personal-data processing relationship); privacy policy linked; no health data into ad-platform pixels (align with sensitive-category rules)[^13]
- Transparent pricing of the *service* (consult fee, program fee) is permitted and converts; comparative price claims against named competitors are not[^23]

**Anti-patterns observed in the market** *(from competitor page review in [seo.md](seo.md) research)*: drug-brand-led landing pages with cart buttons, "dijamin turun Xkg" guarantees, before/after gallery pages — each is simultaneously a Google disapproval risk and a MASA/MAB offence. Do not copy the incumbents.

## 8. Negative keywords and brand defence

**Negative-keyword program (build at launch, review weekly):**
- *Policy-protective negatives*: all POM brand/generic names ("ozempic", "wegovy", "mounjaro", "saxenda", "semaglutide", "tirzepatide", "duromine") — broad/phrase match on program keywords will otherwise match drug queries and serve ads into restricted territory; this is the single most important list in the account *(analysis of §2.1 mechanics)*
- *Intent negatives*: free, percuma, kerajaan (government), klinik kesihatan (public clinics), jawatan kosong/vacancy/salary, murah + grey-market modifiers ("jual", "borong", "supplier"), DIY/side-effect-horror research terms as data dictates
- *Category negatives*: bariatric surgery (until offered), slimming centre brand terms (Marie France, London Weight) unless deliberately conquesting that demand with a medical-alternative message
- *Geo negatives*: out-of-coverage states; Singapore-intent queries ("Wegovy Singapore") that inflate spend without serviceable patients

**Brand defence:**
- Run an always-on exact-match brand campaign from day one: cheap (est. RM0.50–1.50 CPC, §5), protects the WhatsApp funnel entrance, and denies conquesting space. Competitor bidding on rivals' brands is legal and practised in healthcare PPC;[^37] expect aesthetic clinics or platforms to test Welltech's brand as it grows.
- Trademark "Welltech" (ad-copy use of a registered mark can be reported to Google); monitor via Auction Insights + Ads Transparency Center.[^1][^37]
- Conquesting *by* Welltech: bidding on "doctoroncall weight loss" or "ova alternative" is Google-legal (no mark in copy) but sits near MAB's comparative-advertising prohibition if copy implies comparison[^23] — restrict to neutral copy ("Doctor-led weight program, KL") and treat as an experiment, not a pillar.

## 9. Launch budget model (illustrative — every input is an assumption to be replaced by live data)

**Price anchors from prior dossiers:** teleconsult market price RM19.90–80; Welltech program assumed RM900–1,000/month bundled (market-anchored to OVA ~RM900 flat and Seimbang ~RM899; see [../10-market-intelligence/malaysia-weight-loss-market.md](../10-market-intelligence/malaysia-weight-loss-market.md) §9); assumed initial paid consult RM99; assumed median program duration 5 months → gross program revenue/start ≈ RM4,600–5,100, of which drug cost is the major COGS pass-through.

**Base case — month 4–6 steady state, RM30,000/month search spend:**

| Funnel stage | Rate (assumption) | Volume |
|---|---|---|
| Blended CPC | RM4.00 | 7,500 clicks |
| Click → WhatsApp conversation | 8% | 600 conversations |
| Conversation → paid consult | 25% | 150 consults |
| Consult → program start | 40% | 60 starts |
| **Paid-search CAC per program start** | | **RM500** |
| CAC / first-month program revenue | RM500 / ~RM950 | 0.53× |
| CAC / 5-month gross revenue | RM500 / ~RM4,800 | ~10% |

Rate provenance: click→conversation 8% assumes WhatsApp-CTA pages outperform form benchmarks (healthcare search conversion ~5–7% US[^4]; message-first flows reduce friction — *analyst assumption*); conversation→consult 25% and consult→start 40% are working hypotheses consistent with the Dermed case's 55% lead→patient on qualified leads[^24] with a haircut for colder program demand. Consult fee revenue (150 × RM99 ≈ RM14.9K) offsets ~half the media cost even before program starts.

**Sensitivity (CAC per program start):**

| | Conversation rate 5% | 8% | 12% |
|---|---|---|---|
| CPC RM3 | RM600 | RM375 | RM250 |
| CPC RM4 | RM800 | RM500 | RM333 |
| CPC RM6 | RM1,200 | RM750 | RM500 |

Even the worst modeled cell (RM1,200) is ~25% of 5-month gross revenue — paid search clears viability with wide margin *if* retention holds (retention economics live in [funnels.md](funnels.md)). The binding constraint is not CAC but *volume*: at Malaysian search volumes for program-intent terms, RM30K/month may exhaust efficient inventory in Klang Valley; incremental budget then goes to BM/zh expansion, screening/longevity terms, and Meta/social (out of scope here) rather than higher bids *(analysis)*.

**Ramp plan:** Month 1–2: RM10–15K/month, Search only, manual/enhanced CPC, gather CPC + conversation-rate truth. Month 3: enable Smart Bidding on offline-imported consult conversions. Month 4–6: scale to RM30K, add PMax if conversion-volume gate met (§6.4). Re-forecast CAC monthly against this table.

## 9a. 90-day launch plan and budget allocation

**Budget allocation by campaign (launch → steady state):**

| Campaign | Month 1–2 (RM12K/mo) | Month 3 (RM20K/mo) | Month 4–6 (RM30K/mo) | Primary conversion |
|---|---|---|---|---|
| 1. Brand (exact) | RM500 | RM750 | RM1,000 | WhatsApp conversation |
| 2. Weight EN (program/clinic) | RM5,000 | RM8,000 | RM10,500 | WhatsApp conversation |
| 3. Weight BM | RM3,000 | RM5,000 | RM8,000 | WhatsApp conversation |
| 4. Telehealth/consult | RM1,500 | RM2,250 | RM3,000 | Consult booking |
| 5. Screening/longevity | RM2,000 | RM3,000 | RM4,500 | Screening booking |
| 6. PMax (gated on §6.4) | — | RM1,000 test | RM3,000 | Offline-imported consults |

Allocation logic *(analyst design)*: weight clusters take ~60% because program LTV dwarfs consult/screening baskets; BM share rises over time as native-language creative and landing pages mature; PMax is a satellite, never the core, until lead quality is proven.

**90-day gate checklist:**

| Gate | Day | Pass criterion | Fail action |
|---|---|---|---|
| Policy survival | 14 | Zero disapprovals outstanding; message assets serving (or fallback live) | Rework creatives/landing pages before scaling |
| Cost truth | 30 | Observed blended CPC within 2× of §5 estimates | Re-model CAC; renegotiate keyword set |
| Conversation quality | 45 | ≥60% of conversations are in-scope patients (not job-seekers/suppliers) | Negative-keyword expansion; ad-copy qualification |
| Funnel truth | 60 | Conversation→consult ≥15% | Fix WhatsApp response time/scripts before adding spend ([../10-market-intelligence/malaysia-whatsapp-healthcare.md](../10-market-intelligence/malaysia-whatsapp-healthcare.md)) |
| Economics | 90 | CAC per program start ≤ RM900 (≈1 month program revenue) | Hold budget flat; shift mix to best cells of §9 sensitivity table |

## 9b. Settled-questions table (quick reference for the marketing team)

| Question | Answer | Basis |
|---|---|---|
| Can we bid on "Ozempic Malaysia"? | **No.** Prescription-drug terms barred from promotional ads/keywords/landing pages targeting MY | Google restricted drug terms[^5]; MASA POM prohibition[^17] |
| Can our paid landing page mention Wegovy? | **No** (promotional context). Use drug-class language | §2.1[^5][^6] |
| Can we bid on "weight loss clinic KL"? | **Yes** — service advertising; keep claims MAB-clean | §2.4, §3[^7][^23] |
| Can we bid on "ubat kurus"? | **Yes with care** — generic term, but ad copy must not promote a medicine; route to program page | §2.4 *(analysis)* |
| Do search ads need KKLIU approval? | Treat **yes** for anything promoting medicines/medical services; number carried on landing page; confirm mechanics with BPF in writing | §3[^17][^21][^22] |
| Can we retarget site visitors with weight-loss ads? | **No** — sensitive-category personalisation ban | §2.3[^13][^14] |
| Can we use before/after photos or testimonials? | **No** — banned by both Google weight-loss rules and MAB 3/2023 | §2.3, §7[^14][^23] |
| Can we advertise "online prescriptions delivered"? | **No** — prescription-drug-services restriction; no MY certification lane; frame as doctor consultation | §2.2[^10][^11] |
| Can we bid on competitor brand names? | Legal on Google (no mark in copy); MAB comparative-claim risk if copy implies comparison — neutral copy only, experiment-tier | §8[^23][^37] |
| Can we send paid traffic straight to WhatsApp? | **Yes** via message assets where eligible; else landing page with wa.me CTA; log "conversation started" as conversion | §6[^31][^32][^33] |

## 10. Verification plan

1. **Ads Transparency Center sweep (week 1, free):** query DoctorOnCall, Doctor Anywhere, OVA, Nexus, Glojas, CLEO, Alpro, IHH brands; catalogue live creatives, formats, and (where shown) regions.[^1]
2. **Geolocated SERP capture (week 1):** VPN/local device screenshots of the 40-keyword basket in [seo.md](seo.md) Appendix A; record sponsored slots, advertisers, ad copy, KKLIU presence on their landing pages.
3. **Keyword Planner + SEMrush/Ahrefs CPC pull (week 1–2):** replace §5 estimates with tool data for the 40 keywords; Keyword Planner from a Malaysian billing account gives auction-truth ranges.
4. **BPF/MAB written confirmation (week 2–4):** engage a Malaysian regulatory consultant to confirm KKLIU treatment of RSA text ads + landing-page number placement; file first creative batch.[^20][^21]
5. **Message-asset eligibility test (week 2):** build a compliant test campaign to confirm WhatsApp message assets serve for Welltech's category in Malaysia; document any restriction for fallback design.[^31]
6. **Ongoing:** monthly policy-change review (Google healthcare policy changelog) and LIU expiry-list check.[^5][^20]

## 11. Implications for Welltech — summary judgments

1. **The drug-term wall privatises brand demand to organic.** Paid search cannot capture "Ozempic Malaysia"; SEO must ([seo.md](seo.md)). Paid budget belongs on service/program/screening intent.
2. **Compliance is a bidding advantage, not a tax.** Competitors' guarantee-laden, drug-named funnels face both Google disapproval and MAB enforcement; Welltech's clean account compounds quality score and survives sweeps.
3. **WhatsApp-native conversion is the differentiator Google now supports natively** via message assets — most Malaysian clinic advertisers still buy form fills and phone calls; conversation-started optimisation is an executable edge today.
4. **Economics clear easily; volume is the ceiling.** Modeled CAC (RM250–750/start) versus RM4,600+ gross program revenue leaves room for aggressive early bidding to buy data; plan for search-inventory saturation in Klang Valley and pre-build BM/zh and longevity expansions.
5. **Expect the regime to tighten** — Google's Malaysian financial-services verification shows the localisation direction; a healthcare analogue and the coming Digital Health Act would both reward the operator already running KKLIU-approved, doctor-fronted, claim-clean campaigns.

---

## References

[^1]: Google, Ads Transparency Center, https://adstransparency.google.com/; Admapix, "Google Ads Transparency Center Guide", https://www.admapix.com/blog/ad-intelligence/google-ads-transparency-center-guide (accessed July 2026).
[^2]: ZenWeb, "Google Ads CPC Malaysia: What Each Industry Pays Per Click", https://zenweb.my/blog/google-ads-cpc-by-industry-malaysia/ (RM1.80–12.50 industry range; RM3–6 SME norm; 8–12%/yr inflation) (accessed July 2026).
[^3]: ZenWeb, "Google Ads Cost in Malaysia 2026: What You'll Actually Pay", https://zenweb.my/blog/google-ads-cost-malaysia/ (accessed July 2026).
[^4]: LocaliQ, "Healthcare Search Advertising Benchmarks for 16 Specialties", https://localiq.com/blog/healthcare-search-advertising-benchmarks/; WordStream, "Google Ads Benchmarks 2025", https://www.wordstream.com/blog/2025-google-ads-benchmarks (accessed July 2026).
[^5]: Google Advertising Policies Help, "Healthcare and medicines: Restricted drug terms", https://support.google.com/adspolicy/answer/15595717 (accessed July 2026).
[^6]: Search Engine Land, "Google Ads loosens prescription drug term restrictions for non-promotional use", https://searchengineland.com/google-certification-prescription-drug-advertising-463409; Faebl Studios, "Google Ads Policy Update: New Prescription Drug Advertising Rules (Effective October 2025)", https://faeblstudios.com/resources/google-ads-policy-update-what-healthcare-clinics-need-to-know-about-new-prescription-drug-advertising-rules-effective-october-2025/ (accessed July 2026).
[^7]: Google Advertising Policies Help, "Healthcare and medicines", https://support.google.com/adspolicy/answer/176031 (accessed July 2026).
[^8]: Accelerated Digital Media, "2026 Search Advertising Rules for Health Brands: Policy Guide for Google Ads & Microsoft", https://www.accelerateddigitalmedia.com/insights/health-policies-and-restrictions-guide-for-google-ads-microsoft-ads-2026/ (accessed July 2026).
[^9]: Brandmed, "5 Most Common Google Ads Restrictions for Pharma", https://brandmed.com/blog/marketing/5-most-common-google-ads-restrictions-for-pharma-everything-you-need-to-know (online-pharmacy country list excluding Malaysia; Malaysia birth-control prohibition) (accessed July 2026).
[^10]: Google Ads Help, "Apply for healthcare-related advertising", https://support.google.com/google-ads/troubleshooter/6099627; Google Advertising Policies Help, "Prescription drug services", https://support.google.com/adspolicy/answer/15598647 (accessed July 2026).
[^11]: LegitScript, "Healthcare Certification", https://www.legitscript.com/certification/healthcare-certification/; LegitScript press, "Certification for Telemedicine Businesses Now Recognized by Google in Indonesia and the Philippines", https://www.legitscript.com/about/press/legitscript-telehealth-certification-indonesia-philippines/; Business Wire, "LegitScript Certification Now Recognized by Google for Pharmacies in India and Telemedicine Providers in New Zealand", https://www.businesswire.com/news/home/20260408837286/en/ (accessed July 2026).
[^12]: SoyaCincau, "Google Ads to enforce mandatory verification for financial services ads in Malaysia from 14 April", https://soyacincau.com/2026/03/11/google-ads-mandatory-verification-financial-ads-in-malaysia/ (accessed July 2026).
[^13]: Google Advertising Policies Help, "Restricted targeting in Personalized advertising", https://support.google.com/adspolicy/answer/143465; "Health in personalized advertising", https://support.google.com/adspolicy/answer/16701855 (accessed July 2026).
[^14]: Blockchain-Ads, "How to Run Compliant Weight Loss Ads on Google: Policies, Setup & Best Practices", https://www.blockchain-ads.com/post/weight-loss-ads-on-google (accessed July 2026).
[^15]: EHM Results, "Google Ads Healthcare Policies: Guide to Compliance", https://ehmresults.com/google-ads-not-generating-patients-it-could-be-healthcare-policies/ (accessed July 2026).
[^16]: Google Advertising Policies Help, "Document requirements for advertiser verification — Malaysia", https://support.google.com/adspolicy/answer/9872280?co=GENIE.CountryCode%3DMY; Silver Mouse, "Guide to Google advertiser verification in Malaysia", https://www.silvermouse.com.my/blog/google-advertiser-verification-guide-malaysia/ (accessed July 2026).
[^17]: Medicine Advertisements Board / Pharmaceutical Services Programme, "Guideline on Advertising of Medicines and Medicinal Products to General Public", https://pharmacy.moh.gov.my/sites/default/files/document-upload/latest-guideline-advertising-medicines-and-medicinal-products-general-public.pdf; see [../10-market-intelligence/malaysia-regulations.md](../10-market-intelligence/malaysia-regulations.md) §6 for the full MASA 1956/KKLIU analysis (accessed July 2026).
[^18]: Kosmo, "Iklan ubat tidak sah di platform internet diturunkan" (20 Nov 2025; RM120M fines; platform takedowns; TikTok Live warnings), https://www.kosmo.com.my/2025/11/20/iklan-ubat-tidak-sah-di-platform-internet-diturunkan/ (accessed July 2026).
[^19]: Pharmaceutical Services Programme, MOH, "How to recognize approved advertisement?", https://pharmacy.moh.gov.my/en/content/how-recognize-approved-advertisement.html; "Beware of Illegal Advertisements", https://www.pharmacy.gov.my/v2/en/news/04-dec-2012/beware-illegal-advertisements.html (accessed July 2026).
[^20]: Pharmaceutical Services Programme, MOH, "Iklan Tamat Tempoh Kelulusan Lembaga Iklan Ubat (LIU) 2025", https://pharmacy.moh.gov.my/ms/berita/05-dis-2025/iklan-tamat-tempoh-kelulusan-lembaga-iklan-ubat-liu-2025.html; "Semakan Kelulusan Iklan daripada Lembaga Iklan Ubat", https://www.pharmacy.gov.my/v2/ms/apps/iklan (accessed July 2026).
[^21]: Lamanify, "KKLIU Guideline: Advertising Medicines & Medicinal Products", https://www.lamanify.com/guide/kkliu-guideline; Lamanify, "Healthcare Marketing in Malaysia: A Guide to Building Trust and Attracting Patients", https://www.lamanify.com/blog/healthcare-marketing-in-malaysia-a-guide-to-building-trust-and-attracting-patients (accessed July 2026).
[^22]: Disruptive Doctors, "KKLIU Regulations: A Doctor's Guide to Ethical Healthcare Marketing in Malaysia", https://disruptive-doctors.com/kkliu-advertising-guidelines-malaysia/; Bioprestige, "Medicine Advertisements Board (MAB) (KKLIU): Regulating Medical Advertising in Malaysia", https://bioprestige.my/medicine-advertisements-board-mab-regulating-medical-advertising-malaysia/ (accessed July 2026).
[^23]: Medicine Advertisements Board, "Advertising Guidelines for Healthcare Facilities and Services" (rev. 3/2023), https://pharmacy.moh.gov.my/sites/default/files/document-upload/advertising-guidelines-healthcare-facilities-and-services-mab-3.2023.pdf; MCMC, "Content Industry Reference: Health Claim Advertisements", https://www.mcmc.gov.my/skmmgovmy/media/General/pdf/Content-Industry-Reference-Health-Claim-Advertisements.pdf (accessed July 2026).
[^24]: Omnicore Agency, "Aesthetic Clinic Google Ads/PPC Case Study: Dermed Clinic" (Johor Bahru; 103 leads, 57 patients, 55.34% conversion), https://www.omnicoreagency.com/case-studies/dermed-clinic-google-ads-ppc/ (accessed July 2026).
[^25]: MYSense, "How Google Ads Agency Malaysia Help Aesthetic Clinics", https://mysense.com.my/how-google-ads-agency-malaysia-help-aesthetic-clinics/; ZenWeb, "Best Digital Marketing for Aesthetic Clinic in Malaysia Guide 2026", https://zenweb.my/industries/aesthetic-clinic/digital-marketing/ (accessed July 2026).
[^26]: OVA, https://getova.com.my/; OVA Instagram (@get.ova), https://www.instagram.com/get.ova/ (accessed July 2026).
[^27]: Lamanify, https://www.lamanify.com/ (healthcare websites, booking, AI WhatsApp assistants, SEO/Google Ads for Malaysian clinics) (accessed July 2026).
[^28]: Holland & Knight, "FDA, HHS Taking Action Against Telehealth's Compounded Drug Advertising" (Sept 2025), https://www.hklaw.com/en/insights/publications/2025/09/fda-hhs-taking-action-against-telehealths-compounded-drug-advertising; Patient Care Online, "FDA Issues Warning Letters to 30 Telehealth Companies Over Misleading Compounded GLP-1 RA Marketing" (Feb 2026), https://www.patientcareonline.com/view/fda-issues-warning-letters-30-telehealth-companies-over-misleading-compounded-glp-1-ra-marketing (accessed July 2026).
[^29]: eMarketer, "Hims' copycat GLP-1 gamble backfires" (GLP-1 = ~37% of H1 2025 revenue; Novo lawsuit Feb 2026), https://www.emarketer.com/content/hims--glp-1-growth-engine-gets-rattled-by-novo-lawsuit-regulatory-scrutiny; Frier Levitt, "FDA Warning Letters and Hims–Novo Nordisk Deal", https://www.frierlevitt.com/articles/fda-warning-letters-hims-novo-nordisk-compounded-glp1/ (accessed July 2026).
[^30]: TREEY, "Harga Iklan di Google Ads", https://treey.my/pages/harga-iklan-google-ads; iTrobes, "How Much Does Digital Marketing Cost In Malaysia?", https://www.itrobes.com/digital-marketing-price-malaysia/ (accessed July 2026).
[^31]: Google Ads Help, "About message assets", https://support.google.com/google-ads/answer/14888522 (accessed July 2026).
[^32]: Search Engine Land, "WhatsApp in Google Ads: Everything you need to know about Message Assets", https://searchengineland.com/whatsapp-google-ads-message-assets-450630; SleekFlow, "What is Google Message Asset and how to set up click-to-WhatsApp ads", https://sleekflow.io/blog/google-click-to-whatsapp-ads (accessed July 2026).
[^33]: ALM Corp, "Google Ads Adds 'Messages from Your Ads' in Search", https://almcorp.com/blog/google-ads-messages-from-your-ads-search/ (restricted-content categories including healthcare noted) (accessed July 2026).
[^34]: Pete Bowen, "Tracking WhatsApp leads as conversions in Google Ads", https://pete-bowen.com/tracking-whatsapp-leads-as-conversions-in-google-ads (accessed July 2026).
[^35]: Cardinal Digital Marketing, "Mastering Performance Max (PMAX) for Healthcare", https://www.cardinaldigitalmarketing.com/healthcare-resources/blog/performance-max-pmax-healthcare-guide/; UpMedico, "Google PMax Optimizations for Healthcare Providers", https://upmedico.com/google-pmax-optimizations-for-healthcare-providers/ (accessed July 2026).
[^36]: PPC.live, "How to improve your lead quality on Performance Max", https://ppc.live/library/strategy/how-to-improve-your-lead-quality-on-performance-max/ (accessed July 2026).
[^37]: Adthena, "PPC Brand Bidding: The Complete Guide", https://www.adthena.com/resources/blog/complete-guide-to-ppc-brand-bidding/; Brick Mortar Digital, "Healthcare PPC: What Bidding for Patients Actually Looks Like", https://www.brickmortardigital.com/blog/digital-marketing/healthcare-ppc-what-bidding-for-patients-actually-looks-like/; GrowLeads, "Bidding on Competitor Keywords in Google Ads", https://growleads.io/blog/is-bidding-on-competitor-keywords-legal-the-truth-about-brand-bidding/ (accessed July 2026).
