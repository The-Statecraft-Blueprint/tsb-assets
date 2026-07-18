# Sources — Moderate Decline Chart
## "The Middle Has Disappeared"
### Essay: It Begins With "Why?" (GitHub Issue #107) — now supporting Chapter 2 observation
### Last updated: July 2026

---

## What This Chart Shows

The percentage of U.S. House and Senate members classified as "moderate" by DW-NOMINATE scoring, 92nd–119th Congresses (1971–2025). Both chambers are shown on the same chart because they decline along the same broad trajectory — see "Real volatility and the House/Senate lag" below for how closely, and where they differ.

**Definition of "moderate":** Members whose first-dimension DW-NOMINATE score falls between -0.25 and +0.25. This is the standard threshold used by Voteview/Poole & Rosenthal in their published polarization analyses. The first dimension captures the primary liberal-conservative spectrum (economic and governmental role). A score of 0 is perfectly centrist; -1 is most liberal; +1 is most conservative.

---

## Primary Sources

### Voteview — Congressional Roll-Call Votes Database
- **Main URL:** https://voteview.com/
- **Direct data file (used for this chart):** https://voteview.com/static/data/out/members/HSall_members.csv
- **Column reference:** https://voteview.com/articles/data_help_members
- **Polarization article with methodology:** https://voteview.polisci.ucla.edu/articles/party_polarization
- **Citation:** Lewis, Jeffrey B., Keith Poole, Howard Rosenthal, Adam Boche, Aaron Rudkin, and Luke Sonnet (2026). Voteview: Congressional Roll-Call Votes Database. https://voteview.com/
- **Notes:** DW-NOMINATE scores are derived from roll-call voting records. The methodology assigns each member a score based on their voting pattern relative to all other members across time, making scores comparable across Congresses. The proportion of moderates (|score| < 0.25) is a standard Voteview output used in political science research.

### Supporting Research (context, not data source)
- Pew Research Center, "The Polarization in Today's Congress Has Roots That Go Back Decades" (March 2022) — https://www.pewresearch.org/short-reads/2022/03/10/the-polarization-in-todays-congress-has-roots-that-go-back-decades/ — source for the House/Senate party-overlap finding (see Methodology Notes below).
- Poole, Keith T. and Howard Rosenthal (1997). *Congress: A Political-Economic History of Roll Call Voting*. Oxford University Press.
- Hare, Christopher. "The Polarization of Contemporary American Politics." — https://legacy.voteview.com/pdf/pol201410a.pdf
- Columbia Law Review, "Congressional Polarization: Terminal Constitutional Dysfunction?" — https://www.columbialawreview.org/content/congressional-polarization-terminal-constitutional-dysfunction-2/

---

## Methodology Notes

- **Data derivation (rebuilt July 2026):** Every value in `data.csv` is computed directly from `HSall_members.csv` — not interpolated, not derived from published summary graphs. For each Congress, 92nd through 119th, the chart filters to `chamber == "House"` or `chamber == "Senate"` and `party_code` in `{100, 200}` (Democrats and Republicans only — see "Party coding" below), then computes the percentage of those members whose `|nominate_dim1| < 0.25`, separately for each chamber. Members with no NOMINATE score on file for that Congress (typically those who served too briefly to generate a reliable estimate) are excluded from both the numerator and denominator for that Congress. Party and Congress fields in the source file are stored as floats for some Congresses (e.g. `100.0`) and as plain integers for others — both are parsed and treated identically.
- **What counts as "moderate":** |DW-NOMINATE dim1| < 0.25. This threshold was chosen by Voteview and is used consistently throughout the literature.
- **Party coding:** Only Democrats (ICPSR 100) and Republicans (ICPSR 200) included. Independents, third-party members, and the President (also listed in this file) excluded.
- **Member counts vary by Congress:** Voteview's member file includes everyone who served and cast roll-call votes during a Congress, including members who filled a seat mid-term after a death, resignation, or special election. This means the denominator for a given Congress is sometimes above the nominal 435 House seats or 100 Senate seats (e.g. the 111th Congress has 452 House D+R members on file). This is the standard Voteview convention and is not an error.
- **Real volatility:** Neither series is monotonic. Reading Congress-over-Congress, House moderate share rose (rather than fell) in eight of the twenty-seven transitions in this series — 1977, 1987, 1989, 1999, 2007, 2009, 2019, and 2025. The clearest example is 2007–2011: House moderate share rose from 12.6% (109th) to 13.8% (110th) to 16.5% (111th), then fell sharply to 8.8% (112th). The Senate shows a comparable number of reversals over the same period. This chart does not attempt to explain those reversals — it only reports them, since they are real and were absent from the earlier fabricated version of this chart.
- **Real volatility and the House/Senate lag:** The two chambers decline along the same broad trajectory and land in nearly the same place — 8.7% (House) and 8.9% (Senate) in the 119th Congress, down from 40.1% and 42.6% respectively in 1971. But they don't move in lockstep the whole way: the Senate's decline was slower and later than the House's for roughly two decades. Through the late 1990s and 2000s, Senate moderate share stayed in the high-teens to low-20s (e.g. 22.2% in the 108th Congress, 2003) while the House had already fallen into the low teens (13.4% that same Congress). The Senate did not fall to House-like levels until the 2010s, and the two converge only in the most recent Congresses. Both chambers show the same direction of travel and land at nearly the same endpoint; the path there was not identical.
- **The 1974 inflection (marker removed July 2026 — see Corrections):** The chart previously drew a reference line at 1974, marking the mid-1970s as the beginning of the accelerating decline and tying it to the transparency reform sequence (1970-1974 LRA/FECA) — the argument made explicitly in the Convergence synthesis chart (`book/convergence`), not yet in this Chapter 2 observation chart. The line was removed for that reason; the research observation itself is still valid and worth keeping here: Poole & Rosenthal note "Polarization was then fairly stable until the late 1970s and has been increasing steadily," which is consistent with the mid-1970s inflection visible in the data even without a drawn marker.
- **The 1994 marker (removed July 2026 — see Corrections):** The chart previously drew a reference line at 1994 as well. It has been removed for the same reason as the 1974 marker — this Chapter 2 observation chart has not yet made any causal argument about what drove the decline, and the marker's write-up named a specific mechanism the book hasn't introduced yet. See Corrections below.
- **119th Congress:** In session at the time of this data pull (July 2026); NOMINATE scores for the current Congress are provisional and will be finalized after it concludes.

---

## Key Statistics for Essay Reference

- 1971: 40.1% of House members and 42.6% of Senators were moderates (92nd Congress) — direct calculation from Voteview data
- 2025: 8.7% of House members and 8.9% of Senators were moderates (119th Congress, provisional — still in session) — the two chambers have converged to nearly the same figure
- 2013: 8.8% of House members were moderates (113th Congress); the Senate did not reach a comparable level until several Congresses later
- Party overlap in the House ended in 2002: Rep. Constance Morella (R-MD) was defeated for re-election and Rep. Benjamin Gilman (R-NY) retired, removing the last Republicans more liberal than the most conservative Democrats. Party overlap in the Senate ended in 2004, when Sen. Zell Miller (D-GA) retired. Since those points, 0 Republicans in either chamber have been more liberal than the most conservative Democrat — not "approximately zero." Source: Pew Research Center, "The Polarization in Today's Congress Has Roots That Go Back Decades" (March 2022).

---

## Corrections

| Date | Change |
|------|--------|
| 2026-07-17 | **Full rebuild from primary data.** The previous version of `data.csv` presented a 28-point series that was in fact a smooth curve interpolated between roughly three confirmed anchor points (1971, 2013, and an estimated 2025 figure) — not real per-Congress calculations, despite being labeled as such. Every value has been replaced with a number computed directly from Voteview's `HSall_members.csv` (House, 92nd–119th Congress, party_code 100/200, |nominate_dim1| < 0.25 — see Methodology Notes). The recomputed series shows genuine year-to-year volatility, including several Congress-over-Congress increases in moderate share, which the fabricated smooth curve could not show by construction. |
| 2026-07-17 | **Dropped the "50 years of uninterrupted decline — no reversal in any Congress" callout.** That claim was true of the fabricated smooth curve by construction, since a curve interpolated between three anchor points cannot show a reversal. It does not survive contact with the real data: the recomputed series rises from one Congress to the next at multiple points (see Methodology Notes). The callout has been removed rather than revised, since no accurate short version of it supports the chart's argument. |
| 2026-07-17 | **Removed the 1994 reference-line marker.** Removed for consistency with the other Chapter 2 charts, for the same reason the 1974 marker was removed above: this chapter has not yet made any causal argument about what drove the decline, and the marker's write-up named a specific mechanism from later in the book. That mechanism is not restated here. |
| 2026-07-17 | **Corrected a false sourcing claim.** This file previously stated that "the Voteview direct CSV was not publicly accessible at time of publication." That was false — `HSall_members.csv` is a public, permanently-hosted file at the URL listed above and always has been. The claim has been removed; see the rebuilt Methodology Notes for how the data was actually obtained. |
| 2026-07-17 | **Tightened the party-overlap callout.** The chart previously stated "~0 Republicans more liberal than the most conservative Democrat." The finding is exact, not approximate: per Pew Research Center (March 2022), House overlap ended in 2002 (Rep. Constance Morella defeated, Rep. Benjamin Gilman retired) and Senate overlap ended in 2004 (Sen. Zell Miller retired). The callout and this document now say "0" and cite the specific members and dates. |
| 2026-07-17 | **Added the Senate as a second series.** The chart was House-only; the party-overlap callout already referenced the Senate, which was an inconsistency in an otherwise single-chamber chart. `data.csv` now carries both chambers (with Democrat/Republican breakdowns for each), the chart plots House (navy) and Senate (oxblood) as two lines with a legend, and the callout row reports both chambers side by side. The two series decline along the same broad trajectory and converge to nearly the same figure today, though the Senate's decline lagged the House's by roughly two decades before catching down — see "Real volatility and the House/Senate lag" above. |

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| May 2026 | Initial publication | TSB |
| July 2026 | Removed chart-specific 1974 marker; kept the 1994 marker at that time | TSB |
| July 2026 | Full data rebuild from primary Voteview source; removed 1994 marker; dropped unsupported "no reversal" callout; corrected false CSV-accessibility claim; tightened overlap callout to exact figures (see Corrections above) | TSB |
| July 2026 | Added the Senate as a second series alongside the House (see Corrections above) | TSB |

*If you believe a data point is incorrect, please open an issue at https://github.com/The-Statecraft-Blueprint/tsb-assets or contact us at statecraftblueprint.org.*
