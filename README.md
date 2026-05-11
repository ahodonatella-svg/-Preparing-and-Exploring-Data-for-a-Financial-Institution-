# Loan Default Risk Analysis | Data Preparation & EDA

## Executive Summary
A financial institution facing rising loan defaults sought to improve its 
approval process through data-driven decision-making. Using a dataset of 
32,000+ borrowers, this project identifies key predictors of loan default 
through data preparation and exploratory data analysis. Key findings reveal 
that loan grade, prior default history, interest rate, home ownership, and 
loan percent income are the strongest indicators of default risk, providing 
a foundation for predictive modeling in subsequent phases.

## Business Problem
Rising loan defaults are impacting a financial institution's profitability. 
The goal is to analyze historical loan data to identify which borrower 
characteristics and loan attributes most reliably predict default enabling 
more informed credit decisions and a refined loan approval process.

## Methodology
**Phase 1: Data Preparation**
- Loaded dataset using pandas; identified 165 duplicate records and removed them
- Explored structure: inspected data types, categorical vs. numerical fields, 
  and missing values
- Split data into training and testing sets for future modeling

**Phase 2: Exploratory Data Analysis (EDA)**
- Histograms to examine feature distributions — notable right skew in age, 
  income, and employment length
- Correlation heatmap — strongest relationship between person_age and 
  credit history length (0.88)
- Pair plots to detect multicollinearity
- Bivariate analysis comparing each feature against loan default status
- Binned continuous variables (e.g., age quartiles) to analyze default 
  patterns across groups

**Tools & Libraries:** Python, pandas, matplotlib, seaborn
