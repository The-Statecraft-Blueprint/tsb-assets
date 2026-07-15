# Sources — Party-Line Voting Chart
## "Congress Has Stopped Deliberating"
### Essay: It Begins With "Why?" (GitHub Issue #107)
### Last updated: May 2026

---

## What This Chart Shows

Two metrics, both drawn from the same underlying CQ Roll Call party unity study:

1. **House party-unity votes as a percentage of all House votes** — the share of roll call votes in a given year where a majority of Democrats voted against a majority of Republicans. This measures how often the full chamber divided along party lines, regardless of outcome.

2. **Average member party unity score** — the percentage of party-unity votes on which the average member voted with the majority of their own party. This measures individual compliance with party position.

The chart displays metric 1 only (house party-unity votes %) as the primary visual argument. Metric 2 data is included in data.csv for reference and for the callout statistics below the chart.

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
- **Notes:** CQ Roll Call has published annual party unity studies since the end of World War II. The Brookings series draws from this same source. For years beyond the Brookings 2022 endpoint, CQ Roll Call's published summaries are used directly. The 2025 figure of 85.3% is cited as the highest level in the history of CQ's study.

### Voteview (supplementary cross-check)
- **URL:** https://legacy.voteview.com/Party_Unity.htm
- **Coverage:** 35th–113th Congresses
- **Notes:** Used for cross-checking Brookings figures. Voteview provides member-level party unity scores by Congress in downloadable Excel format.

---

## Methodology Notes

- **Party-line vote definition is consistent** across the full dataset: majority of one party opposed majority of the other. This is the standard CQ Roll Call definition used since the series began.
- **Unity scores shown** in the callout statistics are House averages across both parties for comparability. Individual party scores are available in data.csv.
- **The 2025 data point** is sourced from CQ Roll Call's report covering that year, which noted it as the highest level in the history of their study. This figure covers both chambers combined.
- **Missing data:** Some 2023 member-level scores are not broken out in available summaries; the 2023 row in data.csv is partially complete.
- **The 1974 reference line** marks the year the FECA Amendments took effect, completing the 1970–1974 transparency reform sequence that is the central argument of this essay. The reference line is an editorial annotation, not a data point.

---

## Known Limitations and Disputes

- Party unity scores measure voting alignment, not causal relationship. The chart does not itself prove that transparency reforms caused increased party-line voting — that argument is made in the essay using additional evidence. The chart shows a correlation that is consistent with the structural prediction.
- The Voteview and CQ Roll Call methodologies differ slightly in how they handle absences and procedural votes. Brookings normalizes for absences; raw counts may differ slightly. The trend direction is consistent across all methodologies.
- Pre-1969 data exists in the Brookings series (back to 1953) but is not shown in this chart, which focuses on the post-LRA period. Full historical data is available in data.csv is available upon request.

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| May 2026 | Initial publication | TSB |

*If you believe a data point is incorrect, please open an issue at https://github.com/thestatecraftblueprint/tsb-charts or email jason@statecraftblueprint.org. We will review, correct if warranted, and document the change in this version history.*
