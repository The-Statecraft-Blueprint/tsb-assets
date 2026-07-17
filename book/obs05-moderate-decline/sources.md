# Sources — Moderate Decline Chart
## "The Middle Has Disappeared"
### Essay: It Begins With "Why?" (GitHub Issue #107)
### Last updated: May 2026

---

## What This Chart Shows

The percentage of U.S. House members classified as "moderate" by DW-NOMINATE scoring, 92nd–119th Congresses (1971–2025).

**Definition of "moderate":** Members whose first-dimension DW-NOMINATE score falls between -0.25 and +0.25. This is the standard threshold used by Voteview/Poole & Rosenthal in their published polarization analyses. The first dimension captures the primary liberal-conservative spectrum (economic and governmental role). A score of 0 is perfectly centrist; -1 is most liberal; +1 is most conservative.

---

## Primary Sources

### Voteview — Congressional Roll-Call Votes Database
- **Main URL:** https://voteview.com/
- **Polarization article with methodology:** https://voteview.polisci.ucla.edu/articles/party_polarization
- **Legacy polarization data:** https://legacy.voteview.com/political_polarization_2015.htm
- **Citation:** Lewis, Jeffrey B., Keith Poole, Howard Rosenthal, Adam Boche, Aaron Rudkin, and Luke Sonnet (2026). Voteview: Congressional Roll-Call Votes Database. https://voteview.com/
- **Notes:** DW-NOMINATE scores are derived from roll-call voting records. The methodology assigns each member a score based on their voting pattern relative to all other members across time, making scores comparable across Congresses. The proportion of moderates (|score| < 0.25) is a standard Voteview output used in political science research.

### Poole & Rosenthal — Published Data Points
- Poole, Keith T. and Howard Rosenthal (1997). *Congress: A Political-Economic History of Roll Call Voting*. Oxford University Press.
- Poole, Keith T. "Political Polarization." https://legacy.voteview.com/political_polarization_2015.htm
- **Key confirmed data points:** ~38% moderates in 92nd House (1971); declined to ~10% by 113th Congress (2013-14); accelerating decline continues.

### Supporting Research
- Pew Research Center, "The Polarization in Today's Congress Has Roots That Go Back Decades" (March 2022) — https://www.pewresearch.org/short-reads/2022/03/10/the-polarization-in-todays-congress-has-roots-that-go-back-decades/
- Hare, Christopher. "The Polarization of Contemporary American Politics." — https://legacy.voteview.com/pdf/pol201410a.pdf
- Columbia Law Review, "Congressional Polarization: Terminal Constitutional Dysfunction?" — https://www.columbialawreview.org/content/congressional-polarization-terminal-constitutional-dysfunction-2/

---

## Methodology Notes

- **Data derivation:** The Voteview direct CSV was not publicly accessible at time of publication. Data points are derived from published Voteview polarization graphs and confirmed endpoints in peer-reviewed papers (Poole & Rosenthal 1997, 2015; Hare 2014; Pew 2022). The trend is smooth and well-documented; intermediate values are interpolated from confirmed anchor points.
- **Anchor points (directly sourced):**
  - 92nd Congress (1971): ~38-39% moderates (Poole & Rosenthal published graph)
  - 113th Congress (2013): ~10% moderates, both chambers (Poole & Rosenthal 2015)
  - Current trend: approximately 7% (Pew 2022 and subsequent research)
- **What counts as "moderate":** |DW-NOMINATE dim1| < 0.25. This threshold was chosen by Voteview and is used consistently throughout the literature.
- **Party coding:** Only Democrats (ICPSR 100) and Republicans (ICPSR 200) included. Independents, third-party members excluded.
- **The 1974 inflection (marker removed July 2026 — see Corrections):** The chart previously drew a reference line at 1974, marking the mid-1970s as the beginning of the accelerating decline and tying it to the transparency reform sequence (1970-1974 LRA/FECA) — the argument made explicitly in the Convergence synthesis chart (`book/convergence`), not yet in this Chapter 2 observation chart. The line was removed for that reason; the research observation itself is still valid and worth keeping here: Poole & Rosenthal note "Polarization was then fairly stable until the late 1970s and has been increasing steadily," which is consistent with the mid-1970s inflection visible in the data even without a drawn marker.
- **The 1994 acceleration:** The Republican Revolution (104th Congress) marks a visible acceleration in the decline of moderates, corresponding to the discharge petition transparency reform of 1993. (This marker is unaffected by the 1974 removal — it isn't part of the 1970s reform sequence in question.)

---

## Key Statistics for Essay Reference

- 1971: ~39% of House members were moderates by DW-NOMINATE
- 2013: ~10% of House members were moderates — Voteview published figure
- 2025: ~7% estimated
- The parties have not overlapped ideologically in the House since approximately the early 2000s — there is no Republican more liberal than the most conservative Democrat, and vice versa

---

## Corrections

| Date | Change |
|------|--------|
| 2026-07-17 | Removed the 1974 reference-line annotation from the chart (the 1994 marker is unaffected and remains). It was built for the earlier essay (#107, "It Begins With Why?"), which had already named the FECA/transparency-reform argument; this chart now supports Chapter 2 (observation), which hasn't made that argument yet, so the marker was visually importing an unmade case. Same fix already applied to the Gridlock (`obs01-unresolved-agenda`), Party-Line Voting (`obs04-party-line-voting`), Legislation Decline (`obs01-legislative-decline`), and Congressional Approval (`approval-ratings`) charts, for the same reason. The Convergence synthesis chart intentionally keeps its 1974 indexing, since that chart is where the reform argument is actually made. |

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| May 2026 | Initial publication | TSB |
| July 2026 | Removed chart-specific 1974 marker; kept the 1994 marker (full detail in Corrections above) | TSB |

*If you believe a data point is incorrect, please open an issue at https://github.com/The-Statecraft-Blueprint/tsb-assets or contact us at statecraftblueprint.org.*
