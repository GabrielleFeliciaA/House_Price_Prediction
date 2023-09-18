# House Price Prediction using Linear Regression Algorithm

## Introduction
Predict and determine the factors that affect the price of a home in the King County region of the USA. The information utilised relates to home prices in King County, USA, in 2015. The following URL: https://www.kaggle.com/code/burhanykiyakoglu/predicting-house-prices/notebook was used to access this data on the Kaggle website.

## Exploratory Data Analysis
Several steps were taken to explore this data, including importing files, examining at the data's type, statistical distribution, and checking for missing values. The next step is to do an anomaly check (searching for outliers in the home price variable). Last but not least, we also depict the correlations between variables and discover data patterns.

## Data Processing
First, the correlation between variables is examined at the data processing step. At that point, a number of factors were eliminated since they did not strongly relate to or correlate with the dependent variable, in this case, the variable known as `price`. The second step is to do a linearity check, which involves determining whether pairs of variables have a linear relationship. The third step involves doing a normality check to determine which variables are normally distributed.

## Modelling
A model is developed using linear regression techniques to predict house prices. At this stage, 3 models have been created, and the third model (called `model3`) is determined to be the best model, namely the model that has the best ability to forecast house price. Model 3 is then used to estimate house prices using the test data after the data has been splitted into training and test sets.

## Model Evaluation & Results
The best model (`model 3`) produces an accuracy of 79.2%. The model equation is: `log(price) = -5.932e+01 + sqft_living*(2.163e-04) + view*(8.791e-02) + lat(1.488e+00) + waterfront*(3.772e-01) + grade*(1.497e-01)`. Furthermore, `Model 3` produces a residual standard error value of 0.2746, an adjusted R-squared value of 0.7282, an F-statistic value of 11580 and a p value of <2e-16.

In summary, the square footage of the living room, the presence of a view, the latitude coordinate, the presence of a waterfront, and the house's grade all affect how much a house prices in King County. The explanation is as follows:
- The predicted price will rise for every additional square foot of living space in a home.
- Another factor that affects a home's pricing is the view it has. Particularly, those with views rated at levels 3 and 4 are more expensive than those with views rated at levels 0, 1, or 2.
- The price of a house increases with the grade of the home.
- those with a waterfront are more expensive to buy than those without one.
- Along the latitude, the cost of the dwellings rises from south to north.
