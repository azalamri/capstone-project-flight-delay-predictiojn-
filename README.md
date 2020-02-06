# Predicting Flights Delays Using Machine Learning

## Motivation

Flight delays cause a lot of problems for both airports and individuals.

in this analysis, I've attempted to tackle flight delays using machine learning. you can find a detailed explanation on a medium post [here](https://medium.com/@azalamri3/predicting-flights-delays-using-machine-learning-bfe24999dee4)

## Installations

This project requires Python 3.x and the following Python libraries installed:
* Pandas
* NumPy
* Scikit-learn
* seaborn
* matplotlib.pyplot

## Procedure
- 1- **Expolratory data analysis:** I've checked the data and how it looks like: Features types, nulls values, visualizations, descriptive statistics
- **2- Cleaning the data:** remove unnecessary columns and rows that are outliers (2 rows)
- **3- Data Wrangling:** did a feature engineering with some columns by separating them into many columns -as much as needed- to come with better features for the analysis. Also, changing the data type of categorical features from categorical variables into dummy/indicator variables.
- **4- Implementation of machine learning:** 
- Supervised learning and unsupervised learning algorithms were used in this analysis.
- Supervised learning: linear regression and random forest regression 
- Unsupervised learning: logistic regression and random forest classifier

## Summary & Results
In this project, I've tried regression to predict delay time and Classification to determine the flight status to be on time or will be delayed.

1- Descriptive statistics

| |FLIGHT_NUMBER|DALAY_EARLY_MIN|TOTAL_PASSENGERS|
|---|---|---|---|
|**count**|*31531.000000*|31531.000000|31531.000000|
|**mean**|*864.703688*|58.148204|79.596609|
|**std**|*998.942303*|58.148204|79.596609|
|**min**|*5.000000 *|-586.000000|-0.000000|
|**25%**|*210.000000*|-8.000000| 97.000000|
|**50%**|*709.000000*|10.000000|131.000000|
|**75%**|*1272.000000*|26.000000|164.000000|
|**max**|*9903.000000*|2018.000000|450.000000|


2- Supervised Learning approach results:
- The metric that has been used for regression is the r2 score, we have a good solution as we the score get that is close to 1.0.
- The result of the linear regression approach was off. this might highly indicate that there is no linear relationship between the features and the target feature. On the contrary, the result of the random forest algorithm was better with an accuracy of 0.5258. However, both approaches emphasize that the regression approach (supervised learning) on this data is not really is a good idea.

3- Unsupervised Learning approach results:
- The metric that used was the accuracy score. 
- Logistic regression classifier got an accuracy of 0.7284 which is less than the accuracy obtained by random forest classifier (0.7789)

## Conclusion
The classification approach gave us better results!

## Acknowledgment
Much thanks to those who helped me to get the data, who I'm sure will read this ReadMe (cannot put their names based on their request) and to Udacity for putting my skills into action!
