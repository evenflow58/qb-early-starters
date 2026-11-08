# QB Early Starters by Star Rating

**Do recruiting stars predict who actually starts early in college — and does the school that signs a quarterback actually benefit?**

This repository contains a full study of college football quarterbacks in the 247Sports Composite rankings, built around one test:

> **Early starter** = a quarterback who started **6 or more games in a single season** in his **first or second** college season (Year 1 = fall of his recruiting-class year; starts summed across schools if he transferred).

It covers two eras, split by the start of NIL (July 1, 2021):

- **Post-NIL:** classes **2022–2024** (signed after NIL existed; the first such classes to complete two college seasons)
- **Pre-NIL mirror:** classes **2017–2021** (all signed before NIL existed; 2021 is flagged throughout as a *transition* class — signed pre-NIL, but played under NIL and the April 2021 free-transfer rule)

📖 **Read it as a web page:** https://evenflow58.github.io/qb-early-starters/ *(GitHub Pages — same content as `index.html` in this repo)*

📊 **Check the work:** every dataset is in [`data/`](data/) as a CSV — GitHub renders them as tables right in the browser, or download them for Excel/Sheets. Full methodology, sources, and caveats are in [`reports/`](reports/).

---

## Headline findings

### Early-starter rates are steep — and identical across eras

| Star level | Pre-NIL 2017–2021 | Post-NIL 2022–2024 |
|---|---|---|
| 5-star | 11/16 — 68.8% | 7/12 — 58.3% |
| 4-star | 27/~127 — 21.3% | 15/74 — 20.3% |
| 4+5-star | 38/~143 — 26.6% | 22/86 — 25.6% |
| 3-star | 51/~740 est. — ~6.9% | 26/444 — 5.9% |
| 2-star | 0 verified | 0 |
| 1-star | **No such pool exists** in the Composite QB lists | **No such pool exists** |

Recruiting rankings did not lose predictive power in the NIL era. What changed is who *keeps* the production:

### Capture — the era change is here

"Capture" = the early starter's qualifying starts came at the school that signed him.

| Group | Pre-NIL | Post-NIL |
|---|---|---|
| Blue-chip (4★+5★) | 34/38 — **89.5%** (93.8% for 2017–2020 alone) | 17/22 — **77.3%** |
| 3-star | 49/51 — 96.1% | 26/26 — **100%** |

Post-NIL, nearly a quarter of blue-chip early starters (Sayin, Leavitt, Chiles, Holstein, Demond Williams Jr.) took their qualifying season to a second school. Every single 3-star early starter qualified at his signing school — and because the 3-star pool is ~5× larger, 3-stars produced **more early starters per class than all blue chips combined in both eras** (pre-NIL 10.2 vs 7.6/class; post-NIL 8.7 vs 7.3/class), despite a hit rate roughly one-quarter as high.

### Retention — starting early doesn't keep anyone put

Of early starters, the share who **never transferred from their signing school** (leaving for the NFL or finishing eligibility counts as stayed):

- **Pre-NIL (careers complete): 32.9%** — mobility was already the norm before NIL (the transfer portal opened in 2018).
- **Post-NIL (as of fall 2026, careers unfinished): 22.9%** — and this figure can only fall.
- By star level, the post-NIL drop was **largest for 3-stars** (29.5% → 15.4%) vs blue chips (36.8% → 31.8%). Successful 3-stars transfer *up*.

### Upside — where stars still dominate

Among pre-NIL early starters, **52.6% of blue chips were NFL-drafted** (the 5-star qualifiers went 9/11, eight in Round 1) vs **21.6% of 3-stars**. The 3-star successes are real (Zach Wilson #2, Michael Penix Jr. #8, Kenny Pickett #20) but the median 3-star early starter was an undrafted G5 starter.

### The hypothesis, tested

*Hypothesis: in the NIL era, schools would be wise to recruit 3-star QBs with high upside and low downside instead of 4- and 5-star QBs they don't benefit from.*

**Verdict: PARTLY SUPPORTED.** Raw production (i) and capture (ii) are supported — capture is the strongest component. Retention (iii) is only partly supported and cuts against the hypothesis by star level. Upside (iv) is not supported as stated.

The restatement the data does support:

> *For getting a quarterback on the field early and keeping his qualifying season in-house, a portfolio of 3-star QBs now delivers nearly what blue chips deliver; for keeping that quarterback for his whole career or getting an NFL-caliber player, star level still matters a great deal.*

A cost corollary (prices were **not** measured in this study): per signing, the chance of an in-house early starter is ~50% for a 5-star, ~15% for a 4-star, and ~5.9% for a 3-star. A strategy of signing 3-stars for volume and spending starter money later — on a proven portal starter, or to retain your own 3-star who hit — pays for demonstrated production instead of projection.

### Other positions (RB, WR, TE, OL, DL, LB, DB)

The same test was run at the other positions, but starts data for non-QB positions is published too inconsistently to support a full census. That section therefore reports **verified floors only — do not compute rates from them.** Directionally: the QB pattern generalises best at **RB and DB** (verified 3-star early starters reaching the top of the sport in both eras — Jonathan Taylor, Ashton Jeanty, Sauce Gardner, Nick Emmanwori), **reverses at WR post-NIL** in the floor evidence (verified early starters are blue-chip true freshmen), and is **mis-timed at OL/TE**, where value arrives in Years 3–5 (only 4 of the top-50 OL recruits of 2022 were full-season true-freshman starters). At DL/LB the starts metric itself is too distorted by rotation to judge. See `reports/04-other-positions.md`.

---

## Repository structure

```
index.html                  The full study as a single web page (also served via GitHub Pages)
data/                       All datasets as CSVs (see below)
reports/                    The four underlying research reports, with full sources
  01-qb-post-nil-2022-2024.md
  02-qb-retention-follow-up.md
  03-qb-pre-nil-2017-2021.md
  04-other-positions.md
```

### Data files

| File | Contents | Rows |
|---|---|---|
| `qb_postnil_blue_chips.csv` | Every 5★/4★ QB, classes 2022–2024, with Year 1/Year 2 starts | 86 |
| `qb_postnil_three_star_qualifiers.csv` | Every 3★ QB who met the early-starter test, 2022–2024 | 26 |
| `qb_postnil_retention.csv` | All 48 post-NIL early starters: capture, retention (Metrics A/B), fall-2026 status, transfers | 48 |
| `qb_prenil_blue_chips.csv` | Every 5★/4★ QB named in the 2017–2021 Composite lists, with starts | 142 |
| `qb_prenil_three_star_qualifiers.csv` | Named 3★ early starters, 2017–2021 (headline count is a conservative 51 — one 2018 name may be double-counted/mis-assigned) | 52 named |
| `qb_prenil_early_starters_retention.csv` | Pre-NIL early starters: capture, retention, final status, NFL draft | 90 named |
| `other_positions_verified_early_starters.csv` | **Verified floors only** — RB/WR/TE/OL/DL/LB/DB early starters with both star level and starts sourced | 22 |
| `other_positions_instructive_nonqualifiers.csv` | Near-misses and exclusions that explain the method (e.g., Sam LaPorta) | 6 |

## Methodology in brief

- **Rankings:** 247Sports Composite, final rankings, QB position (pro-style + dual-threat combined), high-school recruits in the main Composite lists only (separate JUCO rankings excluded). Reclassified players count in the class they signed in.
- **Starts:** Sports-Reference CFB game logs, cross-checked against school bios/media guides, FootballDB, and Wikipedia GP/GS tables. Every qualifier and every borderline case (4–5 starts) was individually checked.
- **Counting integrity:** two summary-vs-table discrepancies were found and corrected against the player-level rows during this project (post-NIL 4-star qualifiers: 15, not 16; pre-NIL: Spencer Sanders, whose 0/10 starts line always qualified him, is included in all totals). The page and this README use the corrected, row-consistent figures.
- **Confounders (important):** the transfer portal launched October 2018, graduate transfers predate it, the one-time free-transfer rule arrived April 2021, NIL followed on July 1, 2021, and COVID granted blanket extra eligibility. Era differences in retention **cannot be attributed to NIL alone** — the free-transfer rule is at least as plausible a cause. The cleanest comparisons are early-starter production (nearly identical across eras) and capture.

## Caveats

- Pre-NIL 3-star pool sizes are estimates (~140–156 per class); no conclusion is sensitive to that range. About 22 of the 51 pre-NIL 3-star qualifiers rest on thinner starts sourcing (verified floor ≈ 40).
- Post-NIL retention is a fall-2026 snapshot of unfinished careers; final post-NIL retention will be lower than reported.
- Post-NIL draft outcomes are mostly incomplete and are not used in the verdicts.
- Other-positions numbers are verified floors from a prominence-selected sample, **not rates**.

## License

Data and text in this repository are shared under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — use them, just credit the source. Player statistics remain the property of their original publishers; this is a compilation of publicly reported facts.

*Compiled November 8, 2026. Corrections welcome — open an issue.*
