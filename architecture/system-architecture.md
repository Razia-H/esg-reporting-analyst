# ESG Reporting Analyst — System Architecture

## Overview
4-agent parallel AI pipeline that analyses supplier ESG documents
against GRI, TCFD, CSRD, UN SDGs and SBTi frameworks.

## End-to-End Flow

INGESTION → CONTEXT PACKAGER → PARALLEL AGENTS → ORCHESTRATOR → SHEETS

## Pipeline Steps

1. User uploads supplier ESG document via browser UI
2. Context packager extracts company name, sector, year, document text
3. Three specialist agents run simultaneously:
   - Agent 1: Environmental — carbon, climate, energy, water, net zero
   - Agent 2: Social — labour, human rights, DEI, supply chain
   - Agent 3: Governance — board, anti-corruption, transparency
4. Agent 4 ESG Orchestrator synthesises all three outputs
5. Calculates final ESG score using weighted formula
6. Assigns ESG rating AAA to CCC and approval status
7. Flags greenwashing risks as separate output
8. Results written to Google Sheets dashboard

## Scoring Formula

ESG Score = (Environmental × 0.35) + (Social × 0.30) + (Governance × 0.35)

## Why Environmental and Governance Weighted Higher Than Social
Environmental (35%) and Governance (35%) carry equal weight because
climate liability and board accountability show stronger correlation
with financial risk than social metrics alone — aligned with
institutional ESG rating methodology used by MSCI and Sustainalytics.

## ESG Rating Scale

| Score   | Rating | Approval Status         |
|---------|--------|------------------------|
| 85–100  | AAA    | Approved               |
| 70–84   | AA     | Approved               |
| 55–69   | A      | Conditional Approval   |
| 45–54   | BBB    | Conditional Approval   |
| 35–44   | BB     | Requires Improvement   |
| 20–34   | B      | Requires Improvement   |
| 0–19    | CCC    | Not Approved           |
