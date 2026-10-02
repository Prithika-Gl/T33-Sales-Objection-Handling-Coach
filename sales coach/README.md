# T33 Sales Objection-Handling Coach

## Project Overview

The T33 Sales Objection-Handling Coach is a source-grounded AI sales coaching system designed to help salespeople practise handling realistic customer objections for CloudLedger, an accounting and GST software scenario for SMEs.

The coach simulates buyer objections, evaluates salesperson responses, provides transcript-grounded feedback, and applies explicit controls against unsupported product claims.

---

## Business Scenario

**Company:** CloudLedger  
**Product:** Accounting and GST software for SMEs  
**Price:** ₹1,499 per user per month  
**Buyer:** Owner of a 40-employee distribution business in Nashik  
**Current Process:** Excel + local accountant  
**Competition:** Two popular accounting tools approximately 15–25% cheaper  
**Sales Goal:** Book a paid 30-day pilot

---

## Project Objective

The objective was to develop an AI coach that can:

- Simulate realistic buyer objections
- Keep the conversation focused on the active objection
- Ask useful discovery questions
- Avoid unsupported product claims
- Provide transcript-grounded coaching
- Evaluate salesperson performance
- Suggest practical improvements
- Handle grounding tests without inventing facts

---

## Objection Areas Tested

The project tested five major objection areas:

1. Price
2. Need
3. Competition
4. Trust
5. Risk

The source Objection Library contains 20 objections across 11 categories.

---

## Development Process

### Stage 1 — Source Validation
Validated the original project workbook and identified the source-of-truth materials.

### Stage 2 — Grounding
Tested retrieval of scenario facts and objection-library information and tested the system against unsupported claims.

### Stage 3 — V1 Baseline
Created and tested the first sales-coaching prompt.

### Stage 4 — V2 Coach
Introduced stronger grounding controls, objection locking, response-aware buyer behaviour and transcript-based scoring.

### Stage 5 — Scoring Audit
Audited score calculations, evidence attribution, grounding and pilot handling.

### Stage 6–7 — Final Coach
Introduced the final evidence-attribution rule and conducted the final demonstration and audit.

### Stage 8 — Evidence Packaging
Prepared the master evidence workbook and repository package.

### Stage 9 — Final Report
Created the final project report.

---

## V2 Results

| Objection | Score |
|---|---:|
| Price | 20/25 |
| Need | 18/25 |
| Competition | 14/25 |
| Trust | 18/25 |
| Risk | 20/25 |
| **Total** | **90/125** |

**Average:** 18/25  
**Percentage:** 72%

### V2 Dimension Totals

| Dimension | Score |
|---|---:|
| Objection Handling | 18/25 |
| Discovery | 20/25 |
| Value/Evidence | 14/25 |
| Accuracy/Grounding | 22/25 |
| Next-Step/Pilot | 16/25 |

---

## Final Demonstration

The final demonstration combined:

- Need objection
- Competition objection
- Price objection
- Risk objection
- Trust objection
- Paid pilot discussion
- Grounding test

The grounding test asked whether CloudLedger provides a **3-year warranty and a 100% money-back guarantee**.

The coach did not confirm these as established facts and instead required verification.

---

## Final Score

| Dimension | Score |
|---|---:|
| Objection Handling | 4/5 |
| Discovery | 4/5 |
| Value/Evidence | 3/5 |
| Accuracy/Grounding | 5/5 |
| Next-Step/Pilot | 4/5 |
| **Total** | **20/25** |

**Final Score: 80%**

---

## Responsible AI Controls

The project incorporates the following controls:

- Source-grounded responses
- Explicit unsupported-claim handling
- No invented customer or financial information
- No unsupported product guarantees
- Transcript-based scoring
- Direct evidence attribution
- "Evidence not sufficient to verify this finding" when evidence is inadequate
- Separation of practice suggestions from established product facts

---

## Key Business Insights

- Discovery should precede value positioning.
- Competitive comparisons should be based on buyer requirements rather than unsupported superiority claims.
- Trust and risk objections can be explored through explicit evaluation criteria.
- A paid pilot provides a concrete next-step structure within the scenario.
- The coach should not invent ROI, customer references or product capabilities to strengthen a sales response.

---

## Limitations

- Statistical repeatability was not tested.
- An evidence-attribution issue identified during V2 Competition evaluation was addressed through the final evidence-attribution rule.
- The project uses the supplied CloudLedger scenario and source materials.
- Coach grounding depends on the completeness and accuracy of those source materials.

---

## Repository Structure

```text
T33-Sales-Objection-Handling-Coach/
│
├── 01_Source_Materials/
│   ├── T33_Source_Workbook_ORIGINAL.xlsx
│   ├── T33_Source_Materials.pdf
│   └── T33_Source_Validation.txt
│
├── 02_Prompts/
│   ├── T33_V1_System_Prompt.txt
│   ├── T33_V2_System_Prompt.txt
│   └── T33_FINAL_System_Prompt.txt
│
├── 03_V1_Testing/
│
├── 04_V2_Testing/
│   └── T33_Consolidated_V2_Coaching_Report.txt
│
├── 05_Scoring/
│   └── T33_V2_Scoring_Audit.txt
│
├── 06_Final_Testing/
│   ├── T33_Final_Demonstration_Record.txt
│   └── T33_Final_Evidence_Audit.txt
│
├── 07_Screenshots/
│
├── 09_Transcripts/
│   └── FINAL_Demo_Transcript.txt
│
├── 10_Final_Documents/
│   └── T33_Final_Report.docx
│
├── T33_Sales_Objection_Handling_Coach_FINAL_MASTER_WITH_AI_USE_LOG.xlsx
│
└── README.md