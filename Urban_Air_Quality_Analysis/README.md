# Details of my work

# Data Collection and Preprocessing
I collected all the data form the provided sources, merge them, then started working dta preprocessing.
I cleaned each data set seperatly: Air_Data, Weather_Data, Transport_Data
for each data set I  : 
- looked for structure,
- Provide a basic statistical summary of the dataset
- missing values,
- handle missing values by fill in in the missing values with the mean value of each column
- Plot boxplots to visually inspect outliers
- create a function to  remove outliers
Later I merged all the datasets based on location and timestamp and create a unified dataset with consistent formatting called Unified_Data.csv

# Exploratory Data Analysis (EDA): 
I followed all the given instructions and I :
- Perform univariate analysis on each feature
- Perform univariate analysis on each feature, plot histograms for specified columns
- Conduct bivariate analysis to explore relationships between variables by ploting 
- Create time series plots for pollutants and weather variables. and plot it
- Generate heatmaps for spatial distribution of pollutants
- Use advanced visualization libraries for interactive dashboards, I created interactive plots
- Perform statistical tests to identify significant relationships : I used Correlation matrix, and T-test between high and low pollutant levels for each weather variable

# Feature Engineering: 
- Convert Date to datetime format
- create time-based features (hour, day, month, season).
- Develop lag features for time series data.
1-Day Lag: Short-term, immediate past influence.
7-Day Lag: Weekly patterns.
30-Day Lag: Monthly trends or seasonality
- Calculate rolling averages over different time windows
7-day rolling average for a feature will be the average of the feature values over the past 7 days
- Generate interaction features between variables:
High humidity might lead to the accumulation of PM2.5
interaction between NO2 and wind speed helps in improvemt air quality
Temperature influences CO levels
- Create domain-specific aggregations: traffic Density Index based on the miles and trips data for urban, suburban, and rural areas.
then I combined all of them 
- Implement feature selection techniques:
PM2.5 as the target because it is a commonly monitored air pollutant with well-defined health impact categories
Used Random Forest Regressor for Feature Importance
Selected top features (top 10)

# Unsupervised Learning:
- Implement K-means and hierarchical clustering for pollution hotspots and checked optimal clusters number by Silhouette Score Analysis and dendrogram
- Visualize the clusters using a pairplot
- Use DBSCAN for density-based clustering and plot
- Apply PCA and t-SNE for dimensionality reduction
here I visualized all the cluster techniques

#  Supervised Learning - Multi-class Classification:
- Prepare dataset by binning air quality levels into categories
- Split data 
- Implement and comparethe provided  Models
I creade afunction to find accuracy,Precision,Recall, F1, ROC AUC, and confusion matrix for each model
the used models: - Random Forest - XGBoost - Support Vector Machines - Neural Networks
- Perform hyperparameter tuning and cross-validation for each model
- Evaluate using accuracy, F1-score, and confusion matrices (XGBOOST was the best model)
- visualize each confusion matrix










