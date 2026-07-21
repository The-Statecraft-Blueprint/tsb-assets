# Sources — Political Efficacy (External)
## "Agreement That Officials Don't Care Has Roughly Doubled Since the 1950s"
### Supports: Chapter 2, Observation 8 — Political Efficacy (Diagnostic). STUB as of July 2026; not yet in the draft. Issue number TBD — assign before uploading to tsb-assets.
### Last updated: July 20, 2026

---

## What This Chart Shows

This chart tracks the ANES "external efficacy" item — "Public officials don't care much what people like me think" — across every ANES study year that fielded it, 1952 through 2024, using the ANES Time Series Cumulative Data File (VCF0609) directly rather than piecing together individual study years. It shows the share of Americans who *agree*, i.e., who do *not* believe the system is listening to them.

The honest picture is noisier than a clean upward line: agreement dipped as low as 25% around 1960, climbed unevenly through the 1960s–80s, crossed 50% (majority agreement) around 1970–72, dropped sharply in 2002 (a well-documented post-9/11 rally effect on trust in government), and has run at its highest levels on record — 68.2% and 71.0% — in the two most recent readings, 2020 and 2024.

As the Obs 8 stub notes, this is a distinct construct from Approval (Obs 6): Approval grades current officials' performance; this item asks whether people believe the system hears them at all, independent of who's in office. That's why it's read as closer to a legitimacy measure than a performance measure.

**This version supersedes the version built earlier in this session**, which used five secondary-sourced/partially-derived anchor years. Jason supplied the full ANES Time Series Cumulative Data File (the authoritative source for this variable) after that version was delivered; this version is built directly from it. See "What Changed" below for the specific corrections.

---

## Data and Sourcing

### VCF0609, all years — % agree "officials don't care" (weighted)
- **Formula:** For each study year, (sum of VCF0009z weights where VCF0609 = 1 "Agree") ÷ (sum of VCF0009z weights where VCF0609 ∈ {1, 2, 3} "Agree/Disagree/Neither"). Don't-know/refused (code 9) and not-applicable (code 0, blank) are excluded from the denominator.
- **Source:** ANES Time Series Cumulative Data File, 1948–2024 (release dated 2026-02-05). Variable VCF0609, "R Feels Public Officials Don't Care" / "Government Officials Care What People Like Respondent Think." electionstudies.org. File supplied directly by Jason (downloaded locally, then a 3-column extract — VCF0004, VCF0609, VCF0009z — generated with a short local Python script and passed back for processing, after the full 163MB file repeatedly failed to transfer through the session's device bridge).
- **Weight:** VCF0009z. Per the CDF codebook's Appendices document (WEIGHTS section): weight family (0009 vs. 0010 vs. 0011) depends on which "type" of 1970 data a variable uses — VCF0609 is not listed among the Type 1/Type 2 exception variables, so it uses the default Type 0 → the "0009" family. Suffix (x/y/z) depends on sample: "z" is the combined face-to-face + web sample, the right choice for a single continuous trend spanning the pre- and post-2012 mode change.
- **Confidence level:** High. Primary source, full cumulative microdata, ANES's own harmonized coding and cross-year weight.
- **Sample sizes:** Range from ~1,000 (1986, 2008) to ~7,400 (2020) valid responses per year; see `data.csv` for exact per-year N.
- **Which years have data:** ANES did not field this item every study year. Years with no data (not plotted): 1948, 1954, 1958, 1962, and even-year-only cycles where the item wasn't included (2006, 2010, 2014, 2018, 2022). All years the item *was* fielded are plotted — nothing was cherry-picked or dropped for shape.
- **Known measurement notes:**
  - The response scale format changed over the item's history (fewer categories pre-1988, a 5-point scale 1988+), but ANES's own VCF0609 harmonization already collapses "agree strongly"/"agree somewhat" into one Agree code across every year — so no separate scale-format caveat is needed for this version (the version built earlier in this session, working from individual study-year variables directly, did need that caveat; this cumulative-file version resolves it).
  - 2008 and 2012 fielded this item to only a random half-sample of respondents (per CDF notes); the weight variable accounts for this, but per-year N is correspondingly smaller those years.

---

## What Changed From the Prior Version

The version of this chart built earlier in this session used five anchor years (1952, 1974, 2016, 2020, 2024), three of them from a secondary source (Federalism Index, a Utah Valley University project) and two pulled from individual ANES study-year documentation. Jason then supplied the actual ANES Time Series Cumulative Data File, which is the authoritative source for this exact variable. Specific corrections:

- **2024 changes from 65.1% to 71.0%.** The earlier version used variable V241726SPS (a self-administered supplemental module, smaller subsample) because that's what turned up via web search of ANES/SDA documentation. The CDF's own codebook documents that VCF0609 for 2024 is actually sourced from V242200, a different constituent variable — the one ANES's own harmonization team chose as authoritative. V242200's figure (71.0%, weighted) is what's used now.
- **2020 barely changes (66.8% unweighted before → 68.2% weighted now; 66.7% unweighted in this pull)** — the earlier pull used the correct constituent variable (V202212) and the numbers cross-validate closely; the small remaining difference is applying ANES's cross-year weight rather than leaving the sample unweighted.
- **1952 (35.8% vs. 35% before), 1974 (52.2% vs. 54% before), 2016 (59.1% vs. 59% before)** all land close to the earlier secondary-sourced figures — reassuring that the Federalism Index numbers were reasonably accurate, but these are now primary-sourced and should be treated as authoritative over the earlier version.
- **The gap between 1974 and 2016 is now filled** with 15 additional verified years (1976, 1978, 1980, 1982, 1984, 1986, 1988, 1990, 1992, 1994, 1996, 1998, 2000, 2002, 2004, 2008, 2012), resolving the main limitation flagged in the prior version.
- **The "declined by nearly half from its 1984 peak" claim in the Obs 8 stub does not hold up against this data — see below.**

---

## The Obs 8 Stub's "1984 Peak" Claim: Not Supported by VCF0609

The Obs 8 stub states that "one analysis found external efficacy declined by nearly half from its 1984 peak." Checked directly against this primary data:

- **1984 is a local dip, not a peak.** Weighted agreement in 1984 was 42.6% — lower than 1980 (54.5%) and 1986 (55.0%) on either side of it. It is not the highest point in the 1980s, let alone in the full series.
- **Under the inverse framing** (i.e., if "efficacy peaked" means the *lowest* agreement that officials don't care, the highest confidence that they do), 1984 still doesn't stand out — 1960 (25.0%) and 1956 (27.0%) show meaningfully higher efficacy than 1984 does, by either framing.
- This session could not identify the original analysis behind the stub's claim (see the prior version's sources.md and the accompanying project note for what was searched). It's possible that analysis used a different, composite efficacy index (combining VCF0609 with other items like VCF0610 or VCF0613) rather than this single item, which could produce a different trajectory. But for this specific, stub-quoted item, the "1984 peak" framing should not be used in the draft as written — recommend either dropping it or replacing it with what the primary data actually shows (the 1960 low, the 2002 dip, or the multi-decade rise culminating in 2020/2024).

---

## Known Limitations

- **This chart uses a single ANES item**, not a composite efficacy index. If the original "1984 peak" analysis referenced in the stub used a multi-item index, that would not be directly comparable to this chart and should be sourced and built separately if Jason wants it.
- **Year-to-year swings are real but noisy** at the sample sizes involved (roughly 1,000–2,200 valid responses in most years, ~3,000–7,400 in 2012/2016/2020/2024) — treat single-year jumps (e.g., 1988→1990, +13 points) with appropriate caution; a couple of points of any given year's estimate is within normal sampling variation.
- **The device bridge in this session could not transfer the full 163MB CDF CSV or the 145MB raw `.dat` file** — both repeatedly reported success but never arrived, across three retries with full waits. Jason worked around this by running a short local Python script to extract just the three needed columns (VCF0004, VCF0609, VCF0009z) into a ~1MB file, which transferred normally. Worth knowing if a denser or wider pull (e.g., a composite index, or crosstabs by party/education) is wanted later — it will likely need the same narrow-extract workaround.

---

## Corrections

**2026-07-20:** Replaced the initial 5-point, partly secondary-sourced version with the full VCF0609 series (29 verified years) computed directly from the ANES Time Series Cumulative Data File, weighted with VCF0009z. See "What Changed From the Prior Version" above for specifics. Also determined the stub's "1984 peak" claim is not supported by this item's primary data — see dedicated section above.

## Contact
For corrections or questions: Jason, jason@tracerfitness.com
