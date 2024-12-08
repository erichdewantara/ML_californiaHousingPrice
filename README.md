# CALIFORNIA HOUSING PRICE PREDICTION
This work contains dataset information from the 1990 California sensus sourced originally from the article written by R. Kelley Pace and Ronald Barry for [Statistics & Probability Letters, Vol. 33, 1997](https://www.sciencedirect.com/science/article/abs/pii/S016771529600140X).

## Context
Housing is a primary necessity, but not everyone knows the exact price of a house that matches the features offered. If a developer sets a price too low compared to their competitors, the house may sell quickly but the profit will not be optimal. Conversely, if the price is too high, the house may be difficult to sell due to low buyer interest, and preferences may shift to other similar, more affordable houses.

## Problem Statement
The challenge for developers is determining the right house price based on the location and features offered, while remaining competitive with competitors selling similar types of house. Developers certainly do not want to sell houses at unreasonable prices, taking into account features such as the number of rooms, location, and condition of the house.

## Goals
Modeling is necessary to determine accurate house prices using Machine Learning algorithms by analyzing which features influence house prices in California.

## Conclusion
Based on the model, the following insights can be drawn:
1. The most influential feature on median_house_value is op_inland, which represents the category of the ocean_proximity location. Additionally, median_income and distance_to_sf also have high influence on the model.
2. According to the feature correlation:
   - op_inland is negatively correlated with the target median_house_value, meaning that houses located inland (away from the coast) are predicted to have lower prices.
   - median_income is positively correlated with the target, meaning that as the income of residents increases, house prices are expected to rise.
   - distance_to_sf is negatively correlated with the target, indicating that as the distance to San Francisco increases, house prices tend to decrease, though not significantly.
3. The evaluation metrics used for the model are R-Squared, MAE, RMSE, and MAPE:
   - R-Squared: The model has a good ability to explain 75.5% of the variation in the target data.
   - MAE: The average absolute difference between predicted and actual values is 33,247.99.
   - RMSE: The model shows outliers in predictions, as the RMSE value is higher than the MAE, at 48,126.31.
   - MAPE: The average percentage of absolute error between predictions and actual values is 20.26%.
4. The model for predicting house prices in California has limitations and is only recommended for use within the range of minimum and maximum values for each feature and target.

## Recommendation
Here are some suggestions that may be useful for developing a better model:
1. Add potential features that could influence house prices, such as land and building area, house type, number of floors, or building condition. External features may also have an impact, such as house taxes or proximity to important facilities (e.g., public transportation, hospitals, shopping centers).
2. Update the data with more current information to improve prediction accuracy, considering that the data used in the model is from the 1990 census, which may no longer be relevant to the current conditions.
3. Experiment with other feature engineering techniques, such as binning the features housing_median_age, population, households, or median_income, as the range of data allows for categorization.
4. Experiment with other modeling algorithms that have not been tested in this study.
