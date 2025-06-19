# Home Health Provider Segmentation

## Motivation

This project analyzes the Home Health Provider dataset to understand and segment providers based on services offered, performance metrics, cost efficiency, and quality ratings. The goal is to enable actionable insights for healthcare stakeholders, aiding in resource allocation, partnership decisions, and quality improvement efforts.

## Libraries Used

- pandas: for data loading and preprocessing
- numpy: for numerical operations
- scikit-learn: for clustering and segmentation
- matplotlib: for data visualization

## Files in this Repository

- `data/HH_Provider_Apr2025.csv`: The original dataset containing information about Home Health providers.
- `notebooks/exploratory_analysis.ipynb`: Jupyter notebook with data exploration and cleaning steps.
- `notebooks/segmentation_analysis.ipynb`: Notebook with clustering, profiling, and results.
- `results/segmentation_report.pdf`: Final report and visualizations of the segmentation analysis.

## Summary of Results

The segmentation revealed distinct groups of providers:

- High-performing, low-cost providers.
- Specialized service providers (e.g., therapy-focused, nursing-focused, etc.).
- Regional clusters with differing quality and cost profiles.

These results can support stakeholders in selecting providers for partnerships, identifying opportunities for quality improvement, and optimizing resource allocation.

## Acknowledgments and References

This project uses publicly available Home Health Provider data. Thanks to the Centers for Medicare & Medicaid Services (CMS) for providing this valuable dataset.

- [Home Health Care Agencies](https://data.cms.gov/provider-data/dataset/6jpm-sxkc)
