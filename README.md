\# CostlyCar - Vehicle Repair Cost Prediction



Machine Learning project to predict the annual repair cost of vehicles, helping insurers and fleet managers anticipate maintenance expenses and avoid financial surprises.



\## Objective



Model the relationship between key vehicle characteristics (age, usage, mileage, engine type) and annual repair expenses, in order to:

\- Estimate the annual cost of a vehicle not yet insured

\- Optimize pricing or maintenance budget planning

\- Better anticipate financial risk in auto insurance and fleet management



\## Problem Statement



Annual vehicle repair costs are difficult to estimate in advance. Poor estimation can lead to:

\- Financial losses for insurers

\- Unfair pricing

\- Unexpected expenses for drivers



\## Dataset



\- \*\*Target\*\*: `Annual\_Repair\_Cost` (regression)

\- \*\*Numerical features\*\*: `Vehicle\_Age\_Yrs`, `Engine\_Displacement\_L`, `Avg\_Daily\_Mileage`

\- \*\*Categorical features\*\*: `Modified\_Flag`, `Service\_Geo\_Index`

\- \*\*Size\*\*: 1,000 vehicles



\## Methodology (CRISP-DM)



1\. Business understanding

2\. Data understanding (univariate \& multivariate analysis, correlation study)

3\. Data preparation (missing values, encoding, normalization, PCA)

4\. Modeling \& evaluation

5\. Deployment



\## Key Findings



\- Strong correlation (0.74) between \*\*vehicle age\*\* and \*\*annual repair cost\*\*

\- `Avg\_Daily\_Mileage` shows a strong right-skewed distribution with outliers

\- Positive relationship between mileage, engine displacement and repair cost



\## Models



\### Regression (Annual Repair Cost prediction)



| Model | Technique | R² (Test) | RMSE ($) | MAE ($) |

|---|---|---|---|---|

| Linear Regression | Linear (baseline) | 0.6865 | 381.02 | 307.86 |

| Polynomial Regression (degree 2) | Linear + interactions | 0.6875 | 380.45 | 305.36 |

| Decision Tree Regressor | Tree | 0.2569 | 586.66 | 453.61 |

| XGBoost (optimized) | Boosting | 0.5272 | 467.93 | 357.54 |

| SVR | Non-linear (RBF kernel) | 0.5518 | 455.62 | 342.74 |

| \*\*Random Forest\*\* | \*\*Bagging (ensemble)\*\* | \*\*0.709 (Champion)\*\* | - | - |



\### Classification (Vehicle Age Category prediction)



| Model | Metric | Score |

|---|---|---|

| SVM (SVC) | Accuracy | 0.90 |



\## Technologies



\- Python

\- Pandas, NumPy

\- Scikit-learn

\- Matplotlib / Seaborn

\- Jupyter Notebook



\## Deployment



An interactive prototype allows users to input vehicle characteristics (age, engine size, daily mileage) and get a real-time estimated annual repair cost.



Possible applications:

\- Web or desktop application integration

\- Decision-support dashboard

\- Vehicle comparison tool

\- Budget planning assistant



\## Conclusion



This project demonstrates the value of Machine Learning in predicting automotive repair costs, enabling better expense anticipation and data-driven decision making.



\*\*Future improvements:\*\*

\- Add more data (maintenance history, usage type)

\- Test more advanced models

\- Improve prediction accuracy

