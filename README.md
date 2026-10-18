# Housing Affordability Dissatisfaction in Canada

### A Data Analytics and Machine Learning Capstone Project

## Project Overview

This project investigates housing affordability dissatisfaction among Canadian households using the **2022 Canadian Housing Survey (CHS)**.

The objective is to understand how household income, dwelling ownership, household composition, geographic location, and housing characteristics are associated with dissatisfaction with housing affordability.

The project combines exploratory data analysis, survey-weighted statistics, and machine learning to identify patterns and evaluate the predictability of housing affordability dissatisfaction.

## Research Questions

1. What proportion of Canadian households reported dissatisfaction with housing affordability in 2022?
2. Which household, financial, dwelling, and geographic characteristics are associated with housing affordability dissatisfaction?
3. Can machine learning models predict housing affordability dissatisfaction using household and dwelling characteristics?
4. Which variables contribute most to model predictions?

## Dataset

**Source:** Statistics Canada — Canadian Housing Survey (2022), Public Use Microdata File (PUMF).

**Dataset:** Approximately 38,657 household records.

**Target variable:** `PDWS_10C` — Dwelling satisfaction: affordability.

The binary classification target is defined as:

- `1` — Dissatisfied or very dissatisfied
- `0` — Not dissatisfied
- Missing responses are excluded from target-based analysis.

Household survey weights (`PFWEIGHT`) are used for population-level descriptive estimates.

## Methodology

**1. Data Profiling and Audit**

- Examine variable distributions and missing values.
- Validate survey codes and categories.
- Evaluate target-class imbalance.
- Compare weighted and unweighted statistics.

**2. Exploratory Data Analysis (EDA)**

- Examine affordability dissatisfaction by province.
- Compare dwelling ownership groups.
- Analyze household size and annual income.
- Visualize survey-weighted dissatisfaction rates.

**3. Data Preprocessing**

- Select relevant predictors.
- Handle missing values.
- Encode categorical features.
- Prepare training and testing datasets.

**4. Machine Learning** *(planned)*

- Dummy classifier
- Logistic regression
- Decision tree
- Random forest

**5. Model Evaluation** *(planned)*

- Precision and recall
- F1 score
- PR-AUC and ROC-AUC
- Confusion matrix
- Model interpretation

## Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook
- Git and GitHub

## Preliminary Findings

Initial descriptive analysis indicates that:

- Approximately **14.6%** of Canadian households reported dissatisfaction with housing affordability, using survey weights.
- Households in dwellings not owned by a household member reported higher dissatisfaction (20.8%) than households in member-owned dwellings (11.3%).
- British Columbia (21.8%) and Ontario (16.7%) showed relatively high estimated dissatisfaction rates.
- Dissatisfaction did not decrease consistently across higher household-income categories.

These are descriptive estimates. Statistical uncertainty and associations adjusted for other characteristics have not yet been fully evaluated.

## Limitations

- The survey is cross-sectional and cannot establish causal relationships.
- Housing satisfaction is self-reported.
- Geographic detail is limited by the public-use dataset.
- Survey weights and appropriate variance-estimation methods are necessary for population inference.
- Findings reflect the 2022 survey period.
- Machine learning predictions are intended for research and planning, not individual housing eligibility decisions.

## Reproducibility

The analysis is developed in Python using Jupyter Notebook.

Instructions for installing dependencies and running the complete analytical pipeline will be added as the project develops.

## Data Source and Acknowledgements

Statistics Canada — Canadian Housing Survey, 2022 Public Use Microdata File.

Official source: https://www150.statcan.gc.ca/n1/en/catalogue/46250001

This project is an independent academic analysis and is not an official Statistics Canada publication.

## Project Status

**In progress** — Data profiling and exploratory analysis are underway. Predictive modelling and final evaluation are planned.
