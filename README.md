# Bike-Sharing-Demand-Prediction-

## Seoul-Bike-Sharing-Demand Prediction 
In this project, we train a model to predict the number rental bikes at any hour of the given year in different weather condition like Temprature, Humidity, Windspeed, Dew Point Temprature, Radiation, Snowfall, and Rainfall.
First we did EDA (Exploratory Data Analysis) on given data set to get insight of data and after knowing all variable factors and target variable and relation between them we will apply different kind of Regression models. 
We evaluated different models on the basis of evaluation metrics and compared different models are, Linear Regression, Lasso Regression, Ridge REgression, Elastic Net REgression, Desicion Tree Regressor, Random Forest Regressor. 
We also did Hyperparameter Tunning to get the optimal values for to get best accuracy of the model.

## Objective 
The main Objective of our project is to predict future bike sharing demand with best regression model to get the best accuracy. 
## Data Description 
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.
Attribute Information:

1. Date : year-month-day
2. Rented Bike count - Count of bikes rented at each hour
3. Hour - Hour of he day
4. Temperature-Temperature in Celsius
5. Humidity - %
6. Windspeed - m/s
7. Visibility - 10m
8. Dew point temperature - Celsius
9. Solar radiation - MJ/m2
10. Rainfall - mm
11. Snowfall - cm
12. Seasons - Winter, Spring, Summer, Autumn
13. Holiday - Holiday/No holiday
14. Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

## Libraries and Tools 
1. Numpy 
2. Pandas 
3. Scipy 
4. sklearn 
5. Seaborn 
5. Matplotlib 
## EDA Analysis
    1. We can clearly see in EDA that Bike Rent Count is strongly dependant on Hour Count during different days throughout 
       week, months and season's.
    2. There is high colinearity present between Temprature and Dew Point Temprature.
    3. There is no strong linear relation between dependant variable and independant variable. 
    
## Conclusion 
1. In holidays or non-working days there is demand in rented bikes.
2. There is a surge of high demand in the morning 8AM and in evening 6PM as the people might be going to their office at morning 8AM and returning from their office at the 6PM.
3. People preferred more rented bikes in the morning compared with evening.
4. When the rainfall was less, people have booked more bikes except some few cases.
5. The temperature, Hour are the most important features that positively drive the total rented bikes count.
6. It is observed that highest number of rental bikes counts in Autumn and summer seasons and the lowest in winter season.
7. We observed that the highest number of rental bikes counts on a clear day or little windy day and the lowest on a snowy and rainy day.
8. In the given dataset there was no strong relationship present between dependent variable "Rented bike count" and independent variables.
9. Out of all models we apply Decision tree and Random Forest model are most accurate and the reason is there are no specific relation between features.
10.	Random Forest worked best in predicting the count of rented bikes as its R2 score is maximum from the tried model.
11. We are getting best results using Gradient Boost Regressor.
The plot is as follows 
![image](https://user-images.githubusercontent.com/109215374/199481923-cca5863e-68fa-44ea-8a21-2164b1951b62.png)
