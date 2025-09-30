# Customer-Segmentation-using-PCA-and-K-means

Customer Segmentation using K-Means & PCA

This project demonstrates how to perform customer segmentation using K-Means clustering and Principal Component Analysis (PCA) for dimensionality reduction.
The analysis is performed on a synthetic dataset (segmentation data.csv) containing demographic and socioeconomic information.

Project Overview

The main objective of this project is to:
- Explore and analyze customer demographic and socioeconomic data.
- Identify natural groupings (clusters) within the dataset using K-Means clustering.
- Reduce dimensionality with PCA to visualize and interpret clusters effectively.
- Provide actionable customer segments (e.g., Well-off, Career Focused, Standard, Fewer Opportunities).

Dataset

The dataset (segmentation data.csv) contains 2000 customers, with the following features:
- Sex (0 = Female, 1 = Male)
- Marital Status (0 = Single, 1 = Married)
- Age (18–76 years)
- Education (0 = None, 1 = Graduate, 2 = Postgraduate, 3 = PhD)
- Income (annual income in local currency)
- Occupation (0 = Unemployed, 1 = Employee, 2 = Self-employed)
- Settlement Size (0 = Small, 1 = Mid-size, 2 = Large city)

Methodology

1. Exploratory Data Analysis (EDA)
- Descriptive statistics (.describe())
- Correlation analysis with a heatmap
- Scatter plots for relationships (Age vs. Income)

2. Data Preprocessing
- Standardization using StandardScaler (ensures equal weight to all features).

3. Clustering with K-Means
- Used Elbow Method (WCSS) to determine the optimal number of clusters.
- Final model: 4 clusters.
- Added cluster labels to the dataset for interpretation.

4. Dimensionality Reduction with PCA
- PCA applied to standardized features.
- Selected 3 components, explaining ~81% of variance.
- Visualized clusters in reduced dimensions.

5. Cluster Profiling
- Clusters were analyzed and labeled as:
- Well-off
- Career Focused
- Standard
- Fewer Opportunities

Visualizations

- Correlation Heatmap of features
- Elbow Plot for optimal cluster selection
- Scatter Plot of clusters (Age vs. Income)
- PCA Component Heatmap showing feature loadings
- Clusters plotted on PCA components

Technologies Used

- Python
- NumPy & Pandas → Data manipulation
- Matplotlib & Seaborn → Data visualization
- Scikit-learn → Preprocessing, K-Means, PCA
- SciPy → Hierarchical clustering (optional exploration)
- Pickle → Model persistence

🚀 How to Run

Clone the repository:
```
git clone https://github.com/your-username/customer-segmentation-kmeans-pca.git
cd customer-segmentation-kmeans-pca
```


Install dependencies:
```
pip install -r requirements.txt
```

Open Jupyter Notebook / Colab and run the notebook:
```
jupyter notebook
```

Load the dataset segmentation data.csv and execute all cells.

Results

- The K-Means + PCA approach successfully segmented customers into 4 distinct clusters:

Segment	Key Characteristics
- Well-off -->	Older, higher income, large settlement size
- Career Focused -->	Middle-aged, highly educated, urban professionals
- Standard	Younger --> mid-income, balanced profile
- Fewer Opportunities -->	Lower income, smaller settlements, limited education

Future Improvements

- Use hierarchical clustering for comparison.
- Experiment with DBSCAN and Gaussian Mixture Models.
- Deploy as a web dashboard using Streamlit or Flask.
- Apply to real-world marketing datasets for actionable insights.

License
This project is licensed under the MIT License – feel free to use, modify, and distribute.

✨ Author: Dheeraj Kumar
