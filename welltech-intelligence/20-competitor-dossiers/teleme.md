# Teleme — Competitor Dossier

**Abstract.** Teleme (teleme.co, TeleMe Technologies, Kuala Lumpur) is a small Malaysian telehealth platform founded 2015–2016 by Dr Aqeel Ahmad, Mark Choo and ophthalmologist Dr Hoh Hon Bing. It markets itself as "Malaysia's first integrated telemedicine platform": chat/voice/video consultations with named doctors and specialists, regulator-compliant e-prescriptions dispensed via licensed pharmacies, lab-test ordering, health screening packages and medication delivery. It was grant-funded (Cradle RM300K, MaGIC accelerator) rather than VC-backed, and remains a niche operator — roughly 44,000 lifetime Android downloads — whose most notable recent move is a B2B pivot: powering an e-Pharmacy teleconsultation app for Telekom Malaysia's Unifi Business, targeting independent pharmacies. Unlike most first-generation Malaysian health platforms, its app is still actively updated (January 2026). Teleme's specialist-continuity, e-prescription and lab-integration mechanics are directly relevant to Welltech's clinical workflows; its scale is not.

Last updated: July 2026

Related: [BookDoc dossier](bookdoc.md) · [GetDoc dossier](getdoc.md) · [Malaysia market intelligence](../10-market-intelligence/malaysia-market-intelligence.md)

---

## 1. Company overview & history

| Item | Detail |
|---|---|
| Entity / brand | TeleMe Technologies, Kuala Lumpur, Malaysia[^1][^2] |
| Founded | 2015–2016 (sources conflict: CB Insights says 2016; Vulcan Post's account and Dr Hoh's CMO tenure point to 2015 origins, market launch 2016)[^2][^3][^4] |
| Founders | Dr Aqeel Ahmad (co-founder, physician trained in Ireland), Mark Choo (co-founder & CEO), Dr Hoh Hon Bing (ophthalmologist; Chief Medical Officer, involved since 2015)[^3][^4][^5] |
| Early support | MaGIC Global Accelerator Programme (GAP), 2017 cohort (54 startups); Cradle Fund grant RM300,000[^3][^5] |
| Market | Malaysia (platform claims usability "from anywhere in the world" for follow-ups)[^6] |
| Provider claim | "500+ licensed health practitioners" (company figure — see §5)[^6][^7] |
| Status (July 2026) | Active: app v1.2.47 released 13 January 2026; TM Unifi B2B partnership live[^8][^9] |

### Timeline

- **2015–2016** — Founded; motivation per Dr Aqeel: long waits and misallocated urgent-care attention observed during medical training in Ireland; Dr Hoh joins as CMO to give clinical credibility.[^3][^4]
- **2017** — Selected into MaGIC's inaugural GAP accelerator (Mark Choo interviewed on BFM); Cradle RM300K grant follows; product features largely shaped in this period.[^3][^5]
- **2018–2021** — Builds out integrated stack: chat/voice/video consults, e-prescriptions, pharmacy dispensing, PathLab-type lab integrations, health screening packages, medication delivery; markets itself to both patients and employers.[^6][^7][^2]
- **2023** — B2B milestone: Telekom Malaysia's Unifi Business launches an e-Pharmacy app developed with Teleme Technologies — teleconsultation + e-prescription tooling bundled with business broadband for MSME pharmacies, with government GDPM digitalisation rebates up to 50%; pitched at rural/underserved communities; "over 500 licensed healthcare professionals" accessible.[^9][^10][^11]
- **2024–2026** — Continues incremental app releases (v1.2.38 Jun 2024, v1.2.39 Aug 2024, v1.2.43 Feb 2025, v1.2.47 Jan 2026).[^8]

## 2. Founders & leadership

- **Mark Choo — CEO.** Public face for accelerator/startup media (BFM interview on MaGIC GAP selection).[^5]
- **Dr Aqeel Ahmad — co-founder.** Physician; origin-story carrier (Irish training, frustration with waiting-time triage).[^3]
- **Dr Hoh Hon Bing — Chief Medical Officer.** Senior LASIK/refractive ophthalmologist, involved since 2015; practices on the platform himself and evangelises telemedicine to Malaysian doctors via Disruptive Doctors/Medic Footprints webinars — i.e., the CMO doubles as the doctor-acquisition channel.[^4][^12]
- No leadership changes, departures or new executive hires surfaced in searches — a stable, founder-run micro-team. *(inference)*

## 3. Funding & investors

- **Cradle Fund grant: RM300,000** (announced November, post-GAP 2017).[^3]
- **MaGIC GAP** accelerator support (non-dilutive/programmatic).[^3][^5]
- No VC rounds recorded on PitchBook/Tracxn/CB Insights profiles; no valuation data exists.[^13][^1][^2]
- **Analytical note:** Teleme is a grant-and-revenue company. Ten years in, its ceiling has been set by capital: it survived where peers died, but could never buy growth. Its unit economics must be roughly self-sustaining at very low volume, implying a lean cost base and doctor-pays/patient-pays revenue rather than subsidised pricing.

## 4. Business model & revenue streams

1. **Consultation fees (patient-pays).** Practitioners set their own rates; observed range ~RM10–20 per chat/video session — dramatically cheaper than clinic visits, implying Teleme's cut is small in absolute terms.[^7]
2. **Pharmacy & delivery.** E-prescriptions fulfilled by MOH-licensed local pharmacies with medication delivery or collection; Teleme claims to be one of only two health-tech platforms with Lembaga Farmasi (Pharmacy Board)-compliant e-prescription features — a company claim worth verifying but plausible given the TM pharmacy product.[^7][^6]
3. **Lab tests & health screening packages.** Doctors order labs in-app; patients pay online; results return to the ordering doctor; screening packages sold directly.[^7][^6]
4. **B2B/enterprise.** Employer offerings (screenings, teleconsult access)[^2]; white-label/platform licensing — the TM Unifi e-Pharmacy app is effectively Teleme-as-infrastructure sold through a telco channel.[^9][^10]
5. **Payments** via iPay88 and Billplz gateways (online banking, cards).[^7]

## 5. Product & clinical workflow

**Patient flow:** download app / web → choose a specific named doctor or practitioner (directory includes specialists, pharmacists, labs) → text chat, voice or video consult (response "within minutes to a few hours" — asynchronous-first, not on-demand queue) → e-prescription → licensed pharmacy dispenses, delivery or pickup → labs ordered/paid in-app with results returned to the doctor → longitudinal health records and medication reminders in-app.[^6][^7]

Key differentiators vs. queue-based telehealth (DoctorOnCall-style):

- **Continuity with named clinicians**, including consultant specialists (e.g., ophthalmology follow-ups) rather than anonymous GP pools — suited to chronic-disease monitoring and post-op review.[^4][^6]
- **Regulated e-prescription + community-pharmacy dispensing** rather than in-house pharmacy — the asset that made the TM pharmacy partnership possible.[^7][^9]

**Network claims — treat skeptically.** "500+ licensed health practitioners" is a company figure repeated since at least the TM launch; directory listing ≠ active supply. With ~44K lifetime app downloads, active practitioner count is plausibly an order of magnitude lower.[^6][^9][^8] *(analyst estimate)*

## 6. Technology & AI

- Patient app `com.teleme.teleme` (Android, iOS id1323899039); separate practitioner app "Teleme Health Practitioner" (Android `co.teleme.telemehp`, iOS id1609930264) — a proper two-sided clinical tooling split.[^14][^8]
- Update cadence: consistently maintained; latest v1.2.47 on 13 Jan 2026.[^8]
- Digital-signature support for e-prescriptions (via the TM e-Pharmacy build).[^9]
- **No AI features** claimed anywhere (no triage bots, no LLM assistants). **No WhatsApp workflow** — consults run inside the proprietary app's chat/voice/video.[^7][^15]

## 7. Marketing & positioning

- Positioning line: "Malaysia's first integrated telemedicine platform" / "#1 healthcare app" — both unverifiable superlatives; the "integrated" claim (consult + prescription + pharmacy + labs in one loop) is the legitimate core.[^6]
- **Content/SEO:** teleme.co carries doctor profile pages, FAQ, and a health-tips blog (blog.teleme.co) with doctor-authored content — modest but real organic surface.[^16][^4]
- **Doctor-side marketing:** practitioner sign-up funnel on site; CMO-led webinars targeting doctors (Disruptive Doctors, Medic Footprints) as a supply-acquisition channel.[^17][^12]
- **PR:** thin — Vulcan Post (2018-era), Digital News Asia scepticism piece, then the 2023 TM announcement wave (TM newsroom, Developing Telecoms, Telecom Review Asia, Asian Wireless Communications).[^3][^18][^9][^10][^11]
- Included in third-party "best telemedicine apps in Malaysia" roundups alongside DoctorOnCall, Doc2US, Doctor2U — present in the consideration set but never the headline player.[^15][^19]

## 8. Reviews & reputation

- **Android installs:** ~44,000 lifetime; ~49 downloads/day recent average; **no meaningful rating volume** on AppBrain (too few reviews to score) — confirmation of niche scale.[^8]
- No significant Reddit/Lowyat presence, complaint threads, or press criticism found; equally, no organic user advocacy. *(absence-of-evidence finding, July 2026)*
- Regulatory reputation is a relative strength: Pharmacy Board-compliant e-prescriptions and MOH-licensed dispensing are cited in its own materials and echoed by the TM partnership's legitimacy.[^7][^9]
- Malaysian telehealth press (The Edge, CodeBlue) consistently names DoctorOnCall, Doc2US and Qmed Asia — not Teleme — as the market drivers; Teleme is at the periphery of the narrative.[^19][^20]

## 9. SWOT

| | |
|---|---|
| **Strengths** | Genuine end-to-end clinical loop (consult → e-Rx → pharmacy → labs → records); named-specialist continuity model; regulatory compliance as differentiator; still shipping product (Jan 2026); telco enterprise channel via TM; clinician-founder credibility |
| **Weaknesses** | Tiny scale (~44K downloads, negligible review base); no growth capital ever raised; low brand salience; asynchronous response times ("minutes to hours") unsuited to acute on-demand care; consult pricing (RM10–20) caps take-rate revenue; no AI leverage |
| **Opportunities** | Chronic-disease monitoring programmes with specialists; more white-label infrastructure deals (TM template: insurers, pharmacy chains, state health programmes); Digital Health Act-era compliance positioning[^20] |
| **Threats** | DoctorOnCall/Doc2US scale and funding; hospital groups launching own teleconsult; TM partnership concentration risk; platform commoditisation as e-prescription compliance becomes table stakes under the coming Digital Health Act[^20] |

## 10. Current status assessment

**Verdict: alive and quietly functional — a sustainable micro-business, not a growth company.** Positive signals: app releases through January 2026[^8]; a credible 2023 enterprise partnership with Telekom Malaysia that implies working, certifiable technology[^9]. Limiting signals: no funding events in a decade, no download momentum (~49/day), no press since the TM launch cycle, founder-scale team. Teleme has effectively become telehealth infrastructure with a small direct-to-patient storefront attached.

## 11. Implications for Welltech

1. **Teleme validates the exact clinical loop Welltech needs — at hobbyist scale.** Consult → compliant e-prescription → licensed pharmacy dispensing → labs → longitudinal records is precisely the chassis for GLP-1 weight-loss and longevity programmes. Teleme proves it's regulatorily buildable in Malaysia by a tiny team; Welltech's edge must come from programme design (structured weight-loss/longevity protocols), WhatsApp-native UX, and AI-driven operations, none of which Teleme has.
2. **Named-clinician continuity beats anonymous GP queues for chronic/longitudinal care.** Teleme's specialist-follow-up model (championed by an ophthalmologist CMO) is the right pattern for Welltech's medically supervised weight-loss and preventive-medicine journeys — retain it, but wrap it in concierge coordination.
3. **Compliance is a marketable asset.** Teleme extracted a Telekom Malaysia partnership largely off Pharmacy Board-compliant e-prescription capability. With Malaysia's Digital Health Act targeted for 2026, early compliance investment will convert into B2B distribution deals — Welltech should treat regulatory tooling as sales collateral, not overhead.[^20]
4. **Beware the RM10–20 consult trap.** Pricing telehealth as a cheap commodity consult (Teleme's range) makes venture-scale economics impossible. Welltech's monetisation should sit in programmes, medication cycles and memberships, with consults bundled — not sold à la carte at GP-visit-minus prices.
5. **Partnership watchlist.** If Welltech needs rapid e-prescription/pharmacy rails in Malaysia, Teleme is a plausible acquisition or white-label partner: proven stack, no capital, likely open to enterprise revenue (as the TM deal shows).

---

## References

[^1]: PitchBook, "Teleme 2026 Company Profile", https://pitchbook.com/profiles/company/294497-02; Tracxn, "Teleme - 2025 Company Profile", https://tracxn.com/d/companies/teleme/__Scwe-qFbEjsC5fBCOjvkQwym_x9ij9ChZL0PNeFOWTQ (accessed July 2026).
[^2]: CB Insights, "TeleMe - Products, Competitors, Financials" (KL base; founded 2016; services incl. virtual consultations, e-prescriptions, health screenings, records; individual + employer customers), https://www.cbinsights.com/company/teleme and https://www.cbinsights.com/company/teleme/people (accessed July 2026).
[^3]: Vulcan Post, "Teleme Is A Malaysian Healthcare Startup For Virtual Doctor Consultations" (Dr Aqeel origin story; MaGIC GAP 2017; Cradle RM300K grant), https://vulcanpost.com/631850/teleme-healthcare-startup-malaysia/ (accessed July 2026).
[^4]: Teleme, "Who We Are", https://teleme.co/about-us; Teleme doctor profile, "Dr. Hoh Hon Bing - Ophthalmologist (LASIK and refractive)", https://teleme.co/doctors/profile/dr-hoh-hon-bing; Healthtech Alpha person profile, https://www.healthtechalpha.com/person/hoh-hon-bing (accessed July 2026).
[^5]: MaGIC Central, "TeleMe" organisation profile (GAP cohort; BFM interview with CEO Mark Choo, July 2017), https://central.mymagic.my/network/organization/1520/TeleMe (accessed July 2026).
[^6]: Teleme homepage, "Talk To Health Practitioners Online & Get Your Medication" ("Malaysia's first integrated telemedicine platform"; 500+ practitioners; doctors/pharmacies/PathLab centres), https://teleme.co/ (accessed July 2026).
[^7]: Teleme, "Frequently Asked Questions (FAQ)" (chat/voice/video; response times; RM10–20 consult range; iPay88/Billplz; Lembaga Farmasi-compliant e-prescription claim; MOH-licensed pharmacy dispensing; in-app lab ordering), https://teleme.co/faq (accessed via search excerpts, July 2026).
[^8]: AppBrain, "Teleme for Android" (~44K downloads; ~49/day; no rating volume; last update 13 Jan 2026, v1.2.47), https://www.appbrain.com/app/teleme/com.teleme.teleme; Uptodown/APKCombo version history (v1.2.38 Jun 2024; v1.2.39 Aug 2024; v1.2.43 Feb 2025), https://com-teleme-teleme.en.uptodown.com/android and https://apkcombo.com/teleme/com.teleme.teleme/download/apk (accessed July 2026).
[^9]: Telekom Malaysia newsroom, "TM revolutionises digital healthcare services with next gen e-Pharmacy solution" (Unifi Business × Teleme Technologies; 500+ licensed professionals; digital signature; GDPM rebates up to 50%; rural/underserved focus), https://www1.tm.com.my/news/digital_healthcare_services_with_next_gen_epharmacy_solution (accessed July 2026).
[^10]: Developing Telecoms, "Telekom Malaysia app streamlines prescriptions for pharmacies", https://developingtelecoms.com/telecom-technology/enterprise-ecosystems/16433-telekom-malaysia-app-streamlines-prescriptions-for-pharmacies.html; Telecom Review Asia Pacific, "Telekom Malaysia Transforms Digital Healthcare Services", https://www.telecomreviewasia.com/news/service-news/4075-telekom-malaysia-transforms-digital-healthcare-services (accessed July 2026).
[^11]: Asian Wireless Communications, "Telekom Malaysia's Unifi Business unit launches e-Pharmacy app", https://asianwirelesscomms.com/news-details?itemid=7494 (accessed July 2026).
[^12]: Disruptive Doctors, "Telemedicine with Dr Hoh Hon Bing" (webinar for doctors on telemedicine platforms), https://disruptive-doctors.com/telemedicine-with-dr-hoh-hon-bing/; Medic Footprints mirror, https://medicfootprints.org/telemedicine-with-dr-hoh-hon-bing/ (accessed July 2026).
[^13]: Cradle Fund, corporate site (grant programme context), https://www.cradle.com.my/ (accessed July 2026).
[^14]: Google Play, "Teleme" (com.teleme.teleme) and "Teleme Health Practitioner" (co.teleme.telemehp), https://play.google.com/store/apps/details?id=com.teleme.teleme and https://play.google.com/store/apps/details?id=co.teleme.telemehp; Apple App Store, "Teleme App" (id1323899039), https://apps.apple.com/my/app/teleme/id1323899039, and "Teleme Health Practitioner" (id1609930264), https://apps.apple.com/us/app/teleme-health-practitioner/id1609930264 (accessed July 2026).
[^15]: Pacific Prime, "Telemedicine & Virtual Care: Malaysian Expat Options" (names DoctorOnCall, BookDoc, Teleme, DOC2US, Doctor2U as trusted providers), https://www.pacificprime.com/blog/telemedicine-virtual-care-malaysia-expat-options.html (accessed July 2026).
[^16]: Teleme blog, "Healthtips by TeleMe — Dr. Hoh Hon Bing", https://blog.teleme.co/doctors/dr-hoh-hon-bing/; Teleme doctor search, https://teleme.co/doctors/search (accessed July 2026).
[^17]: Teleme, "Doctor / Practitioner Sign Up", https://teleme.co/doctors/signup (accessed July 2026).
[^18]: Digital News Asia, "Scepticism still surrounds medical technology" (Malaysian medtech adoption context incl. Teleme-era platforms), https://www.digitalnewsasia.com/business/scepticism-still-surrounds-medical-technology (accessed July 2026).
[^19]: The Edge Malaysia, "Cover Story: Next step for digital healthcare" (private teleconsult growth driven by DoctorOnCall, Doc2Us, Qmed Asia), https://theedgemalaysia.com/node/756278; Doc2US, "Best Telemedicine Apps in Malaysia", https://www.doc2us.com/newsroom/best-telemedicine-apps-in-malaysia (accessed July 2026).
[^20]: CodeBlue (Galen Centre), "Stepping Into Digital Health Care Through Telemedicine — Yap Yoong Hong & Dr Sean Thum", Mar 2024 (376 government clinics with virtual consults; MOH digital health division; Digital Health Act targeted 2026), https://codeblue.galencentre.org/2024/03/stepping-into-digital-health-care-through-telemedicine-yap-yoong-hong-dr-sean-thum/ (accessed July 2026).
