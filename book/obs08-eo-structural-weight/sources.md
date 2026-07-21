# Sources — EO Structural Weight Chart
## "Executive Orders: Count vs. Structural Weight, 1969–2026"
### Chapter 2 (observation) — The Statecraft Blueprint (book manuscript)
### Last updated: July 2026

---

## What This Chart Shows

Two annual measurements for U.S. executive orders, 1969 through 2026: the raw count of executive orders issued per year, and the mean "structural weight" score per order for that year (a per-order score from 0–100%, produced by the EO Structural Weight coding project). The two series are plotted together on the same year axis with independent scales — count on the left, mean structural weight percentage on the right — so their separate year-to-year shapes can be compared directly. This chart states the two measurements; it does not interpret what drives either series.

The chart is windowed to 1969–2026, consistent with the date range used elsewhere in this chapter's observation charts. The underlying corpus covers 1936–2026 in full; see Data and Sourcing below.

---

## Data and Sourcing

### Executive order count (`n_orders`)
- **Source:** EO Structural Weight project database (`eo_coding.db`), consolidated from the executive order corpus, 1936–2026.
- **Note:** Counts reflect executive orders with an assigned EO number for that calendar year. 2026 is a partial year — see Methodology Notes.

### Mean structural weight (`mean_structural_weight_pct`)
- **Formula/derivation:** For each year, the unweighted arithmetic mean of the per-order structural weight percentage across every executive order issued that year.
- **Source:** EO Structural Weight project database, file `annual-structural-weight.csv` (`book/obs07-eo-structural-weight/` in the tsb-assets repo).
- **Note:** Mean, not median, is used as the primary series for this chart — see Methodology Notes for why.

### Validation benchmark
- **Citation:** Mayer, Kenneth R., and Kevin Price. 2002. "Unilateral Presidential Powers: Significant Executive Orders, 1949–99." *Presidential Studies Quarterly* 32: 367–386.
- **Note:** Used as the external blind-coding validation benchmark for the structural weight scoring methodology (see Methodology Notes). Not itself a data source for the count or structural weight series.

---

## Methodology Notes

- **Scoring methodology:** Each executive order is scored against a pre-registered coding rubric. The methodology was blind-coded and validated against the Mayer & Price (2002) significant-executive-order census, achieving an AUC of 0.7836 against that external benchmark.
- **Corpus coverage:** 7,149 of 7,151 executive orders from 1936–2026 have an assigned structural weight score (99.97% of the full corpus). Two orders are excluded from the percentage series: EO 9681, which has no published order text anywhere in the source corpus (title-only coding, no defined percentage, since a real denominator requires knowing what the other coding flags would find), and one June 2026 order (regenerative agriculture) whose EO number had not been assigned when the source corpus was built.
- **Coding composition:** 306 orders primary-coded (`claude-church-bells-v1` — the original Mayer & Price validation census plus a calibration set); 3,032 orders coded in Stream A (`cowork-extension-stream-a`, FDR through Truman, 1936–1953); 3,812 orders coded in Stream B (`cowork-extension-stream-b`, Eisenhower through the present). No duplicate scoring and no overlap between streams, verified directly across batch files rather than assumed.
- **Chart window (1969–2026):** This chart shows a 1969–2026 subset of the full 1936–2026 corpus, matching the date window used across this chapter's other observation charts. The full corpus, including 1936–1968, is available in `annual-structural-weight.csv` and `eo_coding.db` in the source folder for any chart that needs the longer historical sweep.
- **Mean vs. median:** This chart uses the annual mean structural weight, not the median, as the primary series. The median sits at or near zero for long stretches of the early data — multiple years in the 1969–1989 span have a median of 0.0 even though the mean is well above zero — which makes the median non-representative of the underlying per-order distribution in those years. The mean is shown as the plotted line; both mean and median are retained in `data.csv` for reference.
- **Aggregation:** Annual mean is a simple unweighted average of individual order scores — not weighted by order significance, word count, or order type. The per-order data in `eo_coding.db` supports recomputing this with alternative weightings if needed.
- **Count axis (square-root scale):** The left (count) axis uses a square-root scale rather than linear. 2025's count (238) is roughly 2.6–12.5× every other year in this series; on a linear axis, that single value would compress the visible variation among all other years toward the bottom of the chart. The square-root scale preserves 2025 as the visible maximum of the series while keeping the smaller year-to-year differences in the rest of the series legible. Exact values for every year are available on hover in `chart.html`, in the callout row (2025's count is called out directly), and in full in `data.csv`.
- **2026 (provisional):** 2026 is a partial year — 43 executive orders and a 29.16% mean structural weight as of this data pull (July 2026). Both series are marked provisional at 2026 (dashed final line segment, open point marker) and labeled "(provisional — partial year)" in the callout row and hover tooltip, consistent with how in-progress years are marked elsewhere in this chapter's charts (e.g. `obs05-moderate-decline`, `obs06-approval-ratings`).
- **No reference-line marker.** This chart was built without a 1974 (or any other) reference-line annotation from the outset. Several other charts in this chapter shipped with one and had it removed afterward (see their own sources.md Corrections sections); this chart skips that step.

---

## Known Limitations

- **Coding depth varies by source stream.** All three coding batches (primary coding plus two extension streams) used full per-flag justification, but were coded independently, by different processes, over an extended period. Section-level self-QA, including caught-and-corrected errors, is documented in each stream's own notable-patterns log.
- **Single coder identity per stream, not blind multi-coder consensus.** The Mayer & Price validation (AUC = 0.7836) demonstrates that the scoring methodology reproduces external expert judgment on that benchmark; the full-corpus extension applies that already-validated methodology at scale but was not independently re-validated end to end beyond it.
- **Raw source files:** `annual-structural-weight.csv`, `annual-structural-weight-chart.png` (full 1936–2026 corpus reference chart), and `eo_coding.db` (full per-order record) live in `book/obs07-eo-structural-weight/` in the tsb-assets repo, alongside this bundle.

---

## Corrections

| Date | Change |
|------|--------|
| 2026-07-19 | **Chart style brought in line with the rest of Ch2.** The chart read heavier than every other chart in this chapter, specifically because of the count series' bars. Three changes: (1) converted the executive-order-count series from bars to a thin navy line — same treatment as the raw series in the Party-Line Voting chart (`obs04-party-line-voting`): 2px stroke, faint area fill fading to transparent, tension 0.3. The dual-axis setup and the square-root scale on the count axis are unchanged — 2025 (238) is still roughly 2.6–12.5× every other year in the series, so the sqrt scale is still needed regardless of bar vs. line. (2) Removed the "238" text label that sat directly on the chart at the 2025 peak — it was redundant with the "238 — largest single-year count" callout already in the stat row, and having it in both places was part of what made the chart feel dense. (3) Lightened the subtitle by dropping the now-unneeded "(bars)"/"(line)" chart-type annotations (both series are lines now). The square-root-axis explanation remains where it already lived — the source line only, alongside the Mayer & Price validation note — and was not duplicated into the subtitle. The 2026-provisional treatment (open point marker, dashed connector) now applies to both series, matching each other. |

---

## Version History

| Date | Change | Author |
|------|--------|--------|
| July 2026 | Initial publication | TSB |
| 2026-07-19 | Chart style brought in line with the rest of Ch2 — count series converted from bars to a thin line, on-chart "238" label removed, subtitle lightened (full detail in Corrections above) | TSB |

*If you believe a data point is incorrect, please open an issue at https://github.com/The-Statecraft-Blueprint/tsb-assets or contact us at statecraftblueprint.org.*
