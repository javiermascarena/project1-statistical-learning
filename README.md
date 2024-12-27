# Football Players Analysis 2022-2023

This repository contains the analysis of football players from the Top 5 European leagues during the 2022-2023 season. The project uses unsupervised learning techniques to identify standout players, discover hidden talent, and analyze key player statistics.

## Project Objective

The primary goal of this project is to:

- Identify the best players of the season.
- Highlight lesser-known players who exceeded expectations.
- Uncover valuable insights and statistics about player performance.

## Datasets

- **Top 5 European Leagues Player Stats 2022-2023**: Includes player statistics for various positions. ([Kaggle dataset link](https://www.kaggle.com/datasets/ameyaranade/big-5-european-leagues-player-stats-2022-23))
- **FIFA 23 Official Dataset**: Adds information about market value and salaries. ([Kaggle dataset link](https://www.kaggle.com/datasets/kevwesophia/fifa23-official-datasetclean-data))

### Data Preprocessing

1. **Variable Reduction**: Irrelevant or redundant variables were removed.
2. **Dataset Merging**: Combined datasets using inner joins and adjusted missing values.
3. **Deduplication**: Addressed duplicate entries caused by mid-season transfers.
4. **Imputation**: Replaced missing numeric values with column means.
5. **Player Filtering**: Removed players with limited playing time.

## Methods and Techniques

### Principal Component Analysis (PCA)
- Reduced dimensionality from 57 numeric variables to 7 principal components, capturing 85.34% of the variance.
- Components highlight characteristics such as offensive midfielders and goalkeepers.

### Factor Analysis
- Extracted 8 factors explaining 85% of data variability.
- Identified hidden insights, e.g., defensive players, forwards, and play-makers.

### Clustering
- **K-Means**: Clustered players into 5 categories (e.g., goalkeepers, forwards).
- **K-Medoids**: Added stability with a similar result to K-Means.
- **Kernel K-Means**: Explored non-linear relationships; results aligned with previous methods.
- **Hierarchical Clustering**: Utilized Euclidean distance and single linkage for detailed heatmaps.
- **Expectation-Maximization (EM)**: Explored Gaussian distribution clustering but found it less effective for this dataset.

## Results and Insights

- PCA and FA revealed meaningful patterns and reduced dimensionality effectively.
- Clustering techniques provided stable groupings for player types.
- Highlighted exceptional players like Bruno Fernandes and David Raya.
- Explored player roles, contributions, and performance metrics in detail.

## Conclusion

This project integrates unsupervised learning techniques to uncover valuable insights about football players. Beyond statistical analysis, it emphasizes understanding the underlying algorithms and decision-making processes.

## Authors

- Álvaro del Cañizo Angurel
- Javier Mascareña González
