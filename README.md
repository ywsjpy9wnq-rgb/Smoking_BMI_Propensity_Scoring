# Smoking Cessation & BMI Change

# Summary
Inverse probability weighting (IPW) was used to estimate the causal effect of smoking cessation on 5-year BMI change in 10,000 smokers. Quitting smoking was associated with a 3.2 percentage point increase in BMI (p < .001). Results were consistent across unadjusted, adjusted, and IPW models.

# Results

- Unadjusted: β = 2.40 (95% CI: 1.97 - 2.82), p < .001
- Adjusted (covariates): β = 3.27 (95% CI: 2.85 - 3.70), p < .001
- IPW (untruncated): β = 3.22 (95% CI: 2.73 - 3.70), p < .001
- IPW (truncated at 99th percentile): β = 3.25 (95% CI: 2.77 - 3.72), p < .001

Baseline characteristics:
- Total participants: 10,000
- Quit smoking: 1,998 (19.98%)
- Continued smoking: 8,002 (80.02%)

# Methods

Unadjusted and adjusted linear regression models were first fitted, with the adjusted model including age, sex, cigarettes per day, baseline BMI, cardiovascular disease, dementia, and diuretics as covariates. For causal inference, propensity scores were estimated using logistic regression with the same covariates. IPW weights were calculated as 1/PS for quitters and 1/(1-PS) for non-quitters. A survey-weighted linear regression was then fitted using these weights. As a sensitivity analysis, weights were truncated at the 99th percentile to assess the influence of extreme weights. An overlap plot was generated to assess the positivity assumption, which showed substantial overlap in propensity scores between groups with no scores at exactly 0 or 1.