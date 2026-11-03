# Project Card

## Project Title
Educational Attainment and Positive Depression Screening Among U.S. Adults: NHANES 2021–2023

## Dataset
Dataset A: National Health and Nutrition Examination Survey (NHANES), August 2021–August 2023.

Data files:
- DEMO_L.xpt: Demographic variables and sample weights
- DPQ_L.xpt: Depression screening questionnaire

Data source: Centers for Disease Control and Prevention (CDC), National Center for Health Statistics (NCHS).

## Research Question
Does the prevalence of positive depression screening differ across educational attainment levels among U.S. adults aged 20 years and older, and does this association remain after adjusting for age, gender, and family income-to-poverty ratio?

## Study Design
Cross-sectional observational study using publicly available NHANES survey data.

## Population and Unit of Observation
The target population is civilian, noninstitutionalized U.S. adults aged 20 years and older.

Each row represents one individual participant, identified by SEQN.

## Main Variables

| Variable | Role | Measurement Type |
|---|---|---|
| Positive PHQ-9 screening (score ≥ 10) | Response | Binary |
| Educational attainment (DMDEDUC2) | Main explanatory variable | Ordinal categorical |
| Age (RIDAGEYR) | Adjustment variable | Quantitative |
| Gender (RIAGENDR) | Adjustment variable | Nominal categorical |
| Family income-to-poverty ratio (INDFMPIR) | Adjustment variable | Quantitative |

The PHQ-9 total score is calculated from nine questionnaire items, with possible scores from 0 to 27. Positive screening is defined as a score of at least 10 and does not constitute a clinical diagnosis of depression.

## Research Question Type
Comparative and associational.

## Initial Hypothesis
The prevalence of positive depression screening differs across educational attainment groups. An association may remain after adjusting for age, gender, and family income-to-poverty ratio.

## Initial Limitations
1. The cross-sectional observational design does not establish causality.
2. Missing questionnaire responses and income data may introduce selection bias.
3. The PHQ-9 is a self-reported screening instrument rather than a clinical diagnosis.
4. NHANES uses a complex survey design, requiring appropriate sampling weights and variance estimation for population-level inference.

## Planned Analysis
Phase 1: Data understanding, cleaning, descriptive statistics, and visualization.

Phase 2: Probability and empirical distributions.

Phase 3: Statistical inference and hypothesis testing.

Phase 4: Regression and adjusted association analysis.

Phase 5: Integration, sensitivity analysis, and final reporting.

## Official Documentation
- https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DEMO_L.htm
- https://wwwn.cdc.gov/Nchs/Data/Nhanes/Public/2021/DataFiles/DPQ_L.htm