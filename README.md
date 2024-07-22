# Life-expectancy-in-different-countries

# Multinomial Regression Model
This project focuses on building a multinomial regression model to predict life expectancy based on various features. The code uses the scikit-learn library in Python to implement the model.

## Project subject
The aim of this project is to predict the life expectancy of countries by examining health, financial and country indicators.
Life expectancy or average life expectancy is a statistical indicator that shows how long the members of a society live on average, or in other words, how long they are expected to live.

## Description
The code performs the following steps:
1. Reads the training data from a CSV file and preprocesses it.
2. Drops the 'Country' column as it may not contribute significantly to the prediction.
3. Handles missing values by filling them with the mean and median of each column.
4. Encodes the 'Status' column into numerical values (0 and 1) using LabelEncoder.
5. Normalizes the data using MinMaxScaler to scale the features.
6. Applies polynomial transformation to the features to capture non-linear relationships.
7. Trains a multinomial regression model.
8. Evaluates the model's performance using the R-squared score.

## Preprocessing
- Dropping the 'Country' column: Since country names are categorical and may not directly impact life expectancy, they are removed.
- Handling missing values: Missing values in numerical columns are filled with the mean and median of each respective column.
- Encoding categorical variable: The 'Status' column is converted into numerical values (0 and 1) using LabelEncoder.
- Normalizing data: MinMaxScaler is used to scale the features to a specific range, ensuring uniformity in feature magnitudes.
- Polynomial transformation: PolynomialFeatures is applied to create higher-order polynomial features for capturing complex relationships.

## Note
The code provided showcases a basic implementation of a multinomial regression model.