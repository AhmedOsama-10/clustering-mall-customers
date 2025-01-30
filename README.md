# Customer Segmentation using K-Means Clustering

## Overview
This project focuses on customer segmentation using the K-Means clustering algorithm. The dataset used is the "Mall_Customers.csv" file, which contains information about customers, including their age, annual income, spending score, and gender. The goal is to segment customers into different groups based on their spending behavior and demographic information.

## Dataset
The dataset contains the following columns:
- **CustomerID**: Unique identifier for each customer.
- **Gender**: Gender of the customer (Male/Female).
- **Age**: Age of the customer.
- **Annual Income (k$)**: Annual income of the customer in thousands of dollars.
- **Spending Score (1-100)**: Score assigned by the mall based on customer behavior and spending nature.

## Project Steps
1. **Data Loading and Inspection**:
   - The dataset is loaded using pandas.
   - Basic information about the dataset is inspected using `data.info()` and `data.describe()`.

2. **Data Preprocessing**:
   - The `CustomerID` column is dropped as it is not relevant for clustering.
   - The `Gender` column is converted into a binary format using one-hot encoding.
   - Outliers in the `Annual Income (k$)` column are handled by replacing them with the mean value.

3. **Exploratory Data Analysis (EDA)**:
   - Box plots are used to visualize the distribution of numerical features.
   - Outliers are identified and handled to ensure the data is suitable for clustering.

4. **K-Means Clustering**:
   - The K-Means algorithm is applied to the dataset to segment customers into clusters.
   - The optimal number of clusters is determined using the silhouette score, which measures the quality of the clusters.

5. **Visualization**:
   - The results of the clustering are visualized to understand the distribution of customers across different segments.

## Key Findings
- The optimal number of clusters for this dataset is 6, as determined by the silhouette score.
- The clustering results provide insights into customer segments based on their spending behavior and demographic information.

## Requirements
To run this project, you need the following Python libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

You can install these libraries using pip:
pip install pandas numpy scikit-learn matplotlib seaborn


## Conclusion
This project demonstrates how to use K-Means clustering to segment customers based on their spending behavior and demographic information. The insights gained from this analysis can help businesses tailor their marketing strategies to different customer segments, ultimately improving customer satisfaction and increasing revenue.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
