# Quantitative Datasets & Statistical Sources Index

An index of the datasets and statistical sources that underpin the numbers throughout the Welltech Intelligence repository — demographics, disease prevalence, digital connectivity, market sizing, company financials and price benchmarks. For each: the dataset, its publisher, coverage/year, the key figures it provides, which repository documents rely on it, and any verification caveats flagged during the research.

**Last updated: July 2026**

Full citations are in [bibliography.md](bibliography.md); every URL is in [links.md](links.md); regulatory instruments are in [regulations.md](regulations.md).

> **General verification caveat.** Market-size estimates for the same segment diverge widely across vendors (e.g. Malaysia telehealth ranges from ~USD 1.1B to ~USD 1.85B for overlapping years depending on scope). The repository reconciles ranges rather than picking one figure; treat any single number below as the low or high bound of a reconciled range and check the source scope. Several government survey PDFs were read via search-indexed content rather than direct download.

## Reading guide

| Type | Datasets |
|---|---|
| Population & demography | DOSM (MY), Singstat (SG), C&SD (HK), life tables, household income |
| Disease prevalence | NHMS (MY), NPHS (SG), Population Health Survey (HK), World Obesity Atlas, IDF Diabetes Atlas, WHO GHO |
| Digital & connectivity | DataReportal Digital ×3 markets, MCMC surveys |
| Market sizing | Grand View, Ken Research, Mordor, Data Bridge, Maximize, Research and Markets, Statista |
| Company financials | IHH, KPJ, Sunway, EC Healthcare, Prenetics, Fullerton, Qualitas |
| Price benchmarks | GLP-1 street/clinic pricing (all three markets) |

---

## 1. Population & demographic datasets

| Dataset | Publisher | Coverage / year | Key figures | Relied on by | Caveats |
|---|---|---|---|---|---|
| **Current Population Estimates 2025** + Population Dashboard | DOSM / OpenDOSM | Malaysia, 2025 | Total population; peak ~42m in 2059 | `10`, `00` | Search-indexed |
| **Abridged Life Tables 2024 / 2025** | DOSM | Malaysia | Life expectancy ~75.2 yrs | `10` | — |
| **Household Income Survey Report 2022** | DOSM | Malaysia & states, 2022 | Median household income by state (Selangor/Penang/Johor above national) | `10` | — |
| **Demographic Statistics (Q3 2024)** + ethnicity breakdown | DOSM | Malaysia | Population by ethnicity; ageing-nation by 2030 / aged by ~2048 | `10` | Ageing dates via press (Malay Mail, MOF) |
| **GDP dashboard / IMF DataMapper / World Bank** | DOSM, IMF, World Bank | Malaysia | GDP per capita; urbanization % | `10` | Cross-checked across three sources |
| **National Population Health Survey (SG)** — demographic modules | MOH SG / HPB | Singapore | Population health & lifestyle | `10` | See disease section |
| **Census & Statistics Department tables** (e.g. 930-92083) | C&SD Hong Kong | Hong Kong | Population; medical institutions with hospital beds | `10` | — |
| **Population.gov.sg / Singstat** | NPTD / Singstat | Singapore | Resident population, ageing | `10` | — |

---

## 2. Disease-prevalence datasets (obesity, diabetes, NCDs, mental health)

| Dataset | Publisher | Coverage / year | Key figures | Relied on by | Caveats |
|---|---|---|---|---|---|
| **National Health & Morbidity Survey (NHMS) 2023** — Fact Sheet | Institute for Public Health (IKU/NIH), MOH Malaysia | Malaysia, 2023 | >50% of adults overweight/obese; >2m adults with 3 NCDs; depression prevalence up since 2019 | `10`, `00`, `20`, `50` | **The anchor dataset for MY obesity claims.** Primary PDF read via search-indexed content; corroborated by CodeBlue, Free Malaysia Today, Nature *Scientific Reports* methodology paper |
| **NHMS 2019 / 2015 / Adolescent Health Survey 2022** | IKU/NIH, MOH Malaysia | Malaysia, various | Overweight determinants; health literacy (n=9,478); teen obesity ~⅓; T&CM utilization | `10`, `40`, `50` | Accessed via peer-reviewed secondary analyses (PLOS ONE, PMC, Karger) |
| **National Population Health Survey (NPHS) 2023 & 2024** | MOH Singapore / Health Promotion Board | Singapore | Obesity rising; lifestyle-behaviour trends | `10`, `00` | Full 2024 report PDF (isomer-hosted) |
| **Population Health Survey 2020–22 (Parts I & II)** | Centre for Health Protection, DH Hong Kong | Hong Kong, 2020–22 | Obesity 32.6%, overweight 22.0% (ages 15–84); age-standardised overweight+obesity 51.3% (18–84) | `10`, `00` | — |
| **World Obesity Atlas 2023** | World Obesity Federation | Global incl. 3 markets | Obesity prevalence & projections | `10`, `00` | PDF (V5) |
| **IDF Diabetes Atlas** + member pages | International Diabetes Federation | Global incl. 3 markets | Diabetes prevalence (GLP-1 addressable base) | `10`, `50` | — |
| **WHO Global Health Observatory** | World Health Organization | Global | NCD & health-system indicators | `10`, `40` | — |

---

## 3. Digital connectivity & behaviour datasets

| Dataset | Publisher | Coverage / year | Key figures | Relied on by | Caveats |
|---|---|---|---|---|---|
| **Digital 2025 / 2026: Malaysia** | DataReportal (We Are Social / Meltwater) | Malaysia, early 2025 & 2026 | 34.9m internet users (97.7% penetration); Facebook 23.1m; Instagram 15.5m; Messenger reach 11.1m | `10`, `50` | Also Digital 2024 for trend |
| **Digital 2026: Singapore** | DataReportal | Singapore | Internet/social penetration | `10`, `50` | — |
| **Digital 2026: Hong Kong** | DataReportal | Hong Kong | 7.16m internet users (96.8%); 6.24m social identities (84.4%) | `10`, `50` | — |
| **MCMC Internet Users Survey / Hand Phone Users Survey 2021** | Malaysian Communications & Multimedia Commission | Malaysia | Connectivity; WhatsApp = favourite app of 97.7% of users (via Statista/MCMC) | `10`, `50` | WhatsApp-first thesis anchor |
| **Statista — communication-app usage, urbanization** | Statista (on MCMC/other base data) | Malaysia | WhatsApp/Telegram usage shares; urbanization | `10`, `50` | Secondary; underlying source is MCMC |

---

## 4. Market-sizing datasets

| Dataset | Publisher | Coverage / year | Key figures | Relied on by | Caveats |
|---|---|---|---|---|---|
| **Malaysia Telemedicine Market Size & Outlook 2025–2030** | Grand View Research (Horizon) | Malaysia, 2023–2030 | USD 1,848.6m (2023) → USD 6,515.4m (2030); 19.7% CAGR; MY = 1.6% of global | `10` | Vendor model; reconcile with Ken Research |
| **Malaysia Digital Health & Telemedicine Market** | Ken Research | Malaysia, 2019–2030 | ~USD 1.1B; RM1.2B government digital-health investment since 2020 | `10` | **Diverges from Grand View** — scope differs |
| **Malaysia E-Health & Virtual Clinics / Digital Therapeutics / Clinical Lab / Nutraceuticals markets** | Ken Research | Malaysia, 2019–2030 | Segment sizing & participant lists | `10` | Vendor estimates |
| **Singapore Telemedicine Market Size & Outlook** | Grand View Research | Singapore, 2023–2030 | SG telemedicine sizing | `10` | — |
| **GLP-1 Agonists Weight-Loss Drugs Market** | Grand View Research | Global | GLP-1 market size & CAGR | `10`, `50` | Global, not market-specific |
| **Malaysia Digital Transformation / Digital Health Market** | Mordor Intelligence | Malaysia | Alternative digital-health sizing | `10` | Third estimate for triangulation |
| **Malaysia Weight Loss & Obesity Management Market** | Data Bridge Market Research | Malaysia | Weight-loss market sizing | `10` | — |
| **Malaysia Nutritional Supplements Market 2024–2030** | Maximize Market Research | Malaysia | Supplements/longevity sizing | `10` | Cross-checked vs Ken Research |
| **Malaysia $2B+ Diagnostic Labs Market 2025–2030** | Research and Markets (via GlobeNewswire) | Malaysia | Diagnostic-labs sizing; independent labs ~40% | `10` | — |
| **SEA HealthTech & Life Sciences Funding Report 2024** | Tracxn | SE Asia, 2024 | US$123m (2024, −79% YoY; −90% vs 2022 peak); Singapore ~75% share | `10`, `20` | Funding-environment context |
| **Company/funding databases** | Crunchbase, PitchBook, CB Insights, Tracxn | Various | Round sizes, valuations, investor lists | `10`, `20` | Coverage varies; cross-check |

---

## 5. Company financials & filings

| Dataset | Publisher | Coverage / year | Key figures | Relied on by | Caveats |
|---|---|---|---|---|---|
| **IHH Healthcare Annual Report 2024** (+ 1Q26 analyst notes) | IHH Healthcare Berhad | FY2024–1Q26 | Group revenue RM24.4B (+16%), EBITDA RM5.4B; Malaysia revenue RM4.2B; MY beds 2,822→3,324; 1Q26 profit RM528m; FY2025 net profit RM2.10B | `10`, `20` | AR interactive + PDF; results via Kenanga/DBS/Bernama/The Star |
| **KPJ Healthcare Q4 FY2025 & full-year results** | KPJ Healthcare Berhad | FY2025 | Revenue & network performance | `10`, `20` | Via The Edge advertorial + KPJ site |
| **Sunway Healthcare Holdings IPO factsheet & prospectus** | Bursa Malaysia / Sunway | 2025 IPO | RM833.8m primary proceeds; capacity expansion; expansion plans | `20` | Bursa filing PDFs |
| **EC Healthcare annual/interim results** | EC Healthcare (HK-listed) | FY2021/22 & FY2024/25 | FY22 record revenue HK$3,122.3m (+40.7%); FY25 attributable loss HK$167.2m; HK$213.5m impairments | `20` | Via Nasdaq, MarketScreener, TipRanks |
| **Prenetics Q3/Q4 & FY2025 results** | Prenetics Global | FY2025 | IM8 ~US$120m ARR; revenue +480% YoY | `10`, `20` | Investor-relations releases |
| **Fullerton Healthcare perpetual-securities circular** | SGX (Fullerton) | 2017 | Corporate-health provider structure | `20` | Dated; structural reference |
| **Qualitas Health proposed IPO** | Bloomberg Law / The Edge / Caproasia | 2025 | ~US$942m IPO plan | `20` | Reported, pre-listing |

---

## 6. Price-benchmark datasets (GLP-1 and services)

| Dataset | Source | Coverage / year | Key figures | Relied on by | Caveats |
|---|---|---|---|---|---|
| **Malaysia GLP-1 street/clinic pricing** | Peak Protocol MY, Seimbang, CLEO Clinic, DoctorOnCall, Roczen | MY, 2025–26 | Ozempic/Wegovy/Mounjaro monthly costs (e.g. Mounjaro RM1,500–3,000/mo); registration MAL24026013AZ | `10`, `20`, `50` | Clinic-reported/advertised; move frequently; verify vs NPRA |
| **Singapore GLP-1 pricing across channels** | Regimen, Trimly, HMI Medical, clinic pages | SG, 2025–26 | Advertised SGD monthly ranges by channel | `10`, `20` | Advertised; POM ad limits apply |
| **Hong Kong GLP-1 pricing** | Wa Man Pharmacy, HKUMed Community Pharmacy, Panya, SCMP | HK, mid-2026 | Wegovy ~HK$2,700/mo retail; Mounjaro clinic programmes HK$6,000–11,500/mo | `10`, `20` | Advertised/reported; re-verify |
| **Service-price benchmarks** (teleconsult, screening, labs) | Provider pages across three markets | 2025–26 | Consult & package pricing for competitor comparison | `20`, `50` | Provider-listed; timing-sensitive |

---

*Compiled per [RESEARCH-STANDARDS.md](../RESEARCH-STANDARDS.md). Companion files: [bibliography.md](bibliography.md), [links.md](links.md), [regulations.md](regulations.md).*
