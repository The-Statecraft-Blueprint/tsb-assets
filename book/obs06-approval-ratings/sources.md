# Sources — Congressional Approval Ratings Chart
## "Americans Have Never Really Approved of Congress"
### Essay: It Begins With "Why?" (GitHub Issue #107)
### Last updated: May 2026

---

## What This Chart Shows

Annual approval ratings for the U.S. Congress, as measured by Gallup, 1974–2026.

The chart shows the percentage of Americans who approve of "the way Congress is handling its job" — Gallup's standard question, asked continuously since 1974. Annual figures shown are yearly averages where available; single poll readings used for years with limited data.

---

## Primary Source

### Gallup — Congress and the Public
- **URL:** https://news.gallup.com/poll/1600/congress-public.aspx
- **Coverage:** 1974–present (continuous)
- **Notes:** Gallup is the authoritative and only continuous source for this measure dating to 1974. The question wording has been consistent throughout: "Do you approve or disapprove of the way Congress is handling its job?" Annual averages are preferred over individual poll readings to smooth out event-driven spikes.

### Key Gallup Reference Articles
- "Approval of Congress at an All-Time High" (2001) — https://news.gallup.com/poll/4564/approval-congress-alltime-high.aspx
- "Congress' Job Approval Rating Worst in Gallup History" (2010) — https://news.gallup.com/poll/145238/congress-job-approval-rating-worst-gallup-history.aspx
- "No Improvement in Congress Approval, at 13%" (2016) — https://news.gallup.com/poll/189848/no-improvement-congress-approval.aspx
- "Disapproval of Congress Ties Record High at 86%" (April 2026) — https://news.gallup.com/poll/708722/disapproval-congress-ties-record-high.aspx
- "The Decade in Review: Four Key Trends" (2009) — https://news.gallup.com/poll/124787/decade-review-four-key-trends.aspx — source for the subtitle correction below; describes the October 2001 84% reading as "shattering the previous high of 57% from February 1998."

### Quorum / Statista (supplementary)
- Quorum, "Congressional Approval Rating: 15% in 2026" — https://www.quorum.us/data-driven-insights/congressional-approval-ratings-over-time/
- Statista, Gallup congressional approval time series — https://www.statista.com/statistics/207579/public-approval-rating-of-the-us-congress/

---

## Key Confirmed Data Points

| Year | Approval | Event |
|------|----------|-------|
| 1974 | 32% | First Gallup measurement; yearly average |
| 1979 | 19% | Energy crisis / gas shortages |
| Feb 1998 | 57% | Prior all-time high, pre-9/11 — a separate, unrelated peak; superseded by the Oct 2001 reading (see "The Decade in Review: Four Key Trends") |
| 1992 | 18% | Check-bouncing scandal |
| Oct 2001 | 84% | All-time high — 9/11 rally effect |
| Jul 2008 | 14% | Then-record low; gas prices / recession |
| Nov 2013 | 9% | All-time low — government shutdown aftermath |
| Mar 2025 | 31% | Republican trifecta honeymoon peak |
| Apr 2026 | 10% | Near all-time low; 86% disapproval ties record |

**Long-run average since 1974:** 28% approval / 65% disapproval

---

## Methodology Notes

- **Annual averages vs. point readings:** Where Gallup publishes annual averages, those are used. For some years only individual poll readings are available; these are noted in data.csv.
- **The 1974 start date:** Gallup began tracking congressional approval in 1974 — the same year the FECA Amendments completed the 1970–1974 transparency reform sequence. That timing connection is the argument made explicitly in the Convergence synthesis chart (`book/convergence`), not in this Chapter 2 observation chart — the chart's 1974 reference-line marker was removed for that reason (July 2026 — see Corrections). On this series 1974 is also simply the first year Gallup data exists, so the coincidence isn't visually distinguishable from an ordinary series start.
- **The 9/11 spike:** The October 2001 reading of 84% is a genuine outlier driven by national crisis unity. The annual average for 2001 was approximately 56%. Both are noted in data.csv.
- **Event-driven fluctuations:** Approval spikes when a new party takes control of Congress (honeymoon effect) and drops sharply during shutdowns, scandals, and economic crises. These fluctuations are real but temporary — the long-run trend is what matters.
- **The 28% average:** Gallup's own summary: approval has averaged 28% since 1974, with 65% average disapproval. This is the number to cite in the essay.

---

## Corrections

| Date | Change |
|------|--------|
| 2026-07-17 | Removed the 1974 reference-line annotation from the chart (the 28% long-run-average reference line is unaffected and remains). It was built for the earlier essay (#107, "It Begins With Why?"), which had already named the FECA/transparency-reform argument; this chart now supports Chapter 2 (observation), which hasn't made that argument yet, so the marker was visually importing an unmade case. Same fix already applied to the Gridlock (`obs01-unresolved-agenda`), Party-Line Voting (`obs04-party-line-voting`), Legislation Decline (`obs01-legislative-decline`), and Moderate Decline (`obs05-moderate-decline`) charts, for the same reason. The Convergence synthesis chart intentionally keeps its 1974 indexing, since that chart is where the reform argument is actually made. |
| 2026-07-18 | Corrected the subtitle's approval-threshold claim from "It has been above 50% only briefly — once, after 9/11" to "It has been above 60% only briefly — once, after 9/11." The 50% framing was factually wrong: congressional approval also reached 57% in February 1998, a separate, unrelated peak, so "above 50%" was not unique to 9/11. What's actually true and unique to 9/11 is that approval has topped 60% exactly once — the October 2001 reading of 84%, which Gallup describes as "shattering the previous high of 57% from February 1998" (Gallup, "The Decade in Review: Four Key Trends"). Raising the threshold to 60% makes the claim accurate. |

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| May 2026 | Initial publication | TSB |
| July 2026 | Removed chart-specific 1974 marker; kept the 28% average reference line (full detail in Corrections above) | TSB |
| July 2026 | Corrected subtitle threshold from 50% to 60% — approval also hit 57% in Feb 1998, so only the 60% threshold is unique to the 9/11 spike (full detail in Corrections above) | TSB |

*If you believe a data point is incorrect, please open an issue at https://github.com/The-Statecraft-Blueprint/tsb-assets or contact us at statecraftblueprint.org.*
