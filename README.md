# Zhou_Statistical_Critique_Presentation
A critical appraisal of statistical methods used in Zhou et al. (2020), highlighting limitations in model development, feature selection, and validation strategy.

# Risk Prediction or Risky Predictions?  
## A Critical Appraisal of Zhou et al. (2020)'s COVID-19 Severity Model

This repository contains a presentation evaluating the strengths and weaknesses of Zhou et al.’s (2020) prognostic model for predicting severe COVID-19 cases using clinical and comorbidity data from patients in Sichuan, China.

###  Project Summary

Zhou et al. developed a nomogram-based logistic regression model incorporating clinical symptoms and comorbidities to estimate a patient's risk of developing severe COVID-19. This presentation critically examines the methodological robustness, transparency, and reliability of the statistical approaches used in the study.


###  Key Topics Covered

- Study background and modelling strategy
- Variable selection using univariate screening, LASSO regression, and forward stepwise logistic regression
- Internal validation using bootstrapping and model performance metrics (C-index, AUC)
- Evaluation of model interpretability and generalisability
- Critique of sample size, geographic limitations, and data quality


###  Major Limitations Highlighted

- **Low Events Per Variable (EPV)**: Small number of severe cases (n=43) relative to predictors increases overfitting risk
- **Stepwise Regression After LASSO**: Undermines regularisation and can inflate coefficients
- **Lack of External Validation**: Limits generalisability beyond Sichuan province
- **Opaque Lambda Selection**: Lacks transparency in regularisation tuning
- **Non-standardised Data Collection**: Raises concerns about reproducibility and recall bias


###  Recommendations for Improvement

- Increase sample size and ensure sufficient EPV
- Use penalised regression without stepwise methods
- Perform external validation using independent datasets
- Apply transparent and reproducible feature selection strategies
- Standardise data collection and handle missing data systematically

  ## Reference: https://pmc.ncbi.nlm.nih.gov/articles/PMC7233581/
  
