# 01_royalty_data_audit
Simulated royalty audit analysing music usage, payments, and payout discrepancies across platforms and territories using Python.

## Audit Questions
 * Completeness: What % of reported usage has no matching payment?
 * Integrity: Are there missing IDs, duplicates, or impossible stream values?
 * Risk hotspots: Are issues concentrated by platform or territory?

## Findings (Initial)

- Approximately **10% of reported usage** has **no matching payment record**, indicating a non-trivial reconciliation gap.
- Unpaid usage is **most concentrated on Apple Music**, suggesting higher reconciliation or reporting risk on this platform.
- The **US territory** shows the highest unpaid rate, which is material given its typically large revenue contribution.

These findings suggest that unpaid usage is not evenly distributed and that **Apple Music US usage should be prioritised** for further investigation into payment delays, reversals, or contractual timing differences.