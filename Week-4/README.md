# FinTrust Digital Bank: Customer and Transaction Analytics

## Project Overview

This project was completed as part of the AnalystLab Africa Data Analytics Internship. It analysed customer behaviour, transaction performance, digital channel usage and risk review patterns using a synthetic digital banking dataset.

SQL was used for structured analysis, Python for exploratory data analysis and validation, and Power BI for interactive dashboard development.

## Objectives
* Analyse customer segments and engagement.
* Evaluate transaction volume, value and success rates.
* Compare transaction channels and transaction types.
* Explore monthly transaction trends.
* Investigate patterns in transactions flagged for risk review.
* Develop an interactive Power BI dashboard.
* Validate findings and recommend business actions.

## Tools Used

- SQL
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Jupyter Notebook
- Power BI
- Git and GitHub

## Dataset

The project used two synthetic datasets:

| Dataset | Records | Columns |
|---|---:|---:|
| Customers | 1,500 | 12 |
| Transactions | 12,000 | 11 |

The datasets contained customer information, transaction details, channels, transaction statuses and risk review indicators.

## Project Workflow

1. Data quality assessment and preparation.
2. SQL analysis of customers and transactions.
3. Exploratory data analysis using Python.
4. Validation of key findings.
5. Development and refinement of the Power BI dashboard.
6. Documentation of KPIs, business insights and recommendations.

## Key Findings

* Everyday was the largest customer segment, with 711 customers.
* Transfers recorded the highest transaction volume, with 3,549 transactions.
* The Mobile App recorded the highest transaction volume, with 5,102 transactions.
* The overall transaction success rate was approximately 90.47%.
* International transactions had a higher risk review rate than domestic transactions in the analysed dataset.
* SMEs had the highest average transaction value per active customer among the customer segments.

## Data Quality

The Customers dataset had no missing values. The Transactions dataset contained 96 missing `Device_Type` values and 96 missing `Location` values. No duplicate transaction records or unmatched customer IDs were identified during the initial checks.

The IQR method flagged 1,474 potential high-value outliers. These were treated as values for further investigation rather than automatic errors.

## Power BI Dashboard

The dashboard was designed to monitor:

* Customer KPIs
* Transaction KPIs
* Monthly transaction trends
* Customer segment performance
* Transaction channel performance
* Transaction status
* Risk review patterns

## Business Recommendations

* Investigate Mobile App transaction failures.
* Review the factors associated with international transaction risk flags.
* Monitor transaction types with higher risk review rates.
* Explore opportunities to improve SME customer services.
* Track transaction trends and maintain regular KPI validation.

## Limitations

The dataset was synthetic and may not reflect actual banking behaviour. Missing values and potential outliers were considered when interpreting the results. A risk review flag does not confirm fraud.

## Conclusion

The project demonstrated the use of SQL, Python and Power BI to transform structured data into insights for business performance monitoring and further investigation.


