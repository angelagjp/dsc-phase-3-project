
# Predictions for At Fault Drivers




# Overview

Using Logistic Modeling and DecisionTreeRegression to predict the possibility of a driver being at fault for car crashes in the Chicargo, IL area. The Data was provided by the Chicago, IL police department.

### The Data

The Data used is the data provided by the Chicargo data portal, Traffic Chrashes- Crashes. The data is provided by the Chicargo police department and includes weather condition, injuries, and roadway condition. The Data originally had 49 columns but only 23 columns were ultimately used. 

### Business Problem

Geico would like a way to predict the car crash cases that they should presue an investigation with. They would like to avoid allocating funds to a unnecessary investigations. 


### The Predictive Models


Initially, there was an attempt to check the class balance of the target data. The target data includes has two values, 0 for outside circumstances and 1 for Driver's fault. The class balance check found that the balance is very close to even with a slight bias to false positive. The balance was not adjusted because the sloght balance could benifit Gieco with finding at fauld Drivers. 


![class_balance](./dsc-phase-3-project/images/class_balance.png)

The first 2 models were logistical models using different aspects of the data. The inital model only incorporated the numerical features from the DataFrame. The accuracy score was about 57%. In an attempt to increase the predictivity the categorical features were added in the second model. This addition did not help the model and dropped the accuracy model to 54%. Finally, a DecisionTreeRegression model was used as an attempt to change the predictive model and increaset the accuracy score. The score increase from the second logistical model but was still 1% less then the original model, accuracy score of 55%.


### Conclusions

In conclusion, the best features for predicting the fault of Drivers in car crashes in Chicargo, IL were the numerical features. The features such as speed limit and time of day, had an accurancy of about 57% . Categorical features could predict a crash more then half the time but it is still less then that of the numerical features, categorical features can predict the crashes about 54% of the time. Furthermore, The  DecisionTreeRegressor model was a better indicator then the logistical model that included the categoricals but it was still about 1% less then the original logistical model that only included that numerical model. 
