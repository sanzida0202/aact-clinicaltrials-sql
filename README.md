# AACT Prospective Cancer Trials — SQL Cohort & Patterns

Mini-project using the public **AACT** (Aggregated Analysis of ClinicalTrials.gov) Postgres database.

## What this repo contains
- `sql/01_create_view.sql` – builds a view of **prospective, completed, cancer-related** trials.
- `sql/02_breast_cancer_count.sql` – counts unique **breast cancer** studies.
- `sql/03_intervention_distribution.sql` – distribution of **intervention types**.
- `sql/04_interesting_patterns.sql` – quick text mining for **common terms** and **biomarker hits** (EGFR, HER2, ALK, PD-1/PD-L1, BRCA).

## How to run (pgAdmin)
1. Connect to AACT (provided by CTTI) in pgAdmin.
2. Open `01_create_view.sql` and run it once to create the view.
3. Run each query in `02`, `03`, `04`.  
   - Export results (CSV) and take a screenshot of the grid.

## Results (After running)
- **Breast cancer studies (distinct NCT IDs):** 5949
- Finding: Among prospective, completed, cancer-related trials in AACT, there are 5,949 distinct breast-cancer studies.
- **Intervention type distribution (top lines):**


**Intervention type distribution (top lines):**
- drug — 2909 trials
- other — 1164 trials
- behavioral — 764 trials

**Top common terms (biomarkers/keywords):**
- Paclitaxel — 194 mentions
- Trastuzumab — 171 mentions
- Placebo — 160 mentions
- Docetaxel — 146 mentions
- Cyclophosphamide — 143 mentions
