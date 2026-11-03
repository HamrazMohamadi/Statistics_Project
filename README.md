# Statistics Project

## Educational Attainment and Depression Screening in U.S. Adults

A five-phase statistics course project using the National Health and Nutrition Examination Survey (NHANES), August 2021–August 2023.

## Research Question

Does the prevalence of positive depression screening differ across educational attainment levels among U.S. adults aged 20 years and older, and does this association remain after adjusting for age, gender, and family income-to-poverty ratio?

Positive depression screening is defined as a PHQ-9 total score of 10 or higher.

## Dataset

**Dataset A: NHANES 2021–2023**

The analysis uses two public-use datasets:

- `DEMO_L.xpt`: Demographic information, education, income, and survey design variables.
- `DPQ_L.xpt`: Depression screening questionnaire responses.

The datasets are merged using the unique participant identifier `SEQN`.

## Project Structure

```text
Statistics_Project/
├── data/
│   ├── raw/
│   └── processed/
├── figures/
│   └── phase1/
├── notebooks/
│   └── phase1.ipynb
├── reports/
├── src/
├── PROJECT_CARD.md
└── README.md
```

## Phase 1: Data Understanding and Descriptive Statistics

Phase 1 covers:

- Data sources and study design
- Observation units and sampling
- Variable classification
- Data cleaning and quality assessment
- Frequency tables and descriptive statistics
- Measures of central tendency and dispersion
- Data visualization
- Preliminary descriptive comparisons
- Survey weights and design variables
- Analytical population and sample selection

### Analytical Samples

| Dataset | Participants |
|---|---:|
| Merged DEMO and DPQ | 6,337 |
| Adults aged 20+ | 6,064 |
| Main analytical sample | 5,208 |
| Complete-case sample | 4,584 |

### Preliminary Findings

In the main analytical sample, 12.67% of participants had positive PHQ-9 screening results.

The survey-weighted percentage was 12.19%.

Descriptive comparisons indicated lower positive-screening percentages among participants with higher educational attainment.

These findings are descriptive and do not establish statistical significance or causality.

## Reproducing the Analysis

### Requirements

- Python 3.10 or newer
- pandas
- NumPy
- Matplotlib
- Jupyter Notebook

Install the required packages:

```bash
pip install pandas numpy matplotlib jupyter
```

### Running Phase 1

1. Clone or download this repository.
2. Ensure `DEMO_L.xpt` and `DPQ_L.xpt` are located in `data/raw/`.
3. Open `notebooks/phase1.ipynb` in VS Code or Jupyter.
4. Restart the kernel and run all cells in order.
5. Check the generated CSV files in `data/processed/` and figures in `figures/phase1/`.

The notebook includes data integrity checks for participant counts and duplicate identifiers.

## Project Phases

| Phase | Topic |
|---|---|
| 1 | Data understanding and descriptive statistics |
| 2 | Probability and probability distributions |
| 3 | Statistical inference and hypothesis testing |
| 4 | Regression and association analysis |
| 5 | Integrated analysis and final reporting |

## Limitations

This is a cross-sectional observational study, so causal conclusions cannot be drawn.

The PHQ-9 is a screening instrument rather than a clinical diagnosis.

Missing data and complete-case selection may affect representativeness.

NHANES uses a complex sampling design. Appropriate weights, stratification, and clustering must be considered for population-level statistical inference.

## Data Sources

- [CDC NHANES](https://www.cdc.gov/nchs/nhanes/)
- [NHANES Demographics Documentation](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DEMO_L.htm)
- [NHANES Depression Screener Documentation](https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DPQ_L.htm)

## Project Documentation

See `PROJECT_CARD.md` for the research question, variable definitions, study design, and initial limitations.

## Raw Data Download

The raw NHANES datasets are not included in this repository.

Download the following files from the official CDC documentation pages:

- DEMO_L.xpt: https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DEMO_L.htm
- DPQ_L.xpt: https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DPQ_L.htm

Place both files in `data/raw/` before running the notebook.