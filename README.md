# Loan Default Dashboard

**Credit Risk & Debt-Burden Analysis | Excel, Power Query, Power Pivot & DAX**

## Project Overview

This project analyzes a 2025 loan portfolio to investigate whether borrower debt burden is associated with loan default and whether defaults occur immediately or develop gradually over time.

The analysis uses Excel, Power Query, Power Pivot, and DAX to clean and model loan and repayment data, calculate portfolio risk metrics, segment borrowers by debt-to-income (DTI) ratio, and translate the findings into credit-risk recommendations.

## Business Problem

The credit risk team wanted to determine whether loan size relative to borrower income was associated with repayment failure and whether high debt-burden borrowers were more likely to default.

The analysis also examined whether risk varied across:

- Debt-to-income (DTI) bands
- Credit-score groups
- Loan products
- Branches
- Loan officers
- First-payment behavior

## Objectives

- Establish portfolio baseline KPIs.
- Clean and transform the loan and repayment data.
- Build a structured analytical model using Power Pivot.
- Segment borrowers into Low, Moderate, High, and Severe DTI bands.
- Compare default rates across DTI bands and credit-score groups.
- Distinguish first-payment defaults from gradual defaults.
- Compare risk across products, branches, and loan officers.
- Translate the findings into credit-risk recommendations.

## Tools & Technologies

- **Microsoft Excel**
- **Power Query** — data cleaning and transformation
- **Power Pivot** — data modeling and analysis
- **DAX** — calculated measures and risk metrics
- **PivotTables / PivotCharts** — analysis and dashboard visualization

## Data Scope

| Metric | Value |
|---|---:|
| Analysis period | January–December 2025 |
| Loans analyzed | ~20,000 |
| Total portfolio value | £548.5M |
| Overall default rate | 12.23% |
| Average DTI | 24.04% |
| Portfolio value at risk | £87.5M |
| Repayment shortfall | £12.48M |
| Collection rate | 90.29% |

## Analytical Approach

### 1. Data Preparation

Raw loan and repayment extracts were cleaned and transformed using Power Query before being incorporated into the analytical model.

### 2. Data Modeling

A Power Pivot model was used to support portfolio-level and segmented analysis across loan, borrower, repayment, product, branch, and officer dimensions.

### 3. Debt-Burden Analysis

Debt-to-income ratios were grouped into four risk bands:

- Low
- Moderate
- High
- Severe

Default rates and portfolio exposure were compared across the bands.

### 4. First-Payment Default Analysis

The analysis examined whether borrowers who missed their first payment subsequently defaulted or returned to normal repayment.

### 5. Segment Analysis

Risk patterns were evaluated across credit-score groups, loan products, branches, and loan officers.

## Key Findings

### Debt burden was the strongest observed risk signal

Observed default rates increased from **5.48% for Low DTI borrowers to 43.50% for Severe DTI borrowers**, an approximately eightfold increase.

### A missed first payment was a weak standalone default signal

**63% of loans that missed their first payment subsequently repaid without defaulting**, indicating that a single missed payment should not automatically be treated as evidence of high default risk.

### Credit score provided less differentiation at severe debt burden

At Severe DTI, Fair, Poor, and Unknown credit-score groups showed default rates of approximately **43–45%**, suggesting that high debt burden reduced the ability of credit score alone to distinguish observed risk.

### Defaults were predominantly gradual

Approximately **75–80% of defaults occurred gradually** across DTI bands. Higher DTI increased immediate-failure risk only modestly.

### Some segments warranted further review

SME loans and the Manchester and Newcastle branches showed higher default rates than the broader portfolio and were identified for additional review.

### Apparent loan-officer differences required caution

Although officer-level default rates appeared different when sorted, statistical analysis found that only **3 of 40 officers** had patterns distinguishable from the portfolio average. The remaining variation was not treated as evidence of individual performance differences.

## Recommendations

1. Tighten approval criteria above approximately **35% DTI**, where default risk and money at risk become more concentrated.
2. Give **debt-to-income ratio greater weight alongside credit score**, particularly for loans with high debt burden.
3. Conduct additional review of **SME applications and the Manchester/Newcastle branches**.
4. Use a missed first payment as a trigger for **early borrower contact**, rather than automatically classifying the loan as high risk.
5. Avoid ranking individual loan officers using the observed default rates alone because most apparent differences were not statistically supported.

## Dashboard Preview

![Loan Default Dashboard](screenshots/loan-default-dashboard.png)

## Repository Contents

| File | Description |
|---|---|
| `dashboard/Loan Default Dashboard.xlsx` | Final Excel dashboard and analytical workbook |
| `screenshots/loan-default-dashboard.png` | Final dashboard preview |
| `documentation/Project Brief.pdf` | Project business case and analytical requirements |
| `documentation/Analysis and Recommendations.pdf` | Final analytical summary and recommendations |

## Data Note

The project uses a provided training dataset covering a 2025 loan portfolio of approximately 20,000 loans. The analytical workbook contains the data and transformation/modeling work used for the dashboard.

This project was completed within a structured analytics training program using a provided business case and dataset.

## Project Context

The project was designed to simulate a Junior Data Analyst assignment within a credit-risk environment, requiring data preparation, analytical modeling, dashboard development, and business recommendations.
