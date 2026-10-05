# Lending Club Credit Risk Analytics

## Business Context

**Stakeholder:** Head of Credit Policy at Lending Club
**Decision supported:** Which borrower segments should face tighter underwriting, and which are underpriced relative to their risk?
**Constraint:** Analysis must be defensible to regulators and investors — explainable, not overfit.

## Business Questions

1. Which loan grades have default rates that justify their interest rate?
2. How has default rate shifted year-over-year, and did 2015–2018 cohorts perform worse?
3. Which borrower segments (FICO, income, DTI, purpose) carry disproportionate default risk?
4. For a specific loan, what were the risk factors and how did similar loans perform?

## Data

- **Source:** Lending Club accepted loans (2007–2018)
- **Size:** ~2.26M rows, ~150 columns
- **Filter:** Only loans with final outcome (Fully Paid / Charged Off) — ~1.35M records
- **Critical:** Only origination-time features used. Post-origination columns
  (`total_pymnt`, `recoveries`, `last_pymnt_d`) are excluded to prevent leakage.
- **Download:** [add link here]

## Project Structure

- `sql/` — schema design and business-question queries
- `src/` — Python scripts for loading, cleaning, feature engineering
- `dashboards/` — Power BI dashboard files
- `docs/` — supporting documentation

## Status

- [ ] Week 1: Schema design + SQL queries
- [ ] Week 2: Power BI semantic model
- [ ] Week 3: Dashboard build + publish