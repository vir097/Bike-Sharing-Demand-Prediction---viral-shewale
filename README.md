# Bike-Sharing-Demand-Prediction

## Abstract: 
The project aims to build an ML model that can predict the demand for rental bikes in the city of Seoul. The dataset contains different attributes and the number of bikes rented each hour for 12 months.


## Problem Statment:
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

## EDA Summary:
* The demand for rental bikes was highest in the summer season and lowest in the winter season.

* May-July are peak months to rent a bike. Dec-Feb is the least preferred month for bike renting.

* The rental bike demand was more on a weekday than on weekends. The majority of clients belong to the working class.

* The temperature of 20-30 Degrees, evening time 4 pm- 8 pm and the humidity between 40%-60% are the most favourable parameters where the Bike demand is at its peak.

* Temperature, humidity, hour of day, solar radiation and functional day are major driving factors for the bike rent demand.


## Modeling:
**Model selection approach:-**

* We are working on a dataset which contains outliers. Hence we have to choose a model which is less sensitive to outliers.

* List of Machine Learning algorithms which are less sensitive to outliers:

1. Decision Tree
2. Random Forest
3. XGBoost
* A dataset with many categorical independent variables which are not linearly related to a dependent variable. Hence it is not advisable to use linear models to make   predictions. We can use tree models instead.

* Choose the model with the highest accuracy for deployment.

**Evaluation of build Model:-**

* Model evaluation is very important in data science. It helps to understand the performance of model and makes it easy to present model.

* We know that the data we are working with contains outliers, we didnt drop them because if we do so, we may loose out important trends/patterns in the data.

* The MAE is a good measure for evaluating the performance of a model because MAE is proportional to the observed mean and MAE is robust to outliers.

* Adjusted R Square will penalize additional independent variables added to the model and adjust the metric to prevent overfitting issues.

**Model Summary:-**
* Summarizing the results obtained
![Screenshot 1](https://user-images.githubusercontent.com/101059401/193441659-f8f4598c-1b3e-48a9-811f-77866333b9b1.png)



* The XG Boost model has the lowest test MAE. A low MAE value indicates that the simulated and observed data are close to each other and show better accuracy. Thus lower MAE is better for model performance. (XG Boost model with an accuracy of  88.52 %)
