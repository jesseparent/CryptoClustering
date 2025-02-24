# Crypto Clustering

## Project Overview

This project applies **K-means clustering** and **Principal Component Analysis (PCA)** to classify cryptocurrencies based on their price fluctuations over different timeframes. By analyzing price changes over **24 hours, 7 days, 30 days, 60 days, 200 days, and 1 year**, we aim to identify distinct clusters of cryptocurrencies that exhibit similar market behavior.

## Technologies Used

This project is implemented in a **Jupyter Notebook** and utilizes the following key Python libraries:

- `pandas` - For data manipulation and analysis
- `scikit-learn`:
  - `KMeans` - To perform clustering of cryptocurrencies
  - `PCA` - To reduce dimensionality and visualize clusters
  - `StandardScaler` - To normalize the dataset before clustering

## Installation & Setup

To run this project, follow these steps:

1. **Clone the repository** to your local machine:
   ```sh
   git clone https://github.com/jesseparent/CryptoClustering.git
   ```
2. **Download the dataset** from the repository and place it in the `Resources` folder.
3. **Install dependencies** using `pip`:
   ```sh
   pip install pandas scikit-learn jupyterlab matplotlib seaborn
   ```
4. **Open Jupyter Notebook** and run the cells:
   ```sh
   jupyter lab
   ```

## File Descriptions

- **`Crypto_Clustering.ipynb`** - The main Jupyter Notebook containing the data preprocessing, PCA transformation, K-means clustering, and visualization.
- **`Resources/crypto_market_data.csv`** - The dataset used for clustering, containing cryptocurrency price changes over different time periods.

## Methodology

1. **Data Preprocessing**:
   - Load cryptocurrency price data.
   - Normalize the dataset using `StandardScaler`.

2. **Dimensionality Reduction**:
   - Apply **PCA** to reduce the dataset to two principal components for visualization.

3. **Clustering with K-means**:
   - Use the **Elbow Method** to determine the optimal number of clusters.
   - Apply **K-means clustering** to group similar cryptocurrencies.

4. **Visualization & Analysis**:
   - Plot the clusters in a **2D PCA space**.
   - Analyze the characteristics of each cluster.

## How to Use

- Run all the cells in `Crypto_Clustering.ipynb` to execute the clustering analysis.
- Experiment with different numbers of clusters to see how cryptocurrency groupings change.
- Modify the PCA parameters to explore higher-dimensional clustering.



