# HealthConnect – Week 7: Analytical Testing, KPI Validation & Dashboard Refinement

## Project Overview

This project focuses on testing and refining the HealthConnect healthcare analytics dashboard. The aim is to improve the accuracy, reliability, usability and interpretation of healthcare performance indicators by reviewing previously developed analytical outputs, validating KPI calculations and refining dashboard elements.

The work also identifies analytical limitations, highlights findings relevant to healthcare operations and provides recommendations for further improvement.

## Objectives

- Review previously developed analytical outputs.
- Validate key performance indicators (KPIs).
- Compare dashboard figures against underlying data.
- Review calculations, filters and date comparisons.
- Identify inconsistencies and potential analytical weaknesses.
- Improve dashboard presentation and interpretation.
- Refine business insights and recommendations.
- Document limitations and areas requiring further testing.

## Key Areas of Analysis

### 1. KPI Validation
Reviewed KPI calculations and their intended interpretation, including revenue performance and month-over-month comparisons.

The following DAX measures were used:

**Previous Month Revenue**
```dax
Previous Month Revenue =
CALCULATE(
    [Total Revenue],
    DATEADD('DateTable'[Date], -1, MONTH)
)
```

**Revenue Growth Rate**
```dax
Revenue Growth Rate =
DIVIDE(
    [Total Revenue] - [Previous Month Revenue],
    [Previous Month Revenue],
    BLANK()
)
```

These measures compare current-month revenue with the previous month's revenue to show the percentage increase or decrease.

### 2. Analytical Validation
Reviewed patient, appointment, clinical and financial findings to assess their consistency and business relevance. Particular attention was given to appointment distribution, emergency appointments, common diagnoses, hospital length of stay and revenue performance.

### 3. Dashboard Refinement
Improved revenue monitoring by introducing previous-month revenue comparisons and a month-over-month growth indicator. This provides additional context for interpreting financial performance instead of displaying current revenue in isolation.

### 4. Business Insights
The analysis highlighted patterns in patient distribution, appointment demand, common diagnoses, clinical service utilization and financial performance. These findings can support operational planning, resource allocation and management decision-making.

## Key Findings

- The previously reported dataset contained **20,000 registered patients**.
- The average patient age was **45.03 years**.
- A total of **14,929 patients** were recorded as having chronic diseases.
- Western Province recorded the highest reported patient count, with **4,091 patients**.
- Emergency appointments totalled **1,650** in the previously reported analysis.
- The average number of appointments per doctor was **14.29**.
- The previously reported average hospital length of stay was **5.49 days**.
- Gastritis, diabetes, hypertension, malaria and upper respiratory infections were among the most frequently recorded diagnoses.
- Revenue monitoring was refined to include month-over-month comparisons.


## Tools and Technologies

- **Power BI** – Dashboard development, KPI presentation and analytical reporting.
- **DAX** – KPI calculations and month-over-month revenue comparisons.
- **SQL** – Data querying and analytical validation, where applicable.
- **GitHub** – Project documentation and version control.

## Limitations and Areas for Further Testing

- Some KPI results require independent recalculation against the source dataset.
- Financial figures, including outstanding balances and insurance claims, require further reconciliation.
- Appointment attendance and no-show findings require additional validation across relevant segments.
- Filter behaviour and cross-page interactions should be tested using documented test cases.
- Findings should be reassessed when additional data or corrected records become available.

## Recommendations

1. Continue validating KPIs against the underlying healthcare records.
2. Investigate inconsistencies in financial and insurance-related figures.
3. Monitor appointment attendance and no-show patterns across facilities and patient groups.
4. Improve dashboard usability through clear labels, consistent formatting and meaningful comparisons.
5. Use validated findings to support operational and resource-allocation decisions.
6. Conduct further testing after each dashboard refinement.

## Conclusion

Week 7 focused on improving confidence in HealthConnect's analytical outputs and making dashboard information easier to interpret. The addition of month-over-month revenue comparison strengthened financial monitoring, while the review of existing findings identified areas requiring further validation. These improvements provide a foundation for more reliable healthcare analytics and continued dashboard development.
