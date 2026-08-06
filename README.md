# INTL-I103 Global Business — Fall 2026 course site

A Quarto website ported from the Fall 2024 course, updated for the Fall 2026 M/W meeting pattern and the switch from individual journals to **in-class group case write-ups**.

## What's here

| File | Purpose |
|---|---|
| `_quarto.yml` | Site config — navbar, theme, render list |
| `theme.scss` | IU crimson/cream theme (rebuilt to follow the INTL 503 conventions; that course's `.scss` wasn't accessible from this folder) |
| `styles.css` | Minor layout polish |
| `index.qmd` | Home page |
| `syllabus.qmd` | Full syllabus, updated for Fall 2026 |
| `schedule.qmd` | Week-by-week M/W schedule, readings, case days |
| `assignments.qmd` | Case write-ups, midterm, final, community participation |
| `resources.qmd` | Course pack, student support, study help |
| `CONTENT-UPDATE-FLAGS.md` | **Instructor-only** review list — decisions to make + cases needing updating (not rendered into the site) |

## How to render

This site reuses the **INTL 503 theme verbatim** (`theme.scss`, Open Sans / Roboto Slab, crimson) and the same page conventions (`hero-banner`, `info-box`, `schedule-table`, `assignment-card`), including FontAwesome `{{< fa … >}}` icons.

**Prerequisite:** the FontAwesome extension must be installed in this folder (already done — `_extensions/quarto-ext/fontawesome/`). If you ever clone this site fresh, re-run `quarto add quarto-ext/fontawesome`.

```bash
cd "Fall 2026 Course Site"
quarto preview      # live local preview
quarto render       # build the static site into _site/
```

The Week 1 slide deck (`slides/week01-intro.qmd`) uses `slides/custom.scss` and `slides/iu-trident.png`, matching your 503 deck's YAML (trident-watermark title slide, fade transitions, crimson dividers).

`quarto`, `README.md`, and `CONTENT-UPDATE-FLAGS.md` are excluded from the build via the `render:` list in `_quarto.yml`, so only the five student pages render.

## Before you publish — read `CONTENT-UPDATE-FLAGS.md`

The draft contains **visible review callouts** ("Decision needed," "Action item," "Verify before publishing"). These are intentional flags for you, not student content — **strip them before going live.** They cover:

- the unallocated 5% of the grade (currently folded into Attendance & Participation),
- the revised generative-AI policy,
- case write-up logistics (team size, count, reshuffling, individual accountability),
- time-sensitive cases needing updates (**TikTok, rare earths/UFLPA, tax/Apple–Ireland, Patagonia**),
- corrected wrong-campus (IU South Bend) contacts to verify,
- the dead HBP course-pack link,
- and break/finals dates to confirm against the registrar.

## Key facts baked in

- **Meets:** M/W 9:35–10:50, GISB 1112 · **Aug 24 – Dec 9, 2026**
- **No class:** Labor Day (Sep 7); Thanksgiving week (Nov 23 & 25) — *verify*
- **~50–60 undergraduates;** 29 class meetings
- **Grading:** Case write-ups 40% · Midterm 15% · Final 20% · Attendance & participation 20% · Community participation 5%
