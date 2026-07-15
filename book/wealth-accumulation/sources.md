# Sources — Congressional Wealth Chart
## "Congress Is Getting Richer. You're Not."
### Essay: It Begins With "Why?" (GitHub Issue #107)
### Last updated: May 2026

---

## What This Chart Shows

Two metrics displayed together:

1. **Percentage of Congress members who are millionaires** (left axis, indigo bars) — the share of sitting members of the House and Senate whose average net worth exceeded $1 million, based on mandatory personal financial disclosures.

2. **Median U.S. household net worth, indexed** (right axis, red dashed line) — median American household net worth indexed to 1984 = 1.0, drawn from Federal Reserve Survey of Consumer Finances data. Shown as an index rather than raw dollars to make the divergence between congressional and constituent wealth visually clear on the same chart.

The chart illustrates that congressional wealth has grown substantially while median American household wealth has grown much more slowly — and declined in real terms during some periods.

---

## Primary Sources

### OpenSecrets — "Millionaires' Club" Annual Analyses
- **URL:** https://www.opensecrets.org/news/2014/01/millionaires-club-for-first-time-most-lawmakers-are-worth-1-million-plus/
- **URL (116th Congress):** https://www.opensecrets.org/news/2020/04/majority-of-lawmakers-millionaires/
- **Coverage:** 2008–2024
- **Notes:** OpenSecrets compiles annual analyses from mandatory personal financial disclosure forms filed under the Ethics in Government Act of 1978. Methodology: combines all reported asset ranges to produce an average net worth estimate per member, then counts those at or above $1 million. Some limitations: disclosure forms report asset ranges rather than exact values; top range is "Over $50 million," which OpenSecrets attempts to refine where possible. A 2018 apparent dip in the data reflects a methodology adjustment by OpenSecrets, not an actual decline in congressional wealth.

### Roll Call — "Wealth of Congress" Annual Reports
- **URL:** https://rollcall.com/2024/01/12/wealth-of-congress/
- **Coverage:** 2014–2024
- **Notes:** Roll Call publishes annual analyses of congressional personal financial disclosures. Used for cross-checking and filling gaps in OpenSecrets data. Roll Call noted that wealth gains are heavily concentrated at the top end — the wealthiest 10% of Congress hold many times the wealth of the bottom 90%.

### Ballotpedia — Personal Gain Index
- **URL:** https://ballotpedia.org/Changes_in_Net_Worth_of_U.S._Senators_and_Representatives_(Personal_Gain_Index)
- **Coverage:** 2004–2012
- **Notes:** Ballotpedia compiled a systematic study of congressional net worth changes during this period. Key finding: from 2004 to 2012, median congressional net worth grew at +1.55% annually while median U.S. household net worth declined at -0.94% annually. Used for the callout statistics below the chart.

### Ballotpedia — Net Worth of United States Senators and Representatives
- **URL:** https://ballotpedia.org/Net_worth_of_United_States_Senators_and_Representatives
- **Coverage:** 2004–2020
- **Notes:** Aggregates OpenSecrets data into yearly averages. Notes same methodology limitations as OpenSecrets.

### Federal Reserve — Survey of Consumer Finances (U.S. Household Net Worth)
- **URL:** https://www.federalreserve.gov/econres/scfindex.htm
- **Coverage:** Every 3 years, 1983–2022
- **Notes:** The Federal Reserve's triennial survey is the authoritative source for U.S. household wealth distribution. Median household net worth figures used: 1984 ≈ $65,000; 2004 ≈ $93,000; 2007 ≈ $121,000; 2010 ≈ $77,000; 2013 ≈ $81,000; 2016 ≈ $97,000; 2019 ≈ $122,000; 2022 ≈ $192,000 (all in nominal dollars). Indexed to 1984 = 1.0 for chart display.

---

## Methodology Notes

- **Pre-1978 data:** Mandatory disclosure didn't exist before the Ethics in Government Act of 1978. Figures before 1984 are estimates from academic sources and are labeled as such in data.csv.
- **The 2018 dip:** OpenSecrets changed its methodology in the 2018 analysis, producing an apparent decline in the percentage of millionaires. This reflects the methodology change, not an actual decline. A note is included in the chart.
- **Indexing the U.S. household data:** Raw dollar values are not shown for U.S. household net worth because they would not be legible on the same axis as percentages. The index (1984 = 1.0) shows the relative trajectory clearly. Raw values are in data.csv.
- **"Millionaire" threshold:** $1 million average net worth as calculated by OpenSecrets from disclosure ranges. This is the standard threshold used in political reporting.
- **Wealth concentration caveat:** Aggregate figures mask substantial inequality within Congress itself. The top 10% of congressional wealth holders hold many times the wealth of the bottom 90%. The chart shows the share who cross the $1 million threshold, not the distribution above it.

---

## Key Statistics for Essay Reference

- 2012: First time a majority of Congress were millionaires — 268 of 534 members (50.2%)
- 2024: Approximately 55% of Congress are millionaires
- 2004–2012: Congressional net worth grew at +1.55% annually; U.S. median household net worth declined at -0.94% annually (Ballotpedia Personal Gain Index)
- Congressional median net worth (~$1 million+) vs. U.S. median household net worth (~$192,000 in 2022): roughly 5:1 ratio

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| May 2026 | Initial publication | TSB |

*If you believe a data point is incorrect, please open an issue at https://github.com/The-Statecraft-Blueprint/tsb-assets or contact us at statecraftblueprint.org. We will review, correct if warranted, and document the change in this version history.*
