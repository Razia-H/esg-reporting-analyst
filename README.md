# AI ESG & Sustainability Reporting Analyst
### Agentic AI Portfolio Project | Claude (OpenRouter) + Google Sheets

## What It Does
Analyses supplier ESG questionnaires and sustainability reports using
a 4-agent parallel AI pipeline. Upload any sustainability document and
receive a complete ESG scorecard with domain scores, greenwashing risk
assessment, framework coverage mapping, and improvement priorities
in under 90 seconds.

## Stack
- AI Agents: Claude Haiku via OpenRouter API
- Frameworks: GRI Standards, TCFD, CSRD, UN SDGs, SBTi
- Dashboard: Google Sheets
- Input: Paste document text via browser UI

## The 4-Agent Pipeline

| Agent | Role | Output |
|-------|------|--------|
| Agent 1 | Environmental Analyst | Carbon, climate, energy, water, net zero scores |
| Agent 2 | Social Compliance Auditor | Labour, human rights, DEI, supply chain scores |
| Agent 3 | Governance Ethics Auditor | Board, anti-corruption, transparency scores |
| Agent 4 | ESG Score Orchestrator | Unified ESG score, rating, greenwashing risk |

## ESG Rating Scale

| Score | Rating | Approval Status |
|-------|--------|----------------|
| 85–100 | AAA | Approved |
| 70–84 | AA | Approved |
| 55–69 | A | Conditional Approval |
| 45–54 | BBB | Conditional Approval |
| 35–44 | BB | Requires Improvement |
| 20–34 | B | Requires Improvement |
| 0–19 | CCC | Not Approved |

## Scoring Formula
ESG Score = (Environmental × 0.35) + (Social × 0.30) + (Governance × 0.35)

## Why This Matters
The EU CSRD now mandates ESG disclosure for 50,000+ companies.
Every large enterprise needs to assess supplier ESG performance at
scale. Manual review takes 4-6 hours per supplier. This system does
it in 90 seconds with consistent framework-aligned scoring.

## How to Run the Demo
1. Get OpenRouter key at openrouter.ai/keys
2. Download app/esg-reporting-analyst.html
3. Open in Notepad → replace YOUR_OPENROUTER_KEY_HERE
4. Save → open in Chrome
5. Enter company details → click Load Demo Report
6. Click Run ESG Analysis → wait ~75 seconds

## Portfolio Defense Points
1. E/S/G weighted differently — reflects institutional ESG methodology
2. Greenwashing detection as distinct output — separates disclosure from credibility
3. Framework coverage mapping — shows regulatory alignment, not just summarisation
