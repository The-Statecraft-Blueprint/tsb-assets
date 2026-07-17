# Sources — Party-Line Voting Chart
## "Congress Has Stopped Deliberating"
### Essay: It Begins With "Why?" (GitHub Issue #107)
### Last updated: July 2026 (see Corrections below)

---

## What This Chart Shows

Two metrics, both drawn from the same underlying CQ Roll Call party unity study:

1. **House party-unity votes as a percentage of all House votes** — the share of roll call votes in a given year where a majority of Democrats voted against a majority of Republicans. This measures how often the full chamber divided along party lines, regardless of outcome.

2. **Average member party unity score** — the percentage of party-unity votes on which the average member voted with the majority of their own party. This measures individual compliance with party position.

The chart displays metric 1 only (house party-unity votes %) as the primary visual argument, shown as the jagged annual series (navy) with a 5-year centered moving-average trend (oxblood) — the year-to-year series is genuinely volatile (swings of 15-35 points between adjacent years are normal throughout the range, e.g. 2010's 40.0% to 2011's 75.8%), and the trend line is there to make the underlying direction legible without smoothing away that real volatility. Metric 2 data is included in data.csv for reference and for the callout statistics below the chart.

---

## Primary Sources

### Brookings Institution — Vital Statistics on Congress, Chapter 8
- **URL:** https://www.brookings.edu/wp-content/uploads/2024/11/Chpt-8.pdf
- **Tables used:** Table 8-3 (Party Unity Votes in Congress, 1953–2022) and Table 8-4 (Party Unity Scores in Congressional Voting, 1954–2022)
- **Coverage:** 1969–2022
- **Notes:** Brookings republishes the CQ Roll Call party unity series. Their notes state that recent updates use tabulations based on Voteview roll-call data. The original series was compiled by Congressional Quarterly beginning after World War II. Vital Statistics on Congress was first published in 1980 as a joint effort by Thomas E. Mann (Brookings) and Norman J. Ornstein (AEI), in collaboration with Michael Malbin (Campaign Finance Institute).
- **Definition used:** A party unity vote is "a recorded vote in the Senate or House that splits the parties — that is, a majority of voting Democrats opposed a majority of voting Republicans. Party unity scores represent the percentage of such votes on which a member voted 'yea' or 'nay' in agreement with a majority of his or her party. Percentages are normalized to eliminate the effects of absences."

### CQ Roll Call Annual Vote Studies (2023–2025)
- **URL (2024 study):** https://rollcall.com/2025/02/18/congress-party-unity-vote-studies/
- **URL (2023 study):** https://rollcall.com/2024/02/08/house-gop-had-lowest-win-rate-on-party-unity-votes-since-1982/
- **Coverage:** 2023–2025
- **Notes:** CQ Roll Call has published annual party unity studies since the end of World War II. The Brookings series draws from this same source. For years beyond the Brookings 2022 endpoint, CQ Roll Call's published summaries are used directly. The 2025 figure of 85.3% is cited as the highest level in the history of CQ's study. The 2024 House figure (65.3%) is drawn from this same 2024 study and is now plotted on the chart (see Corrections).

### Voteview (supplementary cross-check)
- **URL:** https://legacy.voteview.com/Party_Unity.htm
- **Coverage:** 35th–113th Congresses
- **Notes:** Used for cross-checking Brookings figures. Voteview provides member-level party unity scores by Congress in downloadable Excel format.

---

## Methodology Notes

- **Party-line vote definition is consistent** across the full dataset: majority of one party opposed majority of the other. This is the standard CQ Roll Call definition used since the series began.
- **Unity scores shown** in the callout statistics are House averages across both parties for comparability. Individual party scores are available in data.csv.
- **The 2025 data point** is sourced from CQ Roll Call's report covering that year, which noted it as the highest level in the history of their study. This figure covers both chambers combined.
- **Trend line:** the chart's oxblood line is a 5-year centered moving average of the House party-unity-votes series (`house_trend_5yr_centered` in data.csv), with a shortened window at the series' endpoints (1969, 2025). It is computed from, but not a substitute for, the raw annual series, which remains the primary line on the chart. The moving average bridges the 2023 data gap using the surrounding years. This mirrors the convention used on the companion Legislative Gridlock chart (`book/obs01-unresolved-agenda`).
- **Genuine data gap — 2023:** No source (Brookings, CQ Roll Call, or Voteview) publishes a House party-unity-votes percentage for 2023; CQ Roll Call's 2023 study year did not break out this particular figure. This is a real gap, not an oversight — data.csv leaves the 2023 house_party_unity_votes_pct cell blank, and the chart shows a visible break in the raw (navy) line at 2023 rather than silently connecting 2022 to 2024 as if no year were missing. (The Senate party-unity-votes figure for 2023, 81.0%, is available and included in data.csv, since it comes from a different part of the same underlying CQ study.)
- **The 1974 reference line has been removed from this chart** (as of July 2026 — see Corrections). It remains in place on other Ch. 2 charts (e.g. Government Shutdowns, Legislative Gridlock) where the FECA Amendments' effective date does align with a turning point in the data. On this chart, 1974 falls in a local dip (29.4%, lower than both 1971 and 1973) and does not correspond to any visible turning point in the House party-line-voting series, so the marker was removed here specifically rather than left as a misleading annotation.

---

## Known Limitations and Disputes

- Party unity scores measure voting alignment, not causal relationship. The chart does not itself prove that transparency reforms caused increased party-line voting — that argument is made in the essay using additional evidence. The chart shows a correlation that is consistent with the structural prediction.
- The Voteview and CQ Roll Call methodologies differ slightly in how they handle absences and procedural votes. Brookings normalizes for absences; raw counts may differ slightly. The trend direction is consistent across all methodologies.
- Pre-1969 data exists in the Brookings series (back to 1953) but is not shown in this chart, which focuses on the post-LRA period. Full historical data is available in data.csv is available upon request.

---

## Corrections

| Date | Change |
|------|--------|
| 2026-07-17 | (1) Removed the 1974 reference-line marker from this chart only — 1974 sits in a local dip (29.4%) here, not a turning point, so the marker didn't correspond to anything visible in this series; left in place on other Ch. 2 charts where it does align with the data. (2) Added a 5-year centered moving-average trend line (oxblood) alongside the raw jagged series (navy, unchanged) to make the underlying direction legible given genuine year-to-year swings of 15-35 points; added `house_trend_5yr_centered` to data.csv. (3) Added the 2024 House party-unity-votes data point (65.3%, already present in data.csv and sourced from the CQ Roll Call 2024 study cited above) to the plotted series — it had been omitted, leaving the chart jumping straight from 2022 to 2025. (4) Corrected the "avg. member unity score in 1970" callout from 74% to 72%: the 74% figure had actually been computed from 1971's House dem/gop scores (72, 76) rather than 1970's (71, 72, average 71.5% → 72%). (5) Documented 2023 explicitly as a genuine House party-unity-votes data gap (no source publishes this figure for that year) rather than leaving it silently absent; the chart now shows a visible break in the raw line at 2023, bridged by the trend line. |

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| May 2026 | Initial publication | TSB |
| July 2026 | Corrected 1970 callout stat, added 2024 data point, added trend line, removed chart-specific 1974 marker (full detail in Corrections above) | TSB |

*If you believe a data point is incorrect, please open an issue at https://github.com/thestatecraftblueprint/tsb-charts or email jason@statecraftblueprint.org. We will review, correct if warranted, and document the change in this version history.*
