# Sources — Convergence Chart
## "Seven Trajectories. One Starting Point."
### Essay: It Begins With "Why?" (GitHub Issue #107)
### Last updated: May 2026

---

## What This Chart Shows

Seven independent measures of congressional function, all indexed to their 1974 value = 100. The chart is designed so that "worse" always means "up" — declining metrics are inverted so that all seven lines move in the same visual direction when things are getting worse.

This is a synthesis chart, not a primary data chart. Its purpose is to show that seven completely independent datasets, measuring completely different things, all bend in the same direction at the same starting point (1974) and have never reversed. The chart is deliberately dense — it is not designed to be read data-point by data-point, but to be experienced as a pattern.

---

## The Seven Series and Their Sources

### 1. Laws Enacted (Declining = Bad, Inverted)
- **Index formula:** (1974 value / current value) × 100. Higher = fewer laws = worse.
- **1974 baseline:** 649 public laws enacted (93rd Congress)
- **Source:** Brookings Institution, Vital Statistics on Congress, Ch. 6
- **See:** `0107/legislation-decline/`

### 2. Shutdown Duration (Rising = Bad)
- **Index formula:** Cumulative shutdown severity proxy, 1974 = 100
- **Source:** CRS Federal Funding Gaps; `0107/shutdown-escalation/`
- **Note:** No real shutdowns before 1981 (Civiletti opinion). The index rises from baseline as shutdown frequency and duration increase.

### 3. Party-Line Voting (Rising = Bad)
- **Index formula:** (current % / 1974 %) × 100
- **1974 baseline:** 29% of House votes were party-line
- **Source:** Brookings Vital Statistics Ch. 8; CQ Roll Call
- **See:** `0107/party-line-voting/`

### 4. Moderate Members (Declining = Bad, Inverted)
- **Index formula:** (1974 value / current value) × 100. Higher = fewer moderates = worse.
- **1974 baseline:** ~30% of House members were moderate (DW-NOMINATE |score| < 0.25)
- **Source:** Voteview/Poole & Rosenthal
- **See:** `0107/moderate-decline/`

### 5. Congressional Approval (Declining = Bad, Inverted)
- **Index formula:** (1974 value / current value) × 100. Higher = lower approval = worse.
- **1974 baseline:** 32% approval (Gallup)
- **Source:** Gallup, Congress and the Public
- **See:** `0107/approval-ratings/`

### 6. Wealth Gap (Rising = Bad)
- **Index formula:** Ratio of congressional wealth growth to median household wealth growth, 1974 = 100
- **Source:** OpenSecrets; Roll Call; Federal Reserve SCF
- **See:** `0107/congressional-wealth/`

### 7. Incumbency Paradox (Rising = Bad)
- **Index formula:** Incumbency rate divided by approval rate (both normalized), 1974 = 100
- **Measures:** The growing paradox between how much Americans disapprove of Congress and how consistently they re-elect the same members
- **Source:** Brookings Table 2-7; OpenSecrets; Gallup
- **See:** `0107/incumbency-rates/` and `0107/approval-ratings/`

---

## Methodology Notes

- **Indexing rationale:** Different metrics have different scales and units. Indexing to 1974 = 100 allows all seven to appear on the same chart. The 1974 baseline was chosen because it is the year the coercion loop (the essay's central argument) became fully operational with the FECA Amendments.
- **The "worse = up" convention:** All series are oriented so that upward movement means worse congressional function. Declining metrics (laws enacted, moderate members, approval) are inverted. This is an editorial choice to make the convergence visually clear.
- **This is a synthesis chart:** The underlying data for each series is documented in its own chart bundle. This chart does not introduce new data — it combines existing series to show the convergence pattern.
- **The intentional density:** The chart is designed to be overwhelming in a specific way. The reader is not expected to track seven lines individually. They are expected to see that all seven lines move together from the same starting point. The legend clarifies what each line represents, but the gestalt is the argument.

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| May 2026 | Initial publication | TSB |

*For questions about individual series, see the sources.md in each chart's folder.*
