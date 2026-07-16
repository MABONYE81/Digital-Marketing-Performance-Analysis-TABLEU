# Tableau Section — Key Insights (One-Pager)
**Greenside Villas | BI Dashboard Design, Jan 2025–Jun 2026**

## What this section adds beyond Excel/SQL/Python
The numbers here aren't new — they're the same funnel and trend findings from Sections 1-3, deliberately reproduced in Tableau's calculated-field language (table calculations like `WINDOW_AVG` and `RANK`, not just `SUM`/`AVG`). The value of this section is showing the same insight translated correctly into a different tool's idioms.

## The 3 things that matter

1. **A flat extract was the right call, not a multi-table join.** With only 4 channels at weekly grain, joining everything into one 27-column CSV before Tableau ever sees it is simpler and faster than making Tableau do 3 joins on every worksheet render.

2. **Table calculations need "Compute Using" set correctly, or they silently break.** `WINDOW_AVG` for the 4-week rolling Facebook reach and `RANK` for monthly revenue both depend on the right partition/addressing field (month or week_date) — a common mistake that produces a number that looks plausible but is wrong.

3. **The "Is Real Data" filter matters as much in Tableau as it did in Excel.** Without it, every average on the dashboard would be diluted by 19 future placeholder weeks that are all zeros — the same data-quality issue flagged from Section 1 onward, now solved with a single boolean calculated field applied dashboard-wide.

## Bottom line
This section is a translation exercise: same funnel bottleneck (1.89% view→inquiry), same reach-vs-bookings disconnect (trend line R² near zero), rebuilt correctly in Tableau's specific calculation model.

*Companion files: `Tableau_Weekly_Extract.csv`, `Tableau_Calculated_Fields.txt`, `Tableau_Build_Guide.docx`, dashboard mockup image.*
