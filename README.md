# 01_royalty_data_audit

Simulated royalty audit analysing music usage, payments, and reconciliation risk across platforms and territories using Python.

This project mirrors an early-stage royalty audit workflow, focusing on data quality, payment completeness, and risk identification prior to detailed financial modelling.

> **Note:** The dataset used in this project is simulated to reflect real-world music royalty reporting structures and includes intentional anomalies for audit analysis.

---

## Audit Questions

- **Completeness:** What percentage of reported usage has no matching payment record?
- **Data integrity:** Are there missing identifiers, duplicates, or invalid stream values?
- **Risk concentration:** Are reconciliation issues concentrated by platform, territory, or time period?

---

## Findings and Interpretation

An initial audit of reported usage data shows that approximately **10% of usage records have no matching payment**, indicating a meaningful reconciliation gap that warrants further investigation.

When unpaid usage was analysed by platform and territory, **Apple Music** and the **US territory** exhibited the highest unpaid rates. Given the material revenue contribution typically associated with US usage, this represents a higher-risk segment from an audit perspective.

To determine whether this elevated unpaid rate was driven by payment timing, average payment delays were analysed across platforms. Payment delays were found to be **broadly consistent across all DSPs** (approximately 75 days on average). Apple Music did not exhibit longer delays than other platforms, suggesting that its higher unpaid rate is **unlikely to be explained by slower payment timing alone**.

A focused analysis of **Apple Music US usage over time**, supported by a visual trend analysis, shows that unpaid rates are **spiky and concentrated in specific reporting months rather than consistently elevated**. This pattern points toward **episodic reporting or reconciliation issues**, such as ingestion failures or delayed reprocessing, rather than structural underpayment.

Taken together, these findings indicate that **Apple Music US usage represents a higher-risk segment for unresolved royalty payments in specific periods and should be prioritised for targeted investigation in a real-world audit context**.
