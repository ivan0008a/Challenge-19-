# Challenge-19-# Crypto Clustering Project

## Overview
This repository contains a Jupyter Notebook that performs clustering analysis on cryptocurrency market data. We use StandardScaler for normalization, K-means for clustering, and PCA for dimensionality reduction and optimization of clusters. Visualizations are created with hvPlot.

## Prerequisites
- Python 3.8+
- JupyterLab or Jupyter Notebook

Install dependencies via conda or pip:

```bash
pip install pandas numpy scikit-learn hvplot holoviews bokeh
```

## Usage
1. **Rename Notebook** (if not already):
   ```bash
   mv Crypto_Clustering_starter_code.ipynb Crypto_Clustering.ipynb
   ```
2. **Launch Notebook**:
   ```bash
   jupyter lab  # or jupyter notebook
   ```
3. **Run Cells** sequentially:
   - **Imports & Setup**: loads libraries
   - **Load Data**: reads `crypto_market_data.csv` into `df_market_data`
   - **Scaling**: normalizes features into `scaled_df`
   - **Elbow Method**: computes inertia vs. k and plots the Elbow Curve
   - **K-Means Clustering**: fits clusters on scaled features and visualizes
   - **PCA**: reduces to 3 components, notes explained variance
   - **Elbow Method (PCA)**: repeats K-means inertia plot on PCA data
   - **Clustering (PCA)**: fits K-means on PCA data and visualizes
   - **Comparison**: composite plots comparing raw vs PCA workflows

4. **Interpret Results**: follow Markdown cells in the notebook for Q&A prompts.

## Key Findings
- **Optimal k**: 4 clusters in both raw and PCA-reduced feature spaces.
- **Explained Variance**: PCA components explain ~89.5% of variance.
- **Impact of PCA**: PCA reduces noise, produces tighter, more interpretable clusters.

## Version Control
After confirming all cells run end-to-end, commit and push:

```bash
git add Crypto_Clustering.ipynb crypto_market_data.csv README.md
git commit -m "Add clustering notebook and README"
git push origin main
```

---
*Prepared by Alexander Ivanoff*

