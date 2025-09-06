# DLL Nozzle – Needle Lapping Elimination (Bosch Nashik)

Process-improvement project to eliminate the **needle lapping** step in DLL nozzle manufacturing by tightening upstream grinding, measurement, and assembly checks. Repository includes data cleaning, deviation analysis (Ghiringhelli), needle classification, assembly time study, and result dashboards.

## Objectives
- Quantify surface/profile deviations driving lapping.
- Improve finish/seat grinding and inspection rules to avoid lapping rework.
- Validate assembly performance (HTF, repetition, visual) post-change.

## Data
Place originals in `data/raw/` (kept out of git):
- *Ghiringhelli Deviation.xlsx* – profile deviations / gauge comparisons  
- *Assembly Reading.xlsx* & *Analysis of Assembly.xlsx* – HTF, repetition, visual outcomes  
- *Needle Classification (First/Second/Third Set).xlsx* – acceptance/reject labeling  
- *Assembly Time Analysis.xlsx* – takt/time study

Processed/cleaned outputs land in `data/processed/`.

## Methods (high level)
1) **Data cleaning & standardization** – column names, units, tolerances; remove test duplicates.  
2) **Deviation analysis** – profile error metrics, trend charts, capability (Cp/Cpk), control charts.  
3) **Classification logic** – simple rules (tolerances) + optional ML baseline to predict accept/rework.  
4) **Assembly study** – HTF/visual/repetition pass-rates; time study vs. throughput.  
5) **Results** – charts and a single-page summary in `reports/`.

