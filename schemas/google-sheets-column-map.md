# Google Sheets — ESG Supplier Dashboard Schema

## Tab Name: ESG_SUPPLIER_DASHBOARD

| Col | Header | Type | Filled By |
|-----|--------|------|-----------|
| A | Run_ID | Text | System |
| B | Timestamp | DateTime | System |
| C | Company_Name | Text | System |
| D | Report_Year | Text | System |
| E | Industry_Sector | Text | System |
| F | ESG_Score | Number 0-100 | System |
| G | ESG_Rating | Dropdown: AAA AA A BBB BB B CCC | System |
| H | Approval_Status | Dropdown | System |
| I | Environmental_Score | Number | System |
| J | Social_Score | Number | System |
| K | Governance_Score | Number | System |
| L | Greenwashing_Risk | Dropdown: HIGH MEDIUM LOW | System |
| M | Critical_Findings | Text | System |
| N | Framework_Coverage | Text | System |
| O | Executive_Summary | Long Text | System |
| P | Reviewed_By | Text | Human |
| Q | Review_Date | Date | Human |
| R | Final_Decision | Dropdown: APPROVED REJECTED PENDING | Human |

## Conditional Formatting Column F
- 85–100: Dark Green #2E7D32
- 70–84: Green #C8E6C9
- 55–69: Yellow #FFF9C4
- 35–54: Orange #FFE0B2
- 0–34: Red #FFCDD2

## Human-in-the-Loop Rules
- APPROVED: no action needed
- CONDITIONAL_APPROVAL: improvement plan required within 90 days
- REQUIRES_IMPROVEMENT: re-assess in 6 months
- NOT_APPROVED: do not onboard until remediation complete
