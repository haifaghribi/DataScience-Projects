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
-




