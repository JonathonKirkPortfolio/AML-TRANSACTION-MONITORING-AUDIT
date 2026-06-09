# AML Transaction Monitoring Audit: Pass-Through & Structuring Identification

## Executive Summary
A forensic review of May transaction data was conducted to identify anomalous behavior. The analysis revealed severe red flags indicative of cash structuring (smurfing) to evade £10k reporting thresholds, and immediate pass-through activity involving high-risk offshore jurisdictions (Panama to the UAE). 

## Technical Methodology
To isolate the risk within the transaction noise, I utilized a "Core 3" data analysis toolkit:
Risk Mapping (`XLOOKUP`): Engineered an automated geographical screener to cross-reference counterparty jurisdictions against FATF High-Risk indices.
Typology Identification (Conditional Formatting): Applied algorithmic highlighting to isolate cash deposits engineered specifically between £8,000 and £9,999.
Volumetric Aggregation (Pivot Tables): Mapped volumetric flow to identify immediate U-turn transactions and filter out low-level domestic spending.

## Key Investigative Findings

1. Cash Structuring (Smurfing)
Between May 4 and May 9, the subject account received three branch cash deposits (£8,900, £9,500, and £9,800) totaling £28,200. These amounts are deliberately structured just below the £10,000 reporting threshold, presenting a clear indicator of evasion.

<img width="192" height="401" alt="smurfing" src="https://github.com/user-attachments/assets/870d88e8-6243-4a24-b8ec-6b163d99e36c" />



2. High-Risk Pass-Through Activity
The account exhibits a classic "U-turn" pass-through pattern that does not align with its routine domestic expenditures (e.g., Tesco, TfL). 
* On May 14, **£125,000** was received from Apex Holdings LLC in Panama.
* The very next day (May 15), **£124,000** was wired out to Global Chemical Corp in the UAE.

<img width="683" height="340" alt="pivot_table" src="https://github.com/user-attachments/assets/73339027-2e3f-4f92-9e2a-2e96d007cde1" />

<img width="165" height="412" alt="risk_flags" src="https://github.com/user-attachments/assets/34691dba-666c-4d48-9440-479278dd9406" />


## Conclusion & Recommendation
The rapid movement of massive funds from a secrecy jurisdiction (Panama) to a high-risk manufacturing hub (UAE) using a UK account holds no discernible economic purpose. Combined with the deliberate structuring of domestic cash deposits, these typologies strongly mirror illicit supply chain financing. 

Recommendation: Restrict account activity immediately and file a Suspicious Activity Report (SAR) detailing the pass-through network and threshold evasion.
