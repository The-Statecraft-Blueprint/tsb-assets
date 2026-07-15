# Sources — Wave Elections Combined Chart
## "Wave Elections Don't Change the Trajectory"
### Essay: It Begins With "Why?" (GitHub Issue #107)
### Last updated: May 2026 — audited and verified

---

## What This Chart Shows

Two series combined on a dual-axis chart, aligned by Congress, 1970–2024:

1. **House incumbency reelection rate** (left axis, blue dashed line with dots) — percentage
   of House incumbents who sought reelection and won. Measured in election years (even) but
   plotted at the seating year (odd) — the year those members were actually seated and voting.
   Source: Brookings Table 2-7, verified May 2026.

2. **Party-line voting as % of all House votes** (right axis, red line) — shifted one year
   right so each year's voting record aligns with the Congress seated that year.
   Source: Brookings Table 8-3, verified May 2026.

Both series reflect the same Congress in each year. Six wave elections are annotated at their
seating years: 1975 (Watergate), 1981 (Reagan), 1995 (GOP Revolution), 2007 (Democratic wave),
2011 (Tea Party), 2019 (Democratic wave).

**The central finding:** Before 1995, incumbency dips and party-line voting dips moved together —
new members were more independent than the veterans they replaced. After 1995, the relationship
inverted: incumbency dips and party-line voting spikes moved together — new members became more
partisan than the veterans they replaced. Something changed the relationship between
turnover and polarization at the 1995 inflection point.

---

## Primary Sources

### Incumbency Data — Brookings Table 2-7
- **URL:** https://www.brookings.edu/wp-content/uploads/2022/11/2-7-Full.pdf
- **Coverage:** 1970–2024
- **Audit status:** Verified May 2026 against Gemini Deep Research and Brookings 2026 update.
  Minor discrepancies in 2002, 2018, 2024 due to edge cases (Traficant, Mink, Pascrell).
  All substantive numbers confirmed.

### Party-Line Voting Data — Brookings Table 8-3
- **URL:** https://www.brookings.edu/wp-content/uploads/2024/11/Chpt-8.pdf
- **Coverage:** 1969–2022 (Brookings); 2023–2024 from CQ Roll Call
- **Audit status:** Verified May 2026. Exact match between Gemini and our dataset on all
  years 1969–2022. ChatGPT data for 2016–2022 found to be unreliable (appeared to confuse
  party-line vote % with party unity scores). Brookings/Gemini data used throughout.

---

## Methodology Notes

- **Data alignment:** Both series use election years as the x-axis spine. Party-line voting
  is measured by calendar year; the election year value (e.g., 2010) reflects voting in the
  outgoing Congress before the new members are seated. This means wave election years show
  the OLD Congress's voting pattern, not the new members'. The first-year effect of new
  members shows up in the FOLLOWING year's party-line data.

- **The 1994/1995 distinction:** The 1994 election year shows party-line voting at 61.8%
  (the outgoing 103rd Congress). The 1995 value — when the new Republican majority was seated
  and voting — was 73.2%, the highest to that point. This distinction matters for interpreting
  the chart: the GOP Revolution's party-line effect appears more clearly in the 1995-1996
  data than in the 1994 election year data.

- **The 2010 anomaly:** Party-line voting in 2010 was 40.0% — verified correct and
  anomalously low. The 2011 value (first year of Tea Party Congress) jumped to 75.8%.
  This is the clearest example of the "new members seated" effect in the dataset.

- **Wave election selection:** Six elections classified as waves based on net seat change
  and political context. 1992 is marked separately as "Redistricting/Perot/Scandal" — a
  different type of disruption than an ideological wave.

---

## Key Findings From This Chart

1. **Pre-1994:** Incumbency and party-line voting move loosely and independently.
   Wave elections produced genuine disruption in both metrics.

2. **1992-1994 crossover:** The lines cross. 1992 incumbency drops (redistricting/scandal),
   party-line voting spikes (Clinton budget). Not a wave election in the traditional sense —
   the 1993 spike is Clinton's doing, not Gingrich's.

3. **1994-2006:** Lines broadly move opposite each other. High incumbency correlates with
   relatively lower party-line voting. Senior members retain some independence.

4. **2006 onward:** Lines begin moving in tandem. Both parties adopt coordinated freshman
   management. New members arrive pre-organized. Capture happens faster.

5. **The shrinking dips:** Each successive wave election produces a smaller incumbency dip.
   The system absorbs disruption more efficiently over time.

---

## Audit Notes

**Corrections made in May 2026 audit:**
- Incumbency 2012: corrected from 91.0% to 89.8% (Brookings)
- Incumbency 2020: corrected from 96.3% to 94.7% (Brookings)
- Incumbency 2002: corrected from 95.9% to 96.2% (Brookings — Traficant/Mink edge cases)
- Incumbency 2024: corrected from 97.1% to 95.9% (Brookings — Pascrell edge case)

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| May 2026 | Initial publication | TSB |
| May 2026 | Audited; corrected incumbency values for 2012, 2020, 2002, 2024; verified party-line data; added full methodology notes | TSB |

*If you believe a data point is incorrect, please open an issue at
https://github.com/The-Statecraft-Blueprint/tsb-assets or contact us at statecraftblueprint.org.*
