# [Running on Empty](https://mikeharman89.github.io/mammoth-road-fatigue-analysis/)
### A two-season fatigue analysis of the Utah Mammoth - 2026 Playoff Edition

---

## The question

Standard hockey stats tell you how a player performed across a season. They don't tell you who was running on fumes when they did it.

This report asks a more specific question: **do Utah Mammoth players hold up as road trips get longer?** And does the answer change from one season to the next?

---

## What we found

We developed the **Road Trip Decay Index**, the difference in a player's points per game between game 1 of a road trip and game 3 and beyond, when cumulative travel, hotel beds, and consecutive nights of play start to compound.

Three things stood out clearly enough to matter heading into the 2026 playoffs:

**1. Logan Cooley is playoff-ready.**
His road fatigue pattern: a measurable issue across 2024/25 and the early part of 2025/26, is essentially gone in his post-return data. His decay index from February through April 2026 is 0.00. Identical production in road game 1 and road game 3+. The injury that cost Utah nine weeks of regular season appears to have functioned as an involuntary reset.

**2. The depth lines transformed.**
Kevin Stenlund improved by +0.47 year-over-year. Lawson Crouse by +0.23. Utah's third and fourth lines are dramatically more durable on the road than they were a season ago, which matters enormously in a seven-game playoff series.

**3. Watch Guenther and Keller in games 5–7.**
Both regressed in road trip durability in 2025/26, likely from heavier workloads during the playoff push. They're still elite. The data just says manage their minutes late in a deep road series.

---

## The report

The full analysis is an interactive HTML report covering:

- The Road Trip Decay Index methodology
- Clayton Keller as the fatigue-resistance baseline
- Full roster back-to-back splits
- Home vs. road trip performance for all 21 tracked skaters
- Logan Cooley's two-season arc — pre-injury, post-return, and what it means now
- Year-over-year comparison for 12 returning players
- Playoff implications by player group

**[View the report →](https://mikeharman89.github.io/mammoth-road-fatigue-analysis/)**

---

## The methodology

```
Road Trip Decay Index = pts/gm (Road Game 3+) − pts/gm (Road Game 1)
```

- **Road Game 1**: first game of any road trip, the "fresh road" baseline
- **Road Game 3+**: game three and beyond, where cumulative fatigue compounds
- Minimum 3 qualifying deep road games required for inclusion
- All data sourced from the NHL public API — no proprietary sources

A decay index of 0.00 means no drop-off. Negative means fading. Positive means the player actually gets better deep in trips.

---

## Data & tools

- **Data:** NHL public API (`api-web.nhle.com`) — game logs, rosters, schedules
- **Analysis:** Python - pandas, requests
- **Visualization:** Chart.js, matplotlib
- **Seasons covered:** 2024–25 and 2025–26 NHL regular seasons
- **Players analyzed:** 21 Utah Mammoth skaters + 12 peer comparables

---

## Related

The same Road Trip Decay Index applied across all 32 NHL teams is available here:
**[nhl-road-fatigue](https://mikeharman89.com/yourusername/nhl-road-fatigue)** — interactive dashboard, sortable league table, and travel maps for every team.
