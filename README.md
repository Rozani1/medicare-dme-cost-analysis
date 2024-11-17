# Unveiling Temporal Disparities in Medicare DME: Machine Learning with Time-Series Cross-Validation for Cost Efficiency and Resource Allocation

## Overview

This project investigates temporal disparities in Medicare Durable Medical Equipment, Prosthetics, Orthotics, and Supplies (DMEPOS) to improve cost efficiency and resource allocation using machine learning and time-series cross-validation techniques.

## Project Goals

The project aims to:

1. Detect anomalies and inefficiencies in Medicare supplier behavior.
2. Identify underserved regions with high supplier charges and low service volumes.
3. Analyze long-term trends in DMEPOS billing practices and resource allocation.
4. Inform policy decisions to improve Medicare's cost efficiency and accessibility.

## Dataset

- **Source**: Medicare DMEPOS data (2014-2022)
- **Features**: Includes supplier charges, service volumes, and geographic variables.
- **Size**: 295,052 observations with 19 variables, processed for dimensionality reduction and analysis.

### Data Processing

- Missing values were handled systematically:
  - Geographic description rows (<0.02% missing) were removed.
  - "National" placeholder used for geographic codes with missing values.
  - Median imputation applied to missing beneficiary data (10-12% missing).
- Features were transformed using one-hot encoding and Principal Component Analysis (PCA) for dimensionality reduction.

### Data Splitting

- **Training set**: 2014-2020
- **Test set**: 2021-2022
- Time Series cross-validation was employed to preserve temporal order and prevent data leakage.

## Methodology

The project leverages the following approaches:

### Exploratory Data Analysis (EDA)

- Assessed data quality and distribution.
- Identified key features influencing supplier behavior.
- Conducted correlation analysis and PCA to uncover relationships and reduce dimensionality.

### Machine Learning Models

1. **Anomaly Detection**:

   - Isolation Forest
   - Local Outlier Factor (LOF)

2. **Classification**:

   - Logistic Regression
   - Random Forest

3. **Time-Series Forecasting**:

   - ARIMA
   - Prophet

### Key Innovations

- **Temporal Analysis**: Evaluating supplier behavior trends over nearly a decade.
- **Underserved Regions**: Defined as areas with supplier charges in the 95th percentile and service volumes in the 5th percentile.
- **Cost-Sensitive Learning**: Balancing detection trade-offs for efficiency.

## Tools and Technologies

- Programming: Python, R
- Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- Development: Jupyter Notebook, Google Colab
- Repository: [GitHub Project](https://github.com/Rozani1/medicare-dme-cost-analysis)

## Research Questions

1. How do supplier service volumes and Medicare payments fluctuate over time, and which specific periods exhibit inefficiencies or potential fraud requiring targeted interventions?
2. How do correlations between service volumes and supplier charges evolve over time, and what temporal patterns suggest inefficiencies or irregular relationships?
3. Do certain regions consistently show higher supplier service volumes and Medicare payments, and are underserved areas disproportionately charged higher rates during specific periods, which could support targeted policy interventions?
4. How have supplier charges varied by region over time, and how can these temporal trends help optimize costs?
5. What are the temporal trends in DME service distribution across geographic regions, and how can these trends identify underserved regions over time?

## Results and Findings

The findings contribute actionable insights to:

- Enhance Medicare's cost efficiency.
- Optimize resource allocation.
- Ensure equitable access to DMEPOS services.

## Repository Structure

```
├── README.md                            # Overview of the project and repository
├── Data Preparation/                    # Scripts and resources for preparing raw data
│   └── README.md                        # Explanation of the data preparation folder
├── Data/                                # Raw and processed data files
│   └── README.md                        # Explanation of the data folder
├── Report/                              # Project reports, including summaries and findings
│   └── README.md                        # Explanation of the report folder
├── Visuals/                             # Visualizations, charts, and related media
│   └── README.md                        # Explanation of the visuals folder
├── Literature Review/                   # Documents containing literature review and related descriptions
│   └── README.md                        # Explanation of the literature review folder
```

## Acknowledgments

- **Author**: Rozani Jeganathan
- **Supervisor**: Tamer Abdou, PhD
- **Institution**: The G. Raymond Chang School of Continuing Education, Toronto Metropolitan University

## License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).



