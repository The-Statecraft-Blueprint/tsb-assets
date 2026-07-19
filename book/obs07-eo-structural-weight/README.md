# EO Structural Weight — Full Corpus, 1936–2026

*Final consolidation of the full-corpus extension. This is the dataset behind the annual chart, along with what it covers, what it doesn't, and how it was assembled.*

## Coverage

**7,149 of 7,151 executive orders from 1936–present now have a structural weight score.** The two gaps are known and documented, not oversights:
- **EO 9681** has no published text anywhere in the source corpus. It's coded — the three always-answerable decision-structure flags are scored from the title alone — but with no defined percentage, since a real denominator requires knowing what the other eight flags would find.
- **One very recent June 2026 order** (on regenerative agriculture) whose official EO number hadn't been assigned yet when the source corpus was built.

Composition:
- **306 orders** — primary coding (`claude-church-bells-v1`), the original Mayer & Price validation census plus calibration set.
- **3,032 orders** — Stream A (`cowork-extension-stream-a`), FDR and Truman, 1936–1953.
- **3,812 orders** — Stream B (`cowork-extension-stream-b`), Eisenhower through the present.

Zero duplicate scoring, zero overlap between the two extension streams, zero overlap between either stream and the primary coding — verified directly, not assumed, across every batch file that went into this.

## What's in this folder

| File | Description |
|---|---|
| `annual-structural-weight.csv` | Year, order count, mean and median structural weight, 1936–2026 |
| `annual-structural-weight-chart.png` | The chart: raw annual mean/median plus a 5-year rolling mean for readability |
| `eo_coding.db` | The full consolidated database — every coding record, every coder, fully queryable |

## Reading the trend

Mean structural weight rises from roughly 1–3% in the late 1930s to the 22–38% range by the 2020s. The rise isn't smooth — there's real year-to-year noise, visible clearly in the unsmoothed mean line — but the multi-decade direction is unambiguous. **2025 is a genuine standout** (37.93% mean, 38.89% median, 238 orders — not a small sample). **2026 is a partial year** (43 orders as of this data pull) and shouldn't be read as a completed data point; exclude it or annotate it clearly in the book chart.

## Known limitations worth carrying into the book text

- **Coding depth varies by source.** The 306 primary-coded orders and the extension streams both used full justification per flag, but they were coded independently by different processes over an extended period. Section-level self-QA is documented in each stream's own notable-patterns-log, including caught-and-corrected errors — worth citing as evidence of care, not hiding.
- **This is one continuous coder identity per stream, not a blind multi-coder consensus.** The Mayer & Price validation (AUC = 0.7836) is the piece of this project that demonstrates the methodology reproduces external judgment; this full-corpus extension applies that already-validated methodology at scale, but wasn't itself independently re-validated end to end.
- **Aggregation is a simple annual mean/median of individual order scores**, not weighted by anything (significance, word count, order type). If the book wants a different weighting, the underlying per-order data in `eo_coding.db` supports recomputing this several ways.

## Rolling up to Congress sessions or presidential terms

The per-order data (`eo_scores` and `eos` tables in `eo_coding.db`, joined on `eo_number`) has a resolvable date for every order, so aggregating to any other period — a presidential term, a Congress session — is a straightforward re-group of the same underlying data. Let me know which grouping the book actually needs and I'll produce it directly rather than you reconstructing it from the annual figures.
