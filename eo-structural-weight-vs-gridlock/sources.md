# Sources — EO Structural Weight vs. Congressional Gridlock
## "Executive Orders Get Heavier When Congress Locks Up"
### Last updated: July 2026 (supersedes the 1947-2016 version built from the Brookings/weebly-hosted series)

---

## What This Chart Shows

Mean executive order "structural weight" per Congress plotted against Sarah Binder's
congressional gridlock score (share of salient issues left unresolved), for the 80th
through 117th Congress (1947-2022) — the full range where both datasets currently overlap.
Both series are indexed to their 1947 (80th Congress) value = 100 so they can share one axis
despite having very different natural units (a roughly 0-30 structural-weight score vs. a
0-100% gridlock share).

Across the full 1947-2022 span the two series move together (Pearson r = 0.62 on the raw,
non-indexed values), consistent with the "policy conversion" / administrative-bypass
literature: when Congress is more gridlocked, presidents lean on structurally more assertive
executive orders. This is a correlation over a shared multi-decade upward trend, not proof of
causation.

**The most recent three Congresses break that pattern.** EO structural weight climbs to a new
series-high in the 117th Congress (2021-22, index 439) even as gridlock in that same Congress
falls to 184.6 (index) / 48.15% raw — its lowest level since the 111th Congress (2009-10) — and
well below the 113th Congress's record of 282.4 (73.68% raw). Binder's own account in Chapter 8
describes 2021-22 as one of the least-gridlocked Congresses since Obama's first term (bipartisan
infrastructure bill, plus two reconciliation packages), which lines up with the drop in the
gridlock series but not with the continued rise in EO structural weight. Worth flagging rather
than smoothing over.

---

## Data and Sourcing

### EO structural weight (indexed)
- **Index formula:** (value / 1947 value) × 100, using `mean_structural_weight` per Congress.
- **Source:** `scores_by_congress.csv` (EO structural-weight scoring project, this repo).

### Gridlock score (indexed)
- **Index formula:** (value / 1947 value) × 100, using the `grid4` column — the "% gridlocked
  (NYT ≥ 4 editorials)" measure, which is the one used in Binder's own published Figure 8-2 and
  in her earlier *Stalemate* / "Polarized We Govern?" work.
- **Source:** Sarah Binder, "Challenges of Legislating in Partisan Times," Chapter 8 in
  *Congress Reconsidered*, 13th ed., ed. Lawrence Dodd and Bruce Oppenheimer (Washington, DC:
  CQ Press, 2025), Figure 8-2, "Frequency of Legislative Deadlock on Salient Issues (1947-2022)."
  Underlying values from `gridlock scores 1947-2022.xlsx`, which also carries four alternate
  salience thresholds (grid1-grid3, grid5) and the raw failed-issue / agenda-size counts behind
  each threshold, not used here.
- **Note:** This replaces the previous source used for this chart (a `.xlsx` hosted on Sarah
  Binder's personal site covering 1947-2016, itself sourced from *Stalemate* and the 2014
  "Polarized We Govern?" Brookings piece). The two sources agree exactly on every overlapping
  Congress (80th-114th) — this update only extends the series three more Congresses (115th,
  116th, 117th) and switches to a citation traceable to the current textbook edition.

Raw (non-indexed) values for both series, plus the Congress number and start year, are in `data.csv`.
