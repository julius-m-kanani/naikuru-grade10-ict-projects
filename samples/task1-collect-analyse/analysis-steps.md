# Task 1 — Spreadsheet Analysis Steps (Excel / Calc / Sheets)
## Using the file `waste-management-survey-20-respondents.csv`

### 1. Prepare the worksheet
1. Open the CSV in your spreadsheet app and save as `GroupXX_Task1_Spreadsheet.xlsx`.
2. Row 1 = headings (already given). Freeze top row: View > Freeze Panes > Freeze Top Row.
3. Add borders, bold headings, centre-align ratings.

### 2. Summary table (create in columns K–M, starting row 1)
Build a small summary block like this:

| Measure | Formula example (row numbers assume data in rows 2–21) | Expected result on sample data |
|---|---|---|
| Total respondents | `=COUNTA(A2:A21)` | 20 |
| Average cleaning days/week | `=AVERAGE(E2:E21)` | 3.45 |
| Average cleanliness rating | `=AVERAGE(F2:F21)` | 2.75 |
| Max cleaning days | `=MAX(E2:E21)` | 6 |
| Min cleaning days | `=MIN(E2:E21)` | 1 |
| Count: Plastic as common waste | `=COUNTIF(C2:C21,"Plastic")` | 10 |
| Count: Food waste | `=COUNTIF(C2:C21,"Food")` | 6 |
| Count: Compound waste | `=COUNTIF(C2:C21,"Compound")` | 4 |
| Count: Dispose in Bin | `=COUNTIF(D2:D21,"Bin")` | 8 |
| Count: Throw on Ground | `=COUNTIF(D2:D21,"Ground")` | 4 |
| % using bin | `=COUNTIF(D2:D21,"Bin")/COUNTA(A2:A21)*100` | 40% |
| Low rating (1–2) flag | `=IF(F2<=2,"Needs attention","OK")` — copy down | — |

### 3. Create at least one chart
- **Bar chart:** select your COUNTIF summary for CommonWaste (Plastic 10, Food 6, Compound 4) > Insert > Column/Bar Chart. Title: "Common Waste Types Observed (n=20)".
- **Pie chart (alternative):** Disposal methods: Bin 8, Pit 5, Ground 4, Burning 2, CarryHome 1. Title: "How Respondents Dispose of Litter".
- Add data labels, axis titles and legend. Place chart on the same sheet below data or on a new sheet named `Charts`.

### 4. Save and check
- Sheet names: `RawData`, `Analysis`, `Charts` (or all on one neat sheet — acceptable).
- Spelling, number formats (1 decimal for averages), chart titles.
- Save as `GroupXX_Task1_Spreadsheet.xlsx`.

### What the teacher expects to see
Headings + 20 rows + at least 4 correct formulas + 1 titled chart + correct file name.
