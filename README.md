Certainly! Here's a README that you can use for your GitHub repository. I've kept it concise, as you requested, while covering the main points of the project:

# Azerbaijan Hotel Industry Financial Analysis and Revenue Prediction

## Project Overview

This project provides a comprehensive analysis of the Azerbaijan hotel industry's financial performance from 2001 to 2024. It delves into revenue streams, expense categories, profitability trends, and leverages machine learning to forecast future total revenue.

## Data

The dataset, `mehmanxana-hotel-v-mehmanxana-tipli-obyektlrin-glir-v-xrclri-dt_bo_012.csv`, contains financial metrics (in thousands of AZN) including:
- **Revenue:** Total Revenue, Room Sales, Food Services, Health Services, Other Revenue.
- **Expenses:** Total Expenses, Fuel & Energy, Food & Beverage, Salaries, Water, Rent, Taxes, Maintenance, Other Expenses.

## Analysis & Key Findings

1.  **Data Preprocessing:** Cleaned the raw data, including renaming columns to English, handling missing values (replacing '-' with NaN), and converting relevant columns to numeric types.
2.  **Exploratory Data Analysis (EDA):**
    *   Calculated descriptive statistics for key financial indicators (Revenue, Expenses, Profit, Profit Margin).
    *   Analyzed correlations, observing strong positive correlations between Total Revenue and core revenue streams/most expenses.
    *   Visualized financial trends over time, highlighting overall growth, the significant dip in 2020 (likely due to COVID-19), and a strong recovery post-2020.
    *   Examined the revenue structure for the latest year (2024) via a pie chart, showing Room Sales as the dominant contributor.
    *   Illustrated year-over-year trends for individual revenue and expense categories.
3.  **Machine Learning for Revenue Prediction:**
    *   Evaluated several regression models (Linear Regression, Ridge, Lasso, Random Forest, Gradient Boosting) to predict `Total_Revenue` based on `Year`.
    *   **Gradient Boosting Regressor** emerged as the best model for fitting historical data, explaining almost 90% of the variance (R2 score: 0.896).
    *   For future revenue extrapolation (2025-2030), a **Linear Regression model combined with Polynomial Features (degree 2)** was employed. This approach proved effective in predicting a continuous, increasing trend into the future, overcoming the extrapolation limitations of tree-based models.

## Future Revenue Predictions (2025-2030)

The project provides a forecast for total revenue, demonstrating a projected growth based on historical trends. This prediction is visualized alongside the historical data.

## Technologies Used

*   Python
*   Pandas (for data manipulation)
*   Numpy (for numerical operations)
*   Matplotlib (for visualizations)
*   Seaborn (for enhanced visualizations)
*   Scikit-learn (for machine learning models: LinearRegression, Ridge, Lasso, RandomForestRegressor, GradientBoostingRegressor, PolynomialFeatures)

Feel free to explore the notebook for detailed steps and code.
