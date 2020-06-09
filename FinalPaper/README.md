# Gender and Racial Disparities in STEM Workforce:A Machine Learning Approach

## Abstract

While previous studies have elaborated on the persisting gender and racial gaps in STEM workforce engagement, there lacks consensus on the classification standards of STEM occupations. In an effort to clarify the boundary of STEM fields, we construct a feature-based machine learning classifier that learns from rich features of occupations and bottom-up responses from workers that indicate their STEM engagement. The classifier achieves 84\% accuracy on the test set and suggests that 7.6\% of occupations are mislabelled by the official STEM classification. Using the prediction of the feature-based classifier, we examine the gender and racial gaps in STEM workforce engagement in the US in 2018. While the regression coefficients suggest female and racial minorities are significantly underrepresented in the STEM workforce, we find the estimations based on the official STEM classification are prone to overestimate the disparities. We also find the disparities are heterogeneous across states in the US.

## Paper

- [paper/gender_racial_disparities_ml.pdf](paper/gender_racial_disparities_ml.pdf)

## Data

The datasets employed by this paper are accessible online.

- [Occupational Information Network (O*NET)](https://www.onetcenter.org/)
- [RAND American Life Panel](https://alpdata.rand.org/) (written request required by the authors.)
- [Detailed 2010 SOC occupations included in STEM (updated 2016)](https://www.onetonline.org/find/stem?t=0)
- [US Census American Community Survey 2018 Data](https://www.census.gov/programs-surveys/acs/data.html)
- [STEM classification result](data/clf_result.csv)
- [processed data for nation-level regressions](data/nation_reg_data.dta.zip)

## Code

- [notebooks/stem_classification.ipynb](notebooks/stem_classification.ipynb): preprocessing of the O*NET and the RAND ALP datasets, classification pipeline, hyperparameter tuning, and classification results.
- [notebooks/nation_level_reg.ipynb](notebooks/nation_level_reg.ipynb): nation-level regressions that identify gender and racial disparities in STEM workforce.
- [notebooks/state_level_reg.ipynb](notebooks/state_level_reg.ipynb): state-level regressions that identify gender disparities in STEM workforce.
