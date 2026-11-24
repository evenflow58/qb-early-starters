# The 4-Star QB Is the Worst Buy in Recruiting

**What does a school actually get for the money it spends on a quarterback out of high school?**

This study started as a simple question — how often do quarterbacks at each star level start early? — and the answer to that question turned out to be the wrong headline. A player starting *somewhere* is not what the school that paid for him bought. The question that matters is **in-house delivery**: how often does one signing produce an early starter **for the school that signed him**?

The test throughout:

> **Early starter** = a quarterback who started **6 or more games in a single season** in his **first or second** college season (Year 1 = fall of his recruiting-class year; starts summed across schools if he transferred).

It covers two eras, split by the start of NIL (July 1, 2021):

- **Post-NIL:** classes **2022–2024** (signed after NIL existed; the first such classes to complete two college seasons)
- **Pre-NIL mirror:** classes **2017–2021** (all signed before NIL existed; 2021 is flagged throughout as a *transition* class — signed pre-NIL, but played under NIL and the April 2021 free-transfer rule)

📖 **Read it as a web page:** https://evenflow58.github.io/qb-early-starters/ *(GitHub Pages — same content as `index.html` in this repo)*

📊 **Check the work:** every dataset is in [`data/`](data/) as a CSV — GitHub renders them as tables right in the browser, or download them for Excel/Sheets. Full methodology, sources, and caveats are in [`reports/`](reports/).

---

## The headline: what one signing delivers, in-house

Post-NIL, the chance that a single signee becomes an early starter **for the school that signed him**:

| Star level | Signed | Delivered in-house | Rate |
|---|---|---|---|
| 5-star | 12 | 6 | **50.0%** |
| 4-star | 74 | 11 | **14.9%** |
| 3-star | 444 | 26 | **5.9%** |

A 5-star is worth roughly **3.4× a 4-star** per roster spot, and a 4-star roughly **2.5× a 3-star** (a 5-star is ~8.5× a 3-star). Those are the break-even multiples: if a 4-star costs more than ~2.5× what a 3-star costs, the 3-star portfolio wins; if a 5-star costs less than ~3.4× a 4-star, the 5-star wins. **NIL prices were not measured in this study** — the multiples are the test to apply to prices, not a price finding.

The 4-star is the worst buy in the middle: expensive enough to hurt, too unreliable to build on. **63 of 74 post-NIL 4-stars (85%) never delivered an early start at all** — and of the 15 who did start early, 4 did it for somebody else.

## The 4-star leak

"Capture" = the early starter's qualifying starts came at the school that signed him. Post-NIL, four of the five early starters who qualified elsewhere were 4-stars — Sam Leavitt, Aidan Chiles, Eli Holstein, and Demond Williams Jr. (the fifth is 5-star Julian Sayin).

| Star level | Capture, post-NIL | Capture, pre-NIL |
|---|---|---|
| 5-star | 6/7 — 85.7% | 9/11 — 81.8% |
| 4-star | 11/15 — **73.3%** | 25/27 — **92.6%** |
| 3-star | 26/26 — **100%** | 49/51 — 96.1% |

Two things to notice. First, the 3-star never leaks: every 3-star early starter in both eras qualified at his signing school. Second, **the 4-star leak is a post-NIL era effect, not a 4-star trait** — before NIL, 4-star capture was 92.6%, the best of any tier. The 2021 transition class and the free-transfer rule sit between those two numbers, so the leak should be stated as a claim about the current era, not about 4-stars as people. The post-NIL sample is also small (15 four-star qualifiers), so one or two players swing the percentage.

## The strategy: pay up, or pay almost nothing

The numbers point to the two extremes, not the middle:

- **Pay up for a true 5-star.** Half of them deliver an in-house early starter, and 86% of the ones who start do it for you. The 5-star is a different asset class from a generic 4-star.
- **Or buy 3-stars cheap, in volume, and keep starter money for later.** The hit rate is low (5.9%), but the pool is ~6× the 4-star pool, the misses are cheap, capture is 100%, and 3-stars produced more early starters per class than all blue chips combined in both eras (post-NIL 8.7 vs 7.3 per class; pre-NIL 10.2 vs 7.6). Starter money then goes to demonstrated production — a proven portal starter, or retaining your own 3-star who hit.

What the middle buys you is the worst of both: a real price, a ~15% in-house hit rate, and a one-in-four chance that even the hit starts somewhere else.

## Starts anywhere — the baseline

Early starts regardless of school: star level still predicts them steeply, and nearly identically across eras:

| Star level | Pre-NIL 2017–2021 | Post-NIL 2022–2024 |
|---|---|---|
| 5-star | 11/16 — 68.8% | 7/12 — 58.3% |
| 4-star | 27/~127 — 21.3% | 15/74 — 20.3% |
| 4+5-star | 38/~143 — 26.6% | 22/86 — 25.6% |
| 3-star | 51/~740 est. — ~6.9% | 26/444 — 5.9% |
| 2-star | 0 verified | 0 |
| 1-star | **No such pool exists** in the Composite QB lists | **No such pool exists** |

Recruiting rankings did not lose predictive power in the NIL era. What changed is who *keeps* the production.

## Retention does not single out 4-stars

One correction to the "you'd be paying every year" intuition: among post-NIL early starters, the share who **never transferred from their signing school** (leaving for the NFL or finishing eligibility counts as stayed) is **4-star 5/15 (33.3%)**, **5-star 2/7 (28.6%)**, **3-star 4/26 (15.4%)**. The 4-star actually stayed slightly better than the 5-star. The re-signing problem for 4-stars is the 85% who never start early at all, plus the capture leak — not uniquely bad retention.

Overall retention: pre-NIL (careers complete) 32.9% stayed; post-NIL (fall-2026 snapshot, can only fall) 22.9%. Mobility was already the norm before NIL — the portal opened in 2018.

## Upside — where stars still dominate

Among pre-NIL early starters, **52.6% of blue chips were NFL-drafted** (the 5-star qualifiers went 9/11, eight in Round 1) vs **21.6% of 3-stars**. The 3-star successes are real (Zach Wilson #2, Michael Penix Jr. #8, Kenny Pickett #20) but the median 3-star early starter was an undrafted G5 starter. This two-extremes approach is a strategy for getting a starter on the field cheaply, not for producing NFL quarterbacks — that still tracks star level.

## The verdict, restated

*Original hypothesis: in the NIL era, schools would be wise to recruit 3-star QBs with high upside and low downside instead of 4- and 5-star QBs they don't benefit from.*

**Mostly supported, as a post-NIL claim.** The 4-star is the tier to avoid: the lowest in-house delivery per dollar after the 5-star premium is accounted for, the worst post-NIL capture, and no retention advantage to compensate. The 5-star premium and the 3-star portfolio are both defensible — which one wins depends on the price gaps, tested against the break-even multiples above.

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
- **Counting integrity:** two summary-vs-table discrepancies were found and corrected against the player-level rows during this project (post-NIL 4-star qualifiers: 15, not 16; pre-NIL: Spencer Sanders, whose 0/10 starts line always qualified him, is included in all totals). The page and this README use the corrected, row-consistent figures. Delivery rates above are recomputed from those counts: 6/12 = 50.0%, 11/74 = 14.9%, 26/444 = 5.9%; multiples from the rates, not averaged.
- **Confounders (important):** the transfer portal launched October 2018, graduate transfers predate it, the one-time free-transfer rule arrived April 2021, NIL followed on July 1, 2021, and COVID granted blanket extra eligibility. Era differences in retention **cannot be attributed to NIL alone** — the free-transfer rule is at least as plausible a cause. The cleanest comparisons are early-starter production (nearly identical across eras) and capture.

## Caveats

- Pre-NIL 3-star pool sizes are estimates (~140–156 per class); no conclusion is sensitive to that range. About 22 of the 51 pre-NIL 3-star qualifiers rest on thinner starts sourcing (verified floor ≈ 40).
- Post-NIL retention is a fall-2026 snapshot of unfinished careers; final post-NIL retention will be lower than reported.
- Post-NIL draft outcomes are mostly incomplete and are not used in the verdicts.
- Other-positions numbers are verified floors from a prominence-selected sample, **not rates**.
- NIL dollar prices were not measured; all cost conclusions are break-even tests against the delivery multiples, not price findings.

## License

Data and text in this repository are shared under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — use them, just credit the source. Player statistics remain the property of their original publishers; this is a compilation of publicly reported facts.

*Compiled November 8, 2026. Corrections welcome — open an issue.*
