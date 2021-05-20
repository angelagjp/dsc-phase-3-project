
# Crash Dummies




# Overview

This research is to us modeling to find predictive modeling to find the the best features to predict primary contributing factory of car crashes in the City of Chicargo, IL. 



### The Data

The Data used is the data provided by the Chicargo data portal, Traffic Chrashes- Crashes. The data is provided by the Chicargo police department and includes weather condition, injuries, and roadway condition. The data was then put through logistical modeling and a desision tree to see which model best predicted the likelihood of a car crash. 


### Business Problem

Geico is looking for the best contributing features that will predict the likelihood of crash in order to adjust their pricing for Chicargo, IL.


### Original Model
![liveable_chart](./notebooks/images/liveable_chart.png)


The first set of data used was the numeric aspect of the data, such as, the speed limit, crash hour, and crash day of the week. The data was trained and used alongside Logistic Modeling in cross validation to find the R^2. The Model found that with the numerical features a crash could be predictable up to about 57%. 


### Categorical Model 

![Aboveliveable_chart](./notebooks/images/Aboveliveable_chart.png)

The second set of data utilized the categorical data, such as, weather condition, lighting, and damage. The categorical data was put though a OneHotEncoder in order to apply a numeric value to them. The data was trained and used alongside Logistic Modeling in cross validation to find the R^2. The Model droped from predicting up to about 57% to only predicting up to about 53%.


### DecisionTreeRegressor Model

The third set of data used was still both the numerical data and caterical data but the model was changed. The Model used was a DecisionTreeRegressor Model. This DecisionTreeRegressor Model returned a negative R^2 and was not helpful in predicting the likelihood of a crash in Chicargo, IL.



### Conclusions

In conclusion, the best features for predicting a crash in Chicargo, IL were the numerical features. The features such as speed limit and time of day, about 57% chance of prediction. Categorical features could predict a crash more then half the time but it is still less then that of the numerical features, categorical features can predict the crashes about 53% of the time. Furthermore, The Logistical Model was a better choice than the DecisionTreeRegressor Model in this set of data to recieve the best results. 
