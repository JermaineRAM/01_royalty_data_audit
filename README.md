# 🎵 Royalty Data Audit — Usage, Payments, and Reconciliation Risk
## Project Overview

This project simulates an early-stage music royalty audit, analysing reported usage data and payment records to identify reconciliation gaps, data quality issues, and areas of elevated risk.

The analysis mirrors the initial phase of a real-world royalty audit, where the goal is not detailed financial modelling, but rather to establish confidence in the data, quantify potential exposure, and prioritise areas for further investigation.

Note: The dataset used in this project is fully simulated to reflect real-world music royalty reporting structures and includes intentional anomalies designed to surface common audit issues.

## Key Audit Questions

The analysis was guided by three core audit questions:

 1. Completeness: What proportion of reported usage has no corresponding payment record?

 2. Data integrity: Are there missing identifiers, duplicate records, or invalid stream values?

 3. Risk concentration: Are reconciliation issues concentrated by platform, territory, or reporting period?

## Dataset

The simulated dataset reflects common royalty reporting inputs and includes:

 - Usage reports by platform, territory, and reporting period

 - Royalty rate tables

 - Payment records linked to usage reports

The data structure mirrors that used by record labels, distributors, and collection societies, allowing for realistic audit-style analysis without using proprietary information.

## Methodology

The audit follows a structured, risk-focused workflow:

 1. Data validation and integrity checks

     - Missing identifiers

     - Duplicate usage records

     - Invalid or impossible stream values

 2. Reconciliation analysis

     - Matching reported usage to payment records

     - Quantifying unpaid or unmatched usage

 3. Risk segmentation

     - Breaking unpaid usage down by:

         - Platform

         - Territory

         - Reporting period

 4. Timing analysis

     - Assessing whether unpaid usage can be explained by normal payment delays

 5. Focused risk investigation

     - Drilling into high-risk platform–territory combinations over time

Visualisations are used selectively to support interpretation rather than to present final financial conclusions.

## Key Findings
### 1️⃣ Meaningful Reconciliation Gap Identified

Approximately 10% of reported usage records have no matching payment, indicating a non-trivial reconciliation gap that would warrant follow-up in a real audit context.

### 2️⃣ Risk Is Not Evenly Distributed

Unpaid usage is not evenly spread across the dataset. The highest concentration of unpaid usage is observed on Apple Music, particularly within the US territory.

Given the typically material revenue contribution of US usage, this represents a higher-risk segment from an audit prioritisation perspective.

### 3️⃣ Payment Timing Does Not Fully Explain the Gap

To assess whether unpaid usage was simply the result of normal payment cycles, average payment delays were analysed across platforms.

Payment delays were found to be broadly consistent across all DSPs, averaging approximately 75 days. Apple Music did not exhibit longer delays than other platforms, suggesting that its higher unpaid rate is unlikely to be explained by slower payment timing alone.

### 4️⃣ Unpaid Usage Is Episodic, Not Structural

A focused analysis of Apple Music US usage over time shows that unpaid rates are spiky and concentrated in specific reporting months, rather than persistently elevated.

This pattern is more consistent with:

 - Reporting ingestion issues

 - Delayed reprocessing

 - Period-specific reconciliation failures

…rather than systematic underpayment.

## Interpretation

Taken together, the findings suggest that unpaid royalty usage is driven less by uniform timing delays and more by episodic reporting or reconciliation breakdowns in specific high-volume segments.

From an audit perspective, this indicates that Apple Music US usage during specific reporting periods should be prioritised for targeted investigation, rather than applying broad, platform-wide assumptions.

## Limitations

 - The dataset is simulated and does not represent actual royalty payments

 - No contractual terms or escalations are modelled

 - Findings are intended for risk identification, not final financial adjustment

## Skills Demonstrated

 - Audit-style exploratory data analysis

 - Data quality and integrity validation

 - Reconciliation logic and gap analysis

 - Risk segmentation by platform, territory, and time

 - Clear communication of audit findings and priorities

## Conclusion

This project demonstrates how structured exploratory analysis can be used to identify reconciliation risk early in the royalty reporting lifecycle, before detailed financial modelling or contractual review.

By focusing on data completeness, integrity, and risk concentration, the analysis mirrors real-world audit workflows used by music industry stakeholders to efficiently allocate investigative effort and reduce revenue leakage.