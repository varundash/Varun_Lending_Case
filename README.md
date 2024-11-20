
# Loan Default Analysis Case Study
> Using Exploratory Data Analysis (EDA) to identify risky loan applicants and minimize credit loss.

## Table of Contents
* [General Information](#general-information)
* [Technologies Used](#technologies-used)
* [Approach and Methodology](#approach-and-methodology)
* [Key Findings and Insights](#key-findings-and-insights)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- **Objective**: Analyze loan data to identify patterns that indicate a borrower's likelihood to default. This insight helps financial institutions manage risk and reduce credit losses.
- **Business Problem**:
  - If a borrower defaults, the lender incurs financial loss.
  - If a loan is denied to a borrower who would repay, it results in loss of business.
- **Dataset**: Loan records from 2007 to 2011, containing details about loan amounts, borrower demographics, and statuses (e.g., "Fully Paid", "Charged Off").

## Technologies Used
- Python Libraries:
  - `pandas` for data processing.
  - `numpy` for numerical operations.
  - `matplotlib` and `seaborn` for visualization.
- Tools:
  - Jupyter Notebook for exploratory analysis.
  - Excel for data dictionary review.

## Approach and Methodology
1. **Data Cleaning**:
   - Columns with >50% missing values removed.
   - Irrelevant columns such as IDs and descriptions excluded.
   - Missing values in numeric columns filled with medians.

2. **Target Variable Creation**:
   - Defined a binary variable `default`:
     - `1` for "Charged Off" loans (defaulted loans).
     - `0` for "Fully Paid" loans.
   - Excluded "Current" loans since they aren't fully paid or defaulted.

3. **Univariate Analysis**:
   - Explored and visualized:
     - Loan status distribution.
     - Spread of interest rates.

4. **Bivariate Analysis**:
   - Analyzed relationships between:
     - Loan amount and default status.
     - Borrower annual income and default status.

5. **Visualization**:
   - Bar charts, boxplots, and histograms created for key variables.

## Key Findings and Insights
1. **Loan Status**:
   - Approximately 15% of loans are "Charged Off", indicating a high risk of default in this subset.
   - Most loans are "Fully Paid".

2. **Loan Amount**:
   - Higher loan amounts tend to correlate with a higher likelihood of default.
   - Defaulted loans show a wider variance in loan amounts compared to fully paid ones.

3. **Annual Income**:
   - Defaulted borrowers typically have lower annual incomes.
   - The income disparity is significant between fully paid and defaulted loans.

4. **Interest Rates**:
   - Riskier loans are associated with higher interest rates.
   - Fully paid loans have a more uniform interest rate distribution.

## Conclusions
- Borrowers with high loan amounts and low incomes are more likely to default.
- Lenders should focus on stringent evaluations for high-risk groups.
- Adjusting interest rates for riskier applicants can help mitigate credit losses.

## Acknowledgements
- This project leverages public loan datasets for educational and analytical purposes.
- Inspired by applications of risk analytics in finance.

## Contact
Created by [Varun Dubey] - feel free to contact for collaboration or queries.

