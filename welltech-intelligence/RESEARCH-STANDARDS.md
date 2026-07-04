# Welltech Intelligence — Research & Writing Standards

This document defines the mandatory standards for every document in this repository. All contributors (human or AI) must follow it.

## Mission

Build an institutional-grade market intelligence repository for Welltech Health covering digital healthcare in Malaysia, Singapore, and Hong Kong — with depth comparable to McKinsey, Bain, BCG, a16z, Sequoia, CB Insights, Gartner, and RedMonk research. The repository serves founders, investors, product managers, clinicians, marketers, and AI agents.

## Focus domains

Telehealth · digital private healthcare · medical weight loss · longevity medicine · preventive medicine · functional medicine · GLP-1 treatment ecosystem · concierge healthcare · AI-enabled healthcare · WhatsApp healthcare workflows.

## Writing standards

1. **Write for executives.** No filler, no marketing language, no AI clichés ("in today's fast-paced world", "delve", "landscape is evolving"). Every sentence must carry information.
2. **Evidence first.** Every factual statement carries a citation. Where data is uncertain, contested, or estimated, say so explicitly and show the range across sources.
3. **Structure.** Use headings, tables, comparison matrices, SWOT, Porter's Five Forces, value-chain analysis, and customer-journey maps where they genuinely add analytical value.
4. **Standalone documents.** Each file must be readable on its own, with internal links (relative Markdown links) to related documents.
5. **Numbers.** State currency (MYR/SGD/HKD/USD), year, and source for every figure. Reconcile conflicting estimates rather than picking one silently.
6. **Analysis over description.** End major sections with "Implications for Welltech" where relevant.

## Citation format

- Inline: numbered footnote-style references, e.g. `...market reached USD 1.85B in 2023.[^1]`
- At the bottom of each document, a `## References` section listing each source:
  `[^1]: Grand View Research, "Malaysia Telemedicine Market Size & Outlook, 2025–2030", https://www.grandviewresearch.com/horizon/outlook/telemedicine-market/malaysia (accessed July 2026).`
- Prefer primary sources: government (MOH Malaysia, MOH Singapore, HK Health Bureau, Bank Negara, DOSM, Singstat, HK C&SD), WHO, OECD, World Bank, medical journals, company filings, hospital annual reports, investor reports. Use market-research firms and press as secondary corroboration.
- Never fabricate a citation. If a claim cannot be sourced, label it clearly as `*(analyst estimate)*` or `*(inference)*` with reasoning.

## Document conventions

- Start each file with an H1 title, a one-paragraph abstract, and a "Last updated: July 2026" line.
- Use tables for comparable data; use fenced Mermaid diagrams for journeys/architectures where useful.
- File naming and folder structure are fixed (see README.md). If a document grows beyond ~1,500 lines, split it logically and cross-link.

## Repository map

See [README.md](README.md) for the full structure and reading order.
