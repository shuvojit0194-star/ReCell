# ReCell — Used Device Dynamic Pricing Model

Linear regression model predicting the resale price of used smartphones and tablets — enabling dynamic pricing for a used device marketplace.

## What It Does

1. Analyzes used device listings with specs (brand, RAM, storage, camera, battery, age)
2. Engineers features and validates multicollinearity using VIF
3. Trains a linear regression model to predict resale price
4. Identifies which device attributes drive the most price premium

## Key Price Drivers

- Device brand (Apple commands significant premium)
- RAM and storage capacity
- Normalized used price relative to new price
- Device age (release year)
- Camera megapixels, battery capacity

## Modeling Approach

- **VIF (Variance Inflation Factor)** analysis to detect and remove multicollinear features
- **Residual analysis** to validate linear regression assumptions
- **Feature scaling** for coefficient interpretability

## Tech Stack

- **Model:** Linear Regression (scikit-learn / statsmodels)
- **Validation:** VIF, residual plots, Q-Q plots, homoscedasticity checks
- **Libraries:** scikit-learn, statsmodels, Pandas, Matplotlib, Seaborn

## Files

| File | Description |
|---|---|
| `recell_pricing_model.ipynb` | Linear regression + VIF analysis + pricing model |
| `recell_supervised_ml_comparison.ipynb` | Extended comparison: Decision Tree, Random Forest, GBM, XGBoost on the same dataset |
| `used_device_data.csv` | Dataset |

## Business Application

Dynamic pricing in recommerce requires fast, accurate price estimates. This model provides a principled, interpretable pricing function that the business can trust and explain to sellers.

## Skills Demonstrated

Linear regression, multicollinearity detection (VIF), assumption validation, feature engineering, regression diagnostics, business-interpretable modeling
