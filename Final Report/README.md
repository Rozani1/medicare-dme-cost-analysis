# Temporal Disparities in U.S. Medicare DME Costs (2014–2022)

## Project Overview
This project explores disparities in Durable Medical Equipment (DME) spending in Medicare from 2014–2022. Using machine learning and time-series analysis, the study identifies inefficiencies, underserved regions, and opportunities for cost optimization.

## Objectives
- Analyze long-term billing trends in Medicare DME costs.
- Identify anomalies and inefficiencies in supplier behavior.
- Examine correlations between service volumes and charges over time.
- Investigate regional disparities in supplier charges.

## Data
- **Dataset Name**: Medicare Durable Medical Equipment, Devices & Supplies - by Geography and Service
- **Timeframe**: 2014–2022
- **Size**: 295,052 observations, 19 variables
- **Source**: [CMS Open Data Portal](https://data.cms.gov/)

## Methodology
- **Techniques**:
  - Anomaly Detection: Isolation Forest, LOF
  - Classification: Random Forest, Logistic Regression
  - Time-Series Forecasting: ARIMA, Prophet
- **Data Preprocessing**:
  - Addressed missing values (median imputation).
  - Applied dimensionality reduction using PCA.

## Key Findings
1. **Temporal Trends**: Significant anomalies detected in 2020, likely driven by COVID-19.
2. **Regional Disparities**: Underserved regions face higher costs despite lower service volumes.
3. **Inefficiencies**: Negative correlations between service volumes and supplier charges indicate systemic inefficiencies.

## Limitations
- Lack of labeled data for anomaly validation.
- Computational overhead in handling large datasets.
- Temporal seasonality and external factors affecting results.

## Future Directions
- Develop real-time anomaly detection systems.
- Incorporate advanced models like LSTM and GRU.
- Address data quality and scalability challenges.


## References
- Centers for Medicare & Medicaid Services (CMS). [Medicare Data](https://data.cms.gov/)






