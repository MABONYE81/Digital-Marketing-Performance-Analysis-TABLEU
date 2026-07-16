<img width="1896" height="1236" alt="03tableau_dashboard_mockup" src="https://github.com/user-attachments/assets/1399a3e4-c101-4294-b4ad-9194ba8956b4" />
# 06_Tableau — README

## Is there a dashboard here?
Not a live one — Tableau Desktop/Public isn't installed in the environment
that built this portfolio, so there's no `.twbx` workbook file to open.
Instead, this folder gives you everything needed to **build the real
dashboard yourself** in about 15-20 minutes, plus a labeled mockup image
showing what it should look like when done.

## What's a "mockup" vs a real dashboard?
`03_mockup/tableau_dashboard_mockup.png` is a reference image (made with
Python/matplotlib) showing the intended layout — KPI cards, charts,
positions. It is **not** a Tableau screenshot. Think of it as a blueprint,
not the finished building.

## How to build the actual dashboard
1. Install **Tableau Public** (free): https://public.tableau.com
   (or Tableau Desktop if you have a license)
2. Open Tableau → Connect → Text File → select `01_Tableau_Weekly_Extract.csv`
3. Open `04_Tableau_Build_Guide.docx` — it has the full step-by-step
   instructions, including exactly which chart type and fields to use for
   each of the 6 visuals shown in the mockup.
4. Open `02_Tableau_Calculated_Fields.txt` alongside it — it has the exact
   formula for every calculated field the guide references (copy-paste
   each one into Tableau's "Create Calculated Field" dialog).

## Why build it yourself instead of getting a finished file?
Tableau workbooks (`.twbx`) are a proprietary binary format that can't be
generated without Tableau itself installed — there was no way to produce
a working one in this sandbox. The extract, formulas, and guide are the
complete, honest alternative: real inputs, real instructions, nothing faked.

## Files in this folder
1. `01_Tableau_Weekly_Extract.csv` — the data, ready to import
2. `02_Tableau_Calculated_Fields.txt` — all 12 formulas you'll need
3. `03_mockup/` — the layout reference image
4. `04_Tableau_Build_Guide.docx` — step-by-step build instructions
5. `05_Tableau_Insights_Summary.md` — one-page takeaways
