# NHANES Data Documentation

## Official Data Source

National Health and Nutrition Examination Survey (NHANES), August 2021–August 2023.

Source: Centers for Disease Control and Prevention (CDC), National Center for Health Statistics (NCHS).

## Required Raw Files

- DEMO_L.xpt — Demographics and survey design variables
- DPQ_L.xpt — Depression screening questionnaire

Official documentation:

- https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DEMO_L.htm
- https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DPQ_L.htm

Data download date: Not recorded.

## Reproducing the Dataset

1. Download both XPT files from the official CDC pages.
2. Place them inside `data/raw/`.
3. Install the required Python packages using `requirements.txt`.
4. Open `notebooks/phase1.ipynb`.
5. Restart the kernel and run all cells in order.

The notebook generates three processed CSV datasets in `data/processed/`:

- nhanes_adult_clean.csv
- nhanes_phq9_analytical.csv
- nhanes_complete_case.csv

Raw datasets are excluded from the submitted archive. Processed datasets can be reproduced by executing the notebook.