# Unsupervised-Learning-Project

## Project/Goals
The main objectives of this project are as follows:

- Utilize unsupervised learning techniques to discover patterns and structures within the dataset without explicit labels.
-  Conduct exploratory data analysis (EDA) to gain insights into the underlying distribution and relationships between variables.
-  Evaluate the effectiveness of different clustering algorithms in grouping similar points of a feature. 

## Process

### Step 1: Data Collection
Loaded the "Wholesale_Data" file from the Kaggle into a DataFrame for further analysis.

### Step 2: Exploratory Data Analysis and Pre-processing

#### A) Analyzed and visualized relationships between variables:
- Performed EDA to understand the distribution, relationships and correlation analysis between the variables using techniques such as scatter plots, histograms and heatcharts.

#### B) Handled missing values and outliers:
- Identified and addressed outliers in the dataset to ensure data quality and reliability.
- Transformed the data using square-root as we did not want to drop any values.

#### C) Data Transformation and Feature Selection:
- Using MinMaxScaler we transformed the data using normalization instead of standardizing since our data is not normally distributed.
- Identified the most important features using PCA in the pre-processing portion of the project. 

### Step 3: Clustering 

#### KMeans Clustering
- Used the elbow method to determine the optimal number of clusters.
- Used KMeans to plot the clusters in a central point called centroids.

#### Hierarchical Clustering
- Plotted a dendrogram to visualize the hierarchical clustering and deducted that there were three clusters after analyzing. 

#### PCA 
- Used dimensionality reduction technique to improve clustering performance.

## Results
Results
1. The analysis using K-means and Hierarchical Clustering revealed three distinct customer segments based on their annual spending across different product categories:

  a. Cluster 1: Represents customers who exhibit moderate spending on all products, potentially indicating medium-sized establishments with a balanced product inventory.
  
  b. Cluster 2: Represents customers with relatively lower spending across all categories, suggesting a segment of budget-conscious individuals prioritizing essential items.
  
  c. Cluster 3: Represents customers with higher spending in different categories, possibly indicating larger businesses such as restaurants or supermarkets.

2. Furthermore, significant correlations between certain pairs of features were observed, shedding light on potential patterns in customer purchasing behaviors:

  a. There is a strong positive correlation between Grocery and Detergents_Paper spending, implying that customers who spend more on groceries also tend to spend more on detergents and paper products.
  
  b. Similarly, there is a strong positive correlation between Grocery and Milk spending, suggesting that customers who spend a lot on groceries tend to include milk in their purchases.
  
  c. Conversely, there is a negative correlation between Fresh and Frozen spending, indicating that customers who spend more on fresh products might spend less on frozen items.

3. Insights from Principal Component Analysis (PCA) highlighted the following:

The first principal component is heavily weighted by spending on Milk, Grocery, and Detergent_Paper, suggesting that these categories are correlated and contribute significantly to customer variance.

4. Based on these findings, tailored marketing strategies can be recommended for each customer segment to enhance sales in various product categories, thus maximizing business profitability.

## Future Goals
If given more time to work on this project, the following future goals could be pursued:

- Explore alternative algorithms and techniques for clustering customer purchasing behaviours. 
- Perform hyperparameter tuning to help with model performance. 
