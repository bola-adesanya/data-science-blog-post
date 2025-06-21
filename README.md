# Cost Efficiency Clustering for U.S. Home Health Agencies (2025)

This project explores how Medicare-certified home health agencies across the U.S. can be clustered based on cost efficiency and quality outcomes. Using CMS data from April 2025, we uncover hidden performance segments to support value-based care strategies.

## Project Motivation

Rising healthcare costs and inconsistent care quality challenge policymakers and payers. This project asks:
**Can home health agencies be segmented into meaningful efficiency profiles to optimize payment models and promote high-value care?**

## Dataset

- **Source:** CMS Home Health Provider Data (April 2025)
- **Fields Used:**
  - Medicare Cost Ratio (agency vs. national average)
  - Number of Episodes
  - Quality of Patient Care Star Rating
  - Risk-Standardized Rates:
    - Potentially Preventable Hospitalizations (PPH)
    - Discharge to Community (DTC)
    - Potentially Preventable Readmissions (PPR)

## Methods

- Preprocessing: Data cleaning, missing value handling, standardization
- Clustering: `KMeans` clustering (k=3), Elbow Method for optimal `k`
- Visualization: PCA for 2D cluster plotting, box plots, summary tables

## Results

Three efficiency clusters emerged:

| Label              | Characteristics                                  |
|-------------------|---------------------------------------------------|
| **Value Leaders** | Low cost, high quality, low readmission rates     |
| **Balanced**      | Average on cost and quality metrics               |
| **Inefficient**   | High cost, lower quality, poor clinical outcomes  |

These clusters can inform:

- Bundled payment model design
- Regional performance audits
- Targeted provider improvement initiatives

## Files in this Repository

- `data/HH_Provider_Apr2025.csv`: The original dataset containing information about Home Health providers.
- `data/HHS_Data_Dictionary.pdf`: Document that contains detailed information about the dataset.
- `notebooks/exploratory_data_analysis.ipynb`: Jupyter notebook with data exploration and cleaning steps.
- `notebooks/cost_efficiency_clustering.ipynb`: Notebook with clustering, results and recommendations.

## Use Case: Value-Based Care Optimization

This clustering supports stakeholders in identifying:

- Which agencies offer **"more care per dollar"**
- Where to **redirect funding or oversight**
- How to **prioritize technical assistance** and quality improvement

## Acknowledgments and References

This project uses publicly available Home Health Provider data. Thanks to the Centers for Medicare & Medicaid Services (CMS) for providing this valuable dataset.

- [Home Health Care Agencies](https://data.cms.gov/provider-data/dataset/6jpm-sxkc)
