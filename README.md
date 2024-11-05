# Google Play Store Data Analysis

## Overview
This notebook performs a comprehensive analysis of the Google Play Store dataset, focusing on data quality, exploratory data analysis, and visualization. The primary objective is to clean the data, understand the distributions of key variables, and identify trends in app ratings, categories, installs, and pricing.

## Dataset
The dataset used for this analysis is googleplaystore_dataanalysis.csv, which contains the following columns:

App: Name of the app
Category: Category of the app
Rating: Average user rating of the app
Reviews: Number of user reviews
Size: Size of the app
Installs: Number of installs
Type: Free or paid app
Price: Price of the app
Content Rating: Target audience (e.g., Everyone, Teen)
Genres: Genre of the app
Last Updated: Date when the app was last updated
Current Ver: Current version of the app
Android Ver: Minimum Android version required
Unnamed: 13, 14: Unused columns

## Data Quality
Missing Values: The dataset is checked for missing values across all columns. Notably, the Rating, Type, Content Rating, Current Ver, and Android Ver columns contain missing values.
Handling Missing Values:
The missing values in the Rating column are filled with the mean rating.
Rows with missing values in critical columns (Type, Content Rating, Current Ver, Android Ver) are dropped.
Data Type Conversion:
The Price and Installs columns are cleaned and converted to numeric types for analysis.
Outliers Analysis
The notebook includes a function to identify the minimum and maximum values in the Rating column and displays the five smallest and five largest ratings.

## Distribution Analysis and Descriptive Statistics
Descriptive Statistics: The mean, median, and mode of the Rating column are calculated.
Histogram Visualization: A histogram of app ratings is plotted to visualize the distribution.
Category Analysis
The number of apps per category is counted and displayed. A box plot is generated to show the distribution of ratings by category.

Top Installed Applications: 
The top ten most-installed applications are identified and displayed in a table.

Correlation Analysis: 
A correlation matrix is generated to explore the relationships between Price, Installs, and Rating. A heatmap visualizes these correlations.

Temporal Analysis: 
A temporal analysis of app updates is performed by extracting the year and month from the Last Updated column. A histogram displays the number of updates per year.

## Data Export
The cleaned dataset is exported to a new CSV file named cleaned_googleplaystore_data.csv.

## Dependencies
Make sure to install the following libraries if not already installed:

pandas
numpy
seaborn
matplotlib
You can install these libraries using pip:

pip install pandas numpy seaborn matplotlib
# PlayStore_Data_Analysis
