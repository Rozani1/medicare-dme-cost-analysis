# Report Folder

This folder contains documents and notebooks related to the analysis and reporting of Medicare Durable Medical Equipment (DME) data. The contents aim to document analytical approaches, highlight key insights, and support data-driven decision-making.

## File Descriptions

### Addressing Research Questions
Each notebook in this folder addresses a specific research question related to the Medicare Durable Medical Equipment (DME) data analysis.

### Notebooks

1. **Supervised Classification for Underserved Regions**
   - **Research Question**: Do certain regions consistently show higher supplier service volumes and Medicare payments, and are underserved areas disproportionately charged higher rates during specific periods, which could support targeted policy interventions? 
   - **Overview**: This Jupyter Notebook explores supervised classification techniques to identify and analyze underserved regions in the context of Medicare Durable Medical Equipment (DME) data. The analysis aims to uncover inefficiencies, optimize resource allocation, and inform targeted policy interventions.
   - **Objectives**:
     - Classify underserved regions based on supplier charges and service volumes.
     - Identify temporal and regional disparities in service distribution.
   - **Key Features**:
     - **Supervised Models**: Logistic Regression, Random Forest.
     - **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score, ROC-AUC, MCC, Brier Score.
     - **Time Series Analysis**: Investigating temporal trends in supplier charges and Medicare payments.
   - **Outputs**:
     - Visualizations of trends and relationships.
     - Classification performance metrics.
     - Insights into underserved regions and temporal patterns.

2. **Supplier Behavior Patterns Over Time**
   - **Research Question**: How do supplier service volumes and Medicare payments fluctuate over time, and which specific periods exhibit inefficiencies or potential fraud requiring targeted interventions? 
   - **Overview**: Analyzes trends in supplier behaviors, focusing on the geographic and temporal distribution of Medicare payments and supplier charges.
   - **Objectives**:
     - Identify patterns in supplier activity over time.
     - Highlight potential inefficiencies or anomalies in supplier practices.
   - **Key Features**:
     - **Unsupervised Models**: Isolation Forest (IF), Local Outlier Factor (LOF).
     - Longitudinal analysis of Medicare payment trends.
     - Visualization of regional disparities in DME services.
   - **Outputs**:
     - An HTML report summarizing supplier behavior patterns and key insights.
     - Graphics and tables depicting regional and temporal dynamics.

## Tools and Libraries

- **Python Version**: 3.9.13.
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn.

## Usage Notes

- The notebooks in this folder are intended for exploratory data analysis and report generation.
- Ensure that all dependencies are installed before executing the notebooks.
- Outputs, including HTML reports, provide summarized insights for quick reference.

## Contribution

If you have additional insights or improvements, feel free to submit updates or new resources to this folder.
