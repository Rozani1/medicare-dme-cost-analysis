## Research Question 2: Initial Results and Code Walkthrough

This section focuses on **Research Question 2**:

*"Do certain regions consistently show higher supplier service volumes and Medicare payments, and are underserved areas disproportionately charged higher rates during specific periods?"*

### Key Steps and Analyses:
1. **Models Trained**:
   - **Random Forest**: Chosen for its capability to capture complex relationships in the dataset.
   - **Logistic Regression**: Selected for its simplicity and interpretability.

2. **Analysis Criteria**:
   - **Effectiveness**: Assessed using metrics such as AUC, MCC, and Brier Score.
   - **Efficiency**: Evaluated based on fit time, score time, and memory usage.
   - **Stability**: Analyzed through cross-validation consistency.

3. **Specific Analyses Performed**:
   - **Regional Analysis**: Understanding geographic disparities in service volumes and payments.
   - **Temporal Analysis**: Examining changes over time in service volume and charges.
   - **Disproportionate Charges Analysis**: Investigating patterns in underserved areas.
   - **Mann-Whitney U Test**: Statistical test to compare distributions.

### Results and Conclusions:
- **Model Performance**:
  - Random Forest outperformed Logistic Regression in effectiveness and predictive power.
  - Logistic Regression was more efficient, with faster training and lower resource usage.
- **Insights**:
  - Underserved regions are rare but strongly associated with higher charges and lower service volumes.
  - Policies should target improving service availability and reducing costs in these areas.

### Summary:
The initial results show actionable insights that can inform policy decisions. The code is well-structured to ensure reproducibility and ease of interpretation.


