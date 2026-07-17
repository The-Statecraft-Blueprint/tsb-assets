# Sources — Party-Line Vote Explainer

## "What Counts as a 'Party-Line Vote'"
### Companion explainer for *The Rules that Shape the Rules*, Chapter 2, Observation 4 (Party-Line Voting)
### Last updated: July 2026

---

## What This Chart Shows

This is a definitional diagram, not a data chart. Before Chapter 2, Observation 4 presents the actual historical trend in party-line voting, readers need to know exactly what the term means — and the definition is narrower than people assume. A "party-line vote" is any roll call on which a majority of one party votes one way and a majority of the other party votes the opposite way. Its named counterpart, a "bipartisan vote," is one where both parties' majorities land on the same side. Neither term requires unanimity within a party.

The diagram uses two schematic 20-member "party blocs" per panel — not real chamber sizes or real votes — to show the test in action. Panel A shows a case that counts as party-line (each party's majority opposes the other's, even though several members on each side crossed over). Panel B shows a bipartisan case (both parties' majorities land on the same side, even though a large minority in each party dissented). The point is to make clear that the test is about where each party's *majority* lands, not about party discipline or unanimity.

The actual Obs. 4 evidence chart — the historical share of House roll calls that were party-line votes over time — is a separate, forthcoming asset built from real CQ/Voteview vote data (per the Binder methodology already scoped for that observation). This explainer does not substitute for that chart; it only establishes the terms.

---

## Data and Sourcing

### Definition of "party-line vote" / "bipartisan vote"
- **Formula:** A roll call is a party-line vote if a majority of voting members of Party X vote one way AND a majority of voting members of Party Y vote the opposite way. It's a bipartisan vote if both parties' majorities land on the same side.
- **Primary source:** *Congressional Record* (1956), Vol. 102, Pt. 11, p. 15069 — "A party-line vote is one on which a majority of Republicans vote one way and a majority of Democrats vote another. [...] A bipartisan vote is one in which a majority of Republicans and a majority of Democrats vote the same way."
- **Verification note:** This citation (volume/part/page) is corroborated via the Wikipedia article "Party-line vote," which attributes it to the Congressional Record. I have not independently pulled the scanned 1956 bound volume (available via GovInfo's CRECB collection, https://www.govinfo.gov/app/collection/crecb) to confirm the exact wording against the primary document itself. Treat as CONTESTED-but-plausible per TSB's confidence taxonomy until someone checks the bound volume directly — the citation is precise enough (exact page number) that it's very likely accurate, but it hasn't been eyes-on verified against the source.
- **Corroborating source (operational/statistical definition, same threshold):** CQ Roll Call (formerly Congressional Quarterly), "CQ VoteWatch Methodology," updated 2023: https://cqhelp.zendesk.com/hc/en-us/articles/15610715535643-CQ-VoteWatch-Methodology — "Party unity votes are any 'yea' or 'nay' roll call votes that have a majority of one party opposing a majority of the other party." This is CQ's own current, freely accessible methodology page — a better citation than CQ's older paywalled almanac archives. CQ Roll Call states it has analyzed voting patterns since 1945, with its three current vote studies (including party unity) "conducted consistently since 1953."
- **Secondary/journalistic source, useful for a pull-quote:** Roll Call, "Vote studies 2024: House GOP unity inched up as Senate Democrats set record" (Feb. 18, 2025): https://rollcall.com/2025/02/18/congress-party-unity-vote-studies/ — quotes CQ's own 1947 explanation of why bipartisan votes are excluded: "It should be emphasized that the analysis does not include votes in which the majority of both parties voted the same way; if such votes were included, the party loyalty record of each member of Congress would look better percentage-wise, but it would be less significant."
- **Important distinction:** The *Congressional Record* is the official government transcript of floor proceedings and debates (published by the U.S. Government Publishing Office) — it does not itself compute or score votes. The 1956 quote above is language *entered into* the Record (e.g., in a report, floor statement, or reference material reprinted there), not an editorial classification the Record performs on an ongoing basis. *Congressional Quarterly / CQ Roll Call* is the private organization that has actually computed and published party unity scores continuously since the 1950s — that's the operational source the real Obs. 4 evidence chart will draw on.
- **Note on the 1953 date:** CQ Roll Call's own page states analysis "since 1945" but the three-study series "conducted consistently since 1953." The chart's "1953" stat reflects the latter, more precise claim.

### Illustrative panel data (Panel A / Panel B dot counts)
- **Formula/derivation:** Hand-constructed to satisfy the definition above cleanly — not drawn from any real roll call.
- **Source:** N/A — schematic only. See `data.csv` for the exact tallies plotted.
- **Note:** Deliberately generic ("Party A" / "Party B," not named parties) to keep the explainer non-partisan and reusable regardless of which party the real Obs. 4 data eventually shows holding higher or lower unity, even though the source quote itself names Republicans and Democrats. Confidence level: N/A (illustrative, not an empirical claim).

---

## Corrections

- **2026-07-15:** Replaced initial citation (Voteview + an unverified "since 1953" claim sourced only from an AI web-search summary, not a direct fetch) with CQ Roll Call's own official methodology page, directly fetched and confirmed. Replaced right-hand panel label "Not a Party-Line Vote" with "Bipartisan Vote" and swapped the definition-box quote to the *Congressional Record* (1956) language, per Jason's research — this also resolved an open question about whether the term traces to the Congressional Record or Congressional Quarterly (answer: both are legitimate, independent sources for the same underlying threshold; see verification note above).

## Contact

For corrections or questions: jason@tracerfitness.com
