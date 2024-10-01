# Mammographic Density and Breast Cancer Risk

This repository contains the data and analysis scripts for a comparative study evaluating mammographic density as a predictor of breast cancer risk. This study compares the effectiveness of logistic regression and Random Forest machine learning models using data from the IBIS-I trial.

## Abstract

Breast cancer remains a principal cause of morbidity and mortality among women worldwide. Mammographic density (MD), alongside age and body mass index (BMI), is a significant risk factor for breast cancer. This repository details a case-control study that leverages data from the IBIS-I trial to explore the predictive power of mammographic density, age, and BMI on breast cancer risk, employing both logistic regression and Random Forest models to ascertain their predictive accuracies.

## Study Background

The analysis uses a subset of data from the International Breast Cancer Intervention Study I (IBIS-I), encompassing 7,154 women across 36 locations in 9 countries. Specifically, this study focuses on 1,065 participants for whom mammographic data were available to determine breast density and its correlation with breast cancer incidence.

### Key Findings

- **Logistic Regression**: Identified BMI and mammographic density as significant predictors, with a model accuracy of 58% and an AUC of 0.57.
- **Random Forest**: Showed higher overall accuracy at 88% but was initially biased towards predicting non-cancer cases. Sensitivity improved after threshold adjustments, capturing 47% of cancer cases with a corresponding increase in false positives.

## Data Description

The dataset includes the following variables:
- **Case**: Binary (1 = cancer, 0 = no cancer)
- **ARM**: Treatment assignment (2 = tamoxifen, 1 = placebo)
- **Age**: Age at the time of the first mammogram (continuous)
- **BMI**: Body Mass Index (continuous)
- **Breast Density**: Percentage of dense tissue in the mammogram (continuous)

## Repository Structure

- `/data`: This folder contains the datasets used in the analyses.
- `/notebooks`: Jupyter notebooks with detailed analysis, including exploratory data analysis and model comparisons.
- `/results`: Contains output from the models, including figures and tables summarizing the study's findings.

## Setup Instructions

To set up the project locally, follow these steps:

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Mammographic-Density-and-Breast-Cancer-Risk.git
