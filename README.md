# Renewable Energy and Economic Growth in the United Kingdom

A data-driven study analysing the impact of renewable energy consumption on GDP growth in the United Kingdom (1990 onwards).

## Summary

This study examined the relationship between renewable and waste-based energy consumption and economic growth in the United Kingdom. The analyses showed that economic growth exhibited a fluctuating pattern and that the impact of renewable energy components was not linear. The Random Forest model provided more accurate predictions compared to Linear Regression and Gradient Boosting, and feature importance analysis within the model revealed that wind, solar and hydroelectric energy had a stronger impact on economic growth than other energy types. The study demonstrates that the energy–growth relationship is dynamic and that the impact of each energy type can vary; therefore, it is recommended that policymakers develop energy strategies by evaluating them on a type-by-type basis.

## Data

Yearly UK series from 1990, combined from energy and economic sources:

- Total energy consumption and renewable & waste energy share
- Breakdown by source: hydro, wind/wave/tidal, solar, landfill gas, sewage gas, biogas, municipal waste, wood, liquid biofuels and others
- Target: annual GDP growth (%)

## Approach

1. **Data integration and cleaning** of multi-source energy and economic data
2. **Exploratory analysis:** GDP growth and renewable energy trends over time, stacked area plot of energy types, correlation heatmap (geothermal removed as near-constant)
3. **Modelling:** train/test split with standard scaling; compared **Linear Regression**, **Random Forest** and **Gradient Boosting**, with cross-validation
4. **Evaluation:** MAE, RMSE and R²
5. **Interpretation:** model-based feature importance from the best model

## Files

| File | Description |
| :--- | :--- |
| `DamlaSuYayla_MLProject.ipynb` | Analysis and modelling notebook |
| `DamlaSuYayla_Data.csv` | Combined yearly dataset (semicolon-separated) |
| `DamlaSuYayla_Report.pdf` | Full project report |

## Tech stack

`Python` · `pandas` · `NumPy` · `scikit-learn` · `Matplotlib` · `Seaborn`
