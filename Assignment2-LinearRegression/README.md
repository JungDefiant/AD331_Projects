## Assignment: Linear Regression, Data Cleaning, and Feature Engineering
Written by Bade Habib

### Description Of Dataset
Dataset used is data of housing built in King County, last updated between 2014-2015.
The data describes

The **target variable** is the **price** of housing, which is compared to the following variables.
- Age of the house (calculated as a feature).
- Whether the house is located on a waterfront.
- How many bedrooms are in the house.
- How many bathrooms are in the house.
- The square footage of living area in the house.

### Data Cleaning & Feature Engineering
The following steps were completed as a part of data cleaning and feature engineering.

## Data Cleaning
1. Removed rows with missing values using *dropna*.
2. Calculated the Z-Score of the data, which is a measure of how far a point deviates from the mean.
3. Allocated the indices of the outliers in the data array, where an element's z-score exceeds a threshold of 2.
4. Removed every row in the data set matching the indices of the outliers.

## Feature Engineering
Calculated age by performing a lambda function, which subtracts the *year built* variable by the current year (2025).

### Final Evaluation Metrics
**MSE:** 156954.15063322696
**R2:** 0.5475104477421255
