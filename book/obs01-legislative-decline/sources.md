# Sources — Legislation Decline Chart
## "Congress Is Passing Less and Less Law"
### Essay: It Begins With "Why?" (GitHub Issue #107)
### Last updated: May 2026

---

## What This Chart Shows

Public laws enacted per Congress, 91st through 118th (1969–2024).

A public law is a bill that has passed both chambers of Congress and been signed by the President (or passed over a veto). Private laws — which address individual cases rather than the general public — are excluded. Simple and concurrent resolutions, which do not carry the force of law, are also excluded.

The chart shows the raw count of public laws per two-year Congress, not the enactment rate (laws as a percentage of bills introduced). The raw count is the more intuitive measure for a general audience. The enactment rate data is included in data.csv for reference.

---

## Primary Sources

### Brookings Institution — Vital Statistics on Congress, Chapter 6
- **URL:** https://www.brookings.edu/multi-chapter-report/vital-statistics-on-congress/
- **Direct chapter PDF:** https://www.brookings.edu/wp-content/uploads/2024/11/Chpt-6.pdf
- **Coverage:** 91st–118th Congresses (1969–2024)
- **Notes:** Brookings compiles this data from the Senate Résumé of Congressional Activity and the Congressional Record. This is the standard reference for congressional workload statistics. Cross-checked against ChatGPT deep research which drew from the same Brookings source.

### Senate Résumé of Congressional Activity
- **URL:** https://www.senate.gov/reference/resources/pdf/Resumes/
- **Notes:** The Senate publishes a final résumé at the end of each Congress documenting legislative activity. Brookings draws from this source. Used for cross-verification.

---

## Methodology Notes

- **Unit of measurement:** Each data point represents one two-year Congress (e.g., the 91st Congress covers 1969–1970).
- **Public laws only:** Private laws are excluded throughout for consistency.
- **The omnibus caveat:** The raw count decline is partially explained by legislative consolidation — Congress has increasingly packaged multiple policy items into large omnibus bills rather than passing individual standalone legislation. This means the raw count decline somewhat overstates the decline in legislative activity. However, this caveat does not invalidate the trend; it reframes it. Average pages per statute rose from approximately 2.5 pages (80th Congress, 1947–48) to nearly 20 pages (111th Congress, 2009–10), meaning legislation became simultaneously rarer and more incomprehensible. The omnibus shift is itself evidence of dysfunction, not evidence of efficiency.
- **The 1974 reference line has been removed (July 2026 — see Corrections).** It was originally built to mark the completion of the 1970–1974 transparency reform sequence — the "coercion loop" argument made explicitly in the Convergence synthesis chart (`book/convergence`). This chart now serves Chapter 2 as a plain observation (raw law count decline), and Chapter 2 has not yet named that reform argument, so the marker was visually importing a case this chart doesn't make on its own. The underlying research connection is still real and still lives in the Convergence chart's sources.md.

---

## Known Limitations

- The enactment rate (laws as % of bills introduced) tells a different story than the raw count, because the number of bills introduced has also changed substantially over time. Both measures are included in data.csv. The chart uses raw count because it is more accessible to a general audience.
- Pre-91st Congress data exists in Brookings (back to the 80th Congress, 1947) but is not shown. The essay focuses on the post-LRA period beginning with the 91st Congress.
- The 119th Congress (2025–2026) is excluded because it is incomplete. As of March 31, 2026, 82 public laws had been enacted in the 119th Congress, but this figure is not comparable to completed Congresses.

---

## Corrections

| Date | Change |
|------|--------|
| 2026-07-17 | Removed the 1974 reference-line annotation from the chart. It was built for the earlier essay (#107, "It Begins With Why?"), which had already named the FECA/transparency-reform argument; this chart now supports Chapter 2 (observation), which hasn't made that argument yet, so the marker was visually importing an unmade case. Same fix already applied to the Gridlock (`obs01-unresolved-agenda`), Party-Line Voting (`obs04-party-line-voting`), and Moderate Decline (`obs05-moderate-decline`) charts, and to the Congressional Approval chart (`approval-ratings`), for the same reason. The Convergence synthesis chart intentionally keeps its 1974 indexing, since that chart is where the reform argument is actually made. |

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| May 2026 | Initial publication | TSB |
| July 2026 | Removed chart-specific 1974 marker (full detail in Corrections above) | TSB |

*If you believe a data point is incorrect, please open an issue at https://github.com/The-Statecraft-Blueprint/tsb-assets or contact us at statecraftblueprint.org. We will review, correct if warranted, and document the change in this version history.*
