# Bank Customer Behaviour & Account Analysis

## Business problem
Explore a sample bank customer dataset to understand customer distribution, account types, employment categories, and mobile-banking activity. The analysis is descriptive and supports exploratory insights, not causal or predictive claims.

## Business questions
1. Which cities have the most customers?
2. How are customers distributed across account types, and how do average incomes and balances compare?
3. How does average monthly income vary by employment type?
4. How do mobile banking users and non-users compare in monthly transaction activity and average balance?

## Data cleaning
- Removed exact duplicate rows.
- Standardized city names by trimming spaces and title-casing.
- Replaced impossible ages (outside 18–100) with missing values, then imputed the median age.
- Imputed missing numeric income, tenure, and credit score values using their medians.
- Filled missing employment type with the mode.

## Derived columns
- `Age_Group`: grouped age ranges.
- `Income_Band`: income buckets.
- `Digital_Banking_Status`: readable label for mobile banking use.

## Project structure
- `data/raw/`: original CSV
- `data/processed/`: cleaned dataset and summary tables
- `notebooks/`: analysis notebook
- `images/`: generated charts

## Run
Open `notebooks/Bank_Customer_Analysis.ipynb` in Jupyter Notebook or VS Code. Ensure pandas, numpy, and matplotlib are installed. Run all cells from top to bottom.
