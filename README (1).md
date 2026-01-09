# Massachusetts Healthcare Cost Analysis

**Massachusetts has the highest healthcare costs in the nation.** This repository documents the crisis using official government data.

## ⚠️ Data Notes

| Figure | Year | Data Type | Source |
|--------|------|-----------|--------|
| State Premiums | 2025 | **Estimated** | 2024 KFF + 10% growth rate |
| US Average Premium | 2025 | Actual | KFF EHBS 2025 ($26,993) |
| Per Capita Spending | 2020 | Actual | CMS State Health Expenditure |
| THCE Growth | 2013-2023 | Actual | CHIA 2025 Annual Report |
| Affordability | 2023 | Actual | CHIA 2025 Annual Report |
| 2026 Rate Increases | 2026 | Actual | MA Division of Insurance |

**2025 State Premium Methodology:** KFF does not publish state-level data in the 2025 survey due to sample size limitations. State estimates were derived by applying the KFF-reported 10% national growth rate (from $24,540 to $26,993) to 2024 state figures.

---

## Key Findings

| Metric | Massachusetts | US Average | Gap |
|--------|--------------|------------|-----|
| Family Premium (2025 Est.) | **$30,966** | $26,993 | **+14.7%** |
| Per Capita Spending (2020) | **$13,319** | $10,191 | **+30.7%** |
| 2023 Cost Growth | **8.6%** | 3.6% benchmark | **+139% over** |
| 2026 Rate Increases | **7-14%** | ~3% inflation | **3-4x inflation** |

---

## Visualizations

### 1. State Premium Comparison (2025 Estimated)
![State Premium Comparison](01_state_premium_comparison_2025.png)

### 2. Premium Trends (2019-2025)
![Premium Trends](02_premium_trends_2025.png)

### 3. Per Capita Spending (2020)
![Per Capita Spending](03_per_capita_spending_2020.png)

### 4. Cost Growth vs Benchmark
![THCE vs Benchmark](04_thce_vs_benchmark.png)

### 5. Affordability by Race
![Affordability](05_affordability_by_race.png)

### 6. Cost Breakdown
![Cost Breakdown](06_cost_breakdown.png)

### 7. 2026 Rate Increases
![2026 Rates](07_2026_rate_increases.png)

### 8. Provider Costs
![Provider Costs](08_provider_costs.png)

### 9. Root Causes Analysis
![Root Causes](09_root_causes_analysis.png)

### 10. PBM (Pharmacy Benefit Manager) Analysis
![PBM Analysis](10_pbm_analysis.png)

### 11. PBM Cost Impact Summary
![PBM Cost Impact](11_pbm_cost_impact.png)

---

## Why Are Costs So High? Root Causes

### 1. Hospital Market Concentration (39% of Gap)
- MA hospitals charge **31% more** than US average
- Mass General Brigham, Beth Israel Lahey dominate market
- Provider consolidation reduces price competition

### 2. Post-Acute Care Costs (19% of Gap)
- Home health: **DOUBLE** national average (+100%)
- Nursing homes: +39% above US average

### 3. Pharmacy & PBM Issues (25% of 2023 Growth)
- Drug costs grew **11.6%** in 2023 (fastest category)
- **$4 billion** in rebates negotiated - but PBMs retain significant portion
- 3 PBMs control 80% of US prescriptions (CVS Caremark, Express Scripts, OptumRx)

**FTC Findings (Jan 2025):**
- Big 3 PBMs generated **$7.3 billion** in excess revenue from specialty generic markups (2017-2022)
- Additional **$1.4 billion** from spread pricing on same drugs
- One drug (tadalafil) marked up **7,736%** ($27 → $2,106)
- 72% of high-markup prescriptions steered to PBM-owned pharmacies
- FTC filed complaint against top PBMs for "artificially inflating insulin prices"

**State Medicaid Audits Found:**
- Ohio: $224.8M pocketed by PBMs in ONE year
- Kentucky: $123.5M annually (triggered AG investigation)
- West Virginia saved $54M first year after becoming its own PBM

### 4. State Policy (23% of 2023 Growth)
- MassHealth added $1.5B in hospital supplemental payments
- Cost benchmark exceeded repeatedly with no penalty
- New PBM law (Jan 2025) requires licensing by 2026, but doesn't ban spread pricing

**Bottom Line: It's PRICE, not utilization.** MA residents don't use more care — providers and middlemen charge more.

---

## Data Sources

| Source | Data | URL |
|--------|------|-----|
| **KFF EHBS 2025** | US national premium ($26,993) | [kff.org/ehbs](https://www.kff.org/health-costs/report/employer-health-benefits-survey/) |
| **KFF EHBS 2024** | State-level premiums (base for estimates) | [kff.org/ehbs](https://www.kff.org/health-costs/report/employer-health-benefits-survey/) |
| **CMS** | Per capita spending by state | [cms.gov](https://www.cms.gov/data-research/statistics-trends-and-reports/national-health-expenditure-data/state-residence) |
| **CHIA 2025** | MA cost growth, affordability, TME | [chiamass.gov](https://www.chiamass.gov/annual-report/) |
| **MA DOI** | 2026 rate filings | [mass.gov](https://www.mass.gov/info-details/2026-health-insurance-rates) |
| **FTC** | PBM Reports (July 2024, Jan 2025) | [ftc.gov](https://www.ftc.gov/news-events/news/press-releases/2025/01/ftc-releases-second-interim-staff-report-prescription-drug-middlemen) |
| **State Audits** | OH, KY, MD, LA, MI, VA Medicaid audits | Various state sources |

---

## Data Files

- `state_premium_2025_estimated.csv` - 2025 state premiums (estimated)
- `state_premium_2024_actual.csv` - 2024 state premiums (actual KFF)
- `premium_trends_2019_2025.csv` - Historical premium trends
- `per_capita_spending_2020.csv` - CMS per capita data
- `thce_growth_vs_benchmark.csv` - MA cost growth history
- `affordability_by_race_2023.csv` - CHIA affordability data
- `cost_breakdown_2020.csv` - Spending by category
- `2026_rate_increases.csv` - DOI rate filings
- `provider_costs_2023.csv` - Provider TME data
- `pharmacy_rebates_2023.csv` - Pharmacy spending gross/net of rebates
- `cost_growth_drivers_2023.csv` - What drove 2023's 8.6% growth

---

## License

Data from official government publications (public domain). Analysis: MIT License.

**Last Updated:** January 2025
