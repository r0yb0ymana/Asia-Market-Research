# Verification — Methodology & Confidence Scheme

This folder is a second-pass verification of the repository's factual claims. It exists because the original research was built under a network constraint (see below) that capped most citations at search-snippet grade rather than primary-source grade.

Last updated: July 2026.

## The environment constraint (read this first)

The research and this verification pass were both produced in an execution environment whose **egress policy blocks direct fetching of most primary-source web pages** — government portals (DOSM, MOH, NPRA, SingStat, HK C&SD), company sites and price pages, stock-exchange filings (Bursa, SGX, HKEX), and paywalled market-research firms all return HTTP 403 to direct fetches. Full-page scraping (Firecrawl `scrape`) and the academic-database tools were not available/approved in this session either.

**What this means:** where a document cites a primary URL (e.g. `moh.gov.my`), the figure was almost always harvested from a **search-engine snippet** of that page, not read from the page itself. This verification pass operates under the same limit. It therefore raises confidence by **corroboration across multiple independent search results**, not by reading source documents.

This catches the failure modes that matter most — pure fabrications, mis-attributed entities, impossible or internally inconsistent figures, and stale/conflicting numbers — but it **cannot** confirm a figure to diligence grade. Any number this pass tags GREEN still merits a primary-source or phone confirmation before it is used in a financing, a regulatory filing, or a pricing commitment.

## Confidence tags

Each verified claim carries one tag:

| Tag | Meaning | Action before external use |
|---|---|---|
| 🟢 **GREEN** | Corroborated by ≥2 independent, credible search results that agree; internally consistent; no contradicting source found | Spot-check only |
| 🟡 **AMBER** | Single credible source, OR sources broadly agree but differ on specifics (range/date), OR figure is an explicitly labelled analyst estimate with sound logic | Confirm against primary source before relying on it |
| 🔴 **RED** | No corroborating source found, OR sources contradict, OR the figure appears to be fabricated / mis-attributed / internally impossible | Do not use until re-researched from primary source |
| ⚪ **UNVERIFIABLE** | Genuinely not checkable by desk research (e.g. private-company internal metrics, un-indexed app-store counts, transaction-only prices) | Requires primary/field research (mystery-shop, filing, interview) |

## What this pass covers

1. **[load-bearing-numbers-audit.md](load-bearing-numbers-audit.md)** — the ~50 figures the strategy actually rests on (market sizes, epidemiology, GLP-1 prices, key funding, regulatory dates), each corroborated and tagged.
2. **[price-verification.md](price-verification.md)** — competitor pricing across all three markets (GLP-1 programs, screening, consults), corroborated and tagged.
3. **[regulatory-verification.md](regulatory-verification.md)** — key regulatory instruments/dates/status per market, plus an explicit list of items that require a **human healthcare lawyer** and **medical director** to sign off (this pass verifies citations, it does not give legal or clinical advice).
4. **[consistency-reconciliation.md](consistency-reconciliation.md)** — internal cross-document reconciliation: the same fact stated differently across the 90 documents, with a discrepancy log and the fixes applied.

The driver-based financial model lives with the blueprint at [../70-welltech-blueprint/financial-model.md](../70-welltech-blueprint/financial-model.md).

## What this pass explicitly does NOT do

- It does not read primary-source documents (environment-blocked).
- It does not constitute legal or clinical advice or sign-off.
- It does not conduct field/primary research (mystery-shopping, transactions, interviews). Where that is the only way to confirm a figure, it is tagged ⚪ and listed for a human to execute.
