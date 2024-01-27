# Jamboree Graduate Admission Probability Analysis

## Context
Jamboree has been instrumental in aiding thousands of students secure admissions to top global colleges. Specializing in GMAT, GRE, and SAT preparations, they have now introduced a feature on their website for students to evaluate their chances of getting into IVY League colleges. This tool is particularly tailored for students from India, assessing their probability of graduate admission.

## Objective
The purpose of this analysis is to identify key factors influencing graduate admissions and understand their interrelationships. This will assist Jamboree in refining their admission probability estimation tool, thereby enabling accurate predictions for prospective students.

## Dataset
- **Download**: [jamboree_admission.csv] -- in the repo

### Column Profiling
- **Serial No.**: Unique row ID
- **GRE Scores**: Out of 340
- **TOEFL Scores**: Out of 120
- **University Rating**: Out of 5
- **SOP and LOR Strength**: Out of 5
- **Undergraduate GPA**: Out of 10
- **Research Experience**: 0 or 1
- **Chance of Admit**: Ranging from 0 to 1

## Methodology
1. **Exploratory Data Analysis (EDA)**
    - Import dataset and perform initial checks (structure, characteristics)
    - Drop the 'Serial No.' as it's a unique identifier
    - Utilize both graphical and non-graphical methods to analyze the data distribution and relationships

2. **Linear Regression Analysis**
    - Apply Linear Regression (using Statsmodel library)
    - Interpret and explain model results

3. **Testing Regression Assumptions**
    - Multicollinearity (VIF score)
    - Mean of residuals
    - Linearity of variables
    - Homoscedasticity test
    - Normality of residuals

4. **Model Evaluation**
    - Metrics: MAE, RMSE, R2 score, Adjusted R2
    - Comparative analysis of model performance on training and test data

5. **Actionable Insights & Recommendations**
    - Analysis of predictor variables' significance
    - Suggestions for model improvement and potential business applications

## Evaluation Criteria (100 Points)
1. **Define Problem Statement and EDA (10 points)**
    - Problem definition, data shape, types, summary
    - Univariate and Bivariate Analysis
    - Comments on data attributes, outliers, and distributions

2. **Data Preprocessing (10 Points)**
    - Duplicate, missing value treatment
    - Outlier treatment, Feature engineering
    - Data preparation for modeling

3. **Model Building (10 Points)**
    - Build and interpret Linear, Ridge, Lasso regression models
    - Display model coefficients with column names

4. **Testing Regression Assumptions (50 Points)**
    - Multicollinearity check by VIF score (variables are dropped one-by-one till none has VIF>5) (10 Points)
    - The mean of residuals is nearly zero (10 Points)
    - Linearity of variables (no pattern in the residual plot) (10 Points)
    - Test for Homoscedasticity (10 Points)
    - Normality of residuals (almost bell-shaped curve in residuals distribution, points in QQ plot are almost all on the line) (10 Points)

5. **Model Performance Evaluation (10 Points)**
    - Metrics: MAE, RMSE, R2, Adj R2
    - Train and test performance, model improvement needs

6. **Actionable Insights & Recommendations (10 Points)**
    - Comments on significance of predictor variables
    - Comments on additional data sources for model improvement, model implementation in real world, potential business benefits from improving the model (These          are key to differentiating a good and an excellent solution)

---
