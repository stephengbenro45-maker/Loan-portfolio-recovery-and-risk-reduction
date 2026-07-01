# Loan-portfolio-recovery-and-risk-reduction strategy
[loan portfolio strategy file .pdf](https://github.com/user-attachments/files/29572263/loan.portfolio.strategy.file.pdf)
Case Study

## Project Overview
This project provides a comprehensive, data-driven credit risk analysis and portfolio recovery framework for a digital lending platform experiencing financial stress. Out of 500 loans collected by customers, 130 loans went overdue, resulting in an alarming *26% delinquency rate* and freezing *₦14.98M* in unrecovered capital. 

The goal of this analysis was to transform raw, unstructured operational data into a strategic decision-making engine. By handling the complete data transformation lifecycle inside Power BI, this dashboard diagnoses exactly why borrowers are paying late, segments future default risks, and executes a structured, operational recovery plan to salvage trapped cash flow.


## Tech Stack & Skills Demonstrated
* *Data Transformation & Cleaning:* Power Query (M formula language)
* *Data Modeling & Analytics:* Power BI Desktop, DAX (Data Analysis Expressions)
* *Core Frameworks:* Descriptive, Diagnostic, Predictive, and Prescriptive Analytics
* *Domain Expertise:* Fintech, Credit Risk Triage, Collections Engineering, Portfolio Management



##  Data Transformation & Cleaning (Power Query)
Before building any visuals or metrics, the raw datasets required intensive data cleaning and restructuring inside *Power Query* to ensure data integrity:
* *Text Normalization:* Fixed structural inconsistencies where regional fields (e.g., Lagos, Abuja, Port Harcourt) were randomly entered in messy uppercase text, bringing everything into a standardized, clean formatting.
* *Null Value Handling:* Isolated and treated null values across critical transactional columns, replacing missing records with logical fallbacks to prevent calculation errors in downstream DAX measures.
* *Data Type Enforcement:* Handled structural alignment across tables to ensure dates, user KYC tiers, and loan amounts perfectly corresponded for analytical filtering.
##  The Analytics Lifecycle Breakdown

### 1. Business Problem & Diagnostics (What Happened & Why)
* *The Portfolio Bottleneck:* A 26% delinquency rate means more than 1 out of every 4 borrowers has failed to repay on time, locking up ₦14.98M of the company's total available liquidity.
* *The Tier 1 Pricing Trap:* Drilling down into KYC tiers revealed that legacy interest rules were crushing unverified Tier 1 users. Tier 1 recorded a high delinquency rate heavily concentrated in high-interest (25 late loans) and medium-interest (15 late loans) brackets, compared to *just 2 late loans* on low-interest terms. Our own pricing structure was forcing early-stage users to default.
* *The Tier 2 & Tier 3 Leak:* Verified, high-limit customers continued to record high delinquency rates (26.44% and 24.68% respectively). This portfolio-wide challenge indicated that these tiers were over-reliant on the platform and intentionally exploiting soft automated reminders to delay payments.

### 2. Predictive Risk Analysis (What Happens If We Do Nothing?)
* *The Write-Off Horizon:* The risk-aging model isolated that *20% of currently delinquent customers* are at immediate risk of churning (moving into total default and becoming permanent bad debt).
* *Localized Hyper-Risk (The Abuja Example):* 
  * General default risk across Abuja: *13.04%*
  * When filtered for only Tier 1 users: *42.86%*
  * When filtered for Abuja Tier 1 users specifically on high-interest loans: *50.00%*
* This predictive modeling proves that pairing unverified users with high interest rates creates a guaranteed 50/50 capital loss scenario in high-volume regions.

### 3. Prescriptive Strategy: The Dual-Truth Recovery Plan (The Solution)
The operational recovery framework targets two priorities: recovering the *₦10.51M in overdue principal* currently sitting across 93 mature overdue accounts, and reforming future pricing rules.

* *Truth 1: Future Lending Reforms (Preventative)*
  * *Tier 1:* Permanently block Tier 1 profiles from accessing high or medium interest rates. Restrict them strictly to low-interest options to ensure repayment viability.
  * *Tiers 2 & 3:* Enforce zero interest reductions. Since we hold verified KYC information, their path relies entirely on strict operational collection efforts, not financial concessions.

* *Truth 2: Tiered Recovery Workflow (Remedial for the ₦10.51M)*
  * *Recently Overdue:* Deploy automated tracking sequences across SMS, WhatsApp, and phone calls to enforce early-stage discipline.
  * *Moderately Overdue:* Implement immediate digital profile restrictions and freeze borrowing privileges while routing accounts to internal human collection squads.
  * *Long-Overdue Tier 1 (61+ Days):* Execute a capital preservation strategy. Issue a limited-time "Principal-Only Settlement Offer" to waive accumulated interest and recover the core underlying cash.
  * *Long-Overdue Tiers 2 & 3 (61+ Days):* Route profiles directly to External Recovery Agents and trigger permanent blacklisting across Nigerian Credit Bureaus to freeze their access to the banking ecosystem.

---

##  Expected Business Impact
* *₦10.51M* in core overdue principal recovered from chronic defaults.
* Drastic reduction in future delinquency velocity by optimizing Tier 1 pricing.
* Unfrozen capital reserves to improve corporate liquidity and cash flow.
* A sustainable, data-validated lending framework built to support long-term portfolio growth.
