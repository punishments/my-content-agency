# Account Baseline

**Last updated:** 2026-03-29
**Data source:** `analytics/raw/account_posts_mar21_pt1.csv` + `analytics/raw/account_posts_mar21_pt2.csv`
**Data range:** December 26, 2025 — March 13, 2026
**Posts included:** 83 posts with view data (3 test posts with no views excluded)

---

## Core Metrics

| Metric | Value |
|--------|-------|
| Total posts | 83 |
| Total views | 393,356 |
| Average views (mean) | 4,739 |
| Median views | 480 |
| Highest performing post | 199,089 views |
| Lowest performing post | 116 views |

**Note on average vs. median:** The mean (4,739) is heavily skewed by 3 outlier posts in early February (199,089 / 55,684 / 44,846). The median (480) better reflects typical post performance. Only 6 of 83 posts exceed the mean.

---

## Baseline Performance

**Baseline defined as:** Average views = **4,739**

| Metric | Value |
|--------|-------|
| Posts above baseline | 6 (7.2%) |
| Posts at or below baseline | 77 (92.8%) |

**Posts above baseline:**
| Views | Name | Date |
|-------|------|------|
| 199,089 | headlines are focusing on brad arnold's passing | Feb 8, 2026 |
| 55,684 | why don't celebrity deaths matter? | Feb 7, 2026 |
| 44,846 | most people think of success in headlines | Feb 10, 2026 |
| 13,096 | "this will get you pregnant.docx" | Jan 25, 2026 |
| 8,486 | NON NEGOTIABLES | Mar 12, 2026 |
| 6,112 | UNFORTUNATELY I DO LOVE | Mar 10, 2026 |

---

## Top Posts

| Rank | Views | Name | Date | Format | Funnel |
|------|-------|------|------|--------|--------|
| 1 | 199,089 | headlines are focusing on brad arnold's passing, but missing moments he helped others | Feb 8, 2026 | Silent / b-roll | Attract |
| 2 | 55,684 | why don't celebrity deaths matter? | Feb 7, 2026 | Talking head | Nurture |
| 3 | 44,846 | most people think of success in headlines, watching brad arnold reminds us connection matters | Feb 10, 2026 | Silent / b-roll | Attract |
| 4 | 13,096 | "this will get you pregnant.docx" | Jan 25, 2026 | Silent / b-roll | Nurture |
| 5 | 8,486 | NON NEGOTIABLES | Mar 12, 2026 | Silent / b-roll | Attract |

---

## Format Breakdown

**Classification method:** Posts with "Talking head" or "Voiceover" in the format field are counted as Talking. All others (Silent / b-roll, Photo, Carousel, Meme, Green screen, Split screen, Relatable/Entertainment) are counted as Non-talking. Several posts use compound formats — classified by primary format listed first.

| Format category | Post count | Total views | Average views |
|----------------|------------|-------------|---------------|
| Talking (Talking head / Voiceover) | 9 | 60,660 | 6,740 |
| Non-talking (all other formats) | 74 | 332,696 | 4,496 |

**Talking posts included in count:** contrarian AI talking head, Aerial silks Neptune City, Week 1: Creating Gabby, Week 2: Creating Gabby, why don't celebrity deaths matter?, long distance — what do all these couples have in common?, I used to think if I keep my head down, Unpopular opinion: normal never wins, planning to post your baby photos.

**Note on skew:** Talking average (6,740) is pulled by the 55,684-view post. Non-talking average (4,496) is pulled by the 199,089-view post. Both averages are skewed.

---

## Distribution Actuals

| Dimension | Count | % of total |
|-----------|-------|------------|
| Attract | 49 | 59% |
| Nurture | 24 | 29% |
| Position | 8 | 10% |
| Convert | 1 | 1% |
| Talking | 9 | 11% |
| Non-talking | 74 | 89% |
| Live status | 66 | 80% |
| Trial status | 17 | 20% |

---

## Execution Review

| Check | Status |
|-------|--------|
| Data range | Dec 26, 2025 — Mar 13, 2026 (~11 weeks) |
| Posts with view data | 83 |
| Test posts excluded (no view data) | 3 |
| Duplicate rows removed | Yes — both CSV files de-duplicated before analysis |
| Pipeline adherence tracked | Not tracked in this dataset |
| QA'd posts | Partial — QA column present but not consistently populated |

---

## Data Usage Rules

**General account data** is operational only.

- **Use for:** Baseline tracking, distribution reporting, execution review
- **Do not use for:** Hook analysis, format recommendations, creative strategy, or pattern identification across the general post set
- **Strategic direction source:** 7x7 research (`/research/`) and defined frameworks (`/docs/`)

**Exception — outliers and breakout performers:**
Posts that significantly exceed the baseline (defined as posts above the mean) may be examined for hook analysis, pattern observations, and content recommendations. These posts have broken from the noise sufficiently to warrant closer inspection.

Outlier threshold (current): **> 4,739 views** (the mean)

Current outliers: headlines are focusing on brad arnold's passing (199,089), why don't celebrity deaths matter? (55,684), most people think of success in headlines (44,846), "this will get you pregnant.docx" (13,096), NON NEGOTIABLES (8,486), UNFORTUNATELY I DO LOVE (6,112)

General account data at this stage is too noisy for broad strategic conclusions. Patterns across the general post set require a minimum of 3+ months of consistent, pipeline-adherent output before they are readable. Outlier analysis is the exception — not a license to draw conclusions from the overall dataset.
