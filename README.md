# Phyllo Product Analyst Internship Assignment

## Orders API — Data Quality Review

### Overview

This repository contains my submission for the Phyllo Product Analyst Intern take-home assignment.

The assignment focuses on reviewing Orders API responses, identifying data quality issues, assessing their impact, and documenting potential bugs that could affect reporting and financial calculations.

### Tasks Completed

1. Data Quality Review
- Identified inconsistencies between API documentation and returned order data.
- Reviewed incorrect order totals and monetary formats.
- Identified pagination inconsistencies.
- Checked missing customer information and undocumented order statuses.
- Assessed the potential impact of each issue.

2. Revenue Analysis
- Calculated the sum of supplied order totals as $328.03.
- Identified limitations in treating this amount as definitive accounting revenue.
- Highlighted the need to clarify refunded order treatment and incorrect order totals.

3. Bug Report
- Documented a pagination bug in the /v1/orders API.
- Actual: has_more: false while another page exists.
- Expected: has_more: true when additional orders are available.
- Impact: Clients may miss orders, resulting in incomplete revenue reports.

### Key Findings

- Incorrect order total — Incorrect financial calculations.
- Monetary format inconsistency — Potential unit misinterpretation.
- Pagination inconsistency — Missing orders and incomplete datasets.
- Missing customer email — Incomplete customer data.
- Undocumented order status — Client handling issues.
- Incorrect missing-order response — Unexpected API behavior.

### Most Serious Issue

The pagination inconsistency was identified as the most concerning issue because it can silently cause clients to miss an entire page of orders, potentially resulting in incomplete datasets and inaccurate reporting.

### Skills Demonstrated

- Data Quality Analysis
- API Response Validation
- Business Impact Assessment
- Revenue Data Review
- Bug Reporting
- Analytical Problem Solving

### Author

Shweta Choori

Product Analyst Intern Candidate
