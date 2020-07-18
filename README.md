# Hourly_Energy_Consumption
Over 10 years of hourly energy consumption data from PJM in Megawatts

## PJM Hourly Energy Consumption Data

PJM Interconnection LLC (PJM) is a regional transmission organization (RTO) in the United States. It is part of the Eastern Interconnection grid operating an electric transmission system serving all or parts of Delaware, Illinois, Indiana, Kentucky, Maryland, Michigan, New Jersey, North Carolina, Ohio, Pennsylvania, Tennessee, Virginia, West Virginia, and the District of Columbia.

The hourly power consumption data comes from PJM's website and are in megawatts (MW).

The regions have changed over the years so data may only appear for certain dates per region.

<p align="center">
  <img src="https://github.com/panambY/Hourly_Energy_Consumption/blob/master/image/PJM_Energy_Cosumption.png">
</p>

This is a Kaggle dataset which can be found in this link: https://www.kaggle.com/robikscube/hourly-energy-consumption

<p align="center">
  <img src="https://github.com/panambY/Hourly_Energy_Consumption/blob/master/image/power_electric_plant.jpg">
</p>

I followed in this project the steps of the project management method called CRISP-DM. This method has undergone modifications aimed at the reality of a Data Science project and with that it was called CRISP-DS.

CRISP-DS has the following steps with their respective courts:

### 1 - Business Question
Predict how much energy the power companies in the datasets will consume in the next 12 months.<br>
### 2 - Understanding the Business
This forecast will be used to plan companies in relation to the investments necessary for the expansion and maintenance of their power plants. <br>
### 3 - Data Collection
**0.0 - IMPORTS** <br>
	0.1 - Helper Function <br>
	0.2 - Loading Data <br>
### 4 - Data Cleaning
**1.0 - DESCRIPTION OF DATA** <br>
	1.1 - Rename Columns <br>
	1.2 - Data Dimensions <br>
	1.3 - Data Types <br>
	1.4 - Check NA <br>
	1.5 - Fillout NA <br>
	1.6 - Change Types <br>
	1.7 - Descriptive Statistical <br>
		- 1.7.1 - Numerical Attributes <br>
		- 1.7.2 - Categorical Attributes <br>
**2.0 FEATURE ENGINEERING** <br>
	2.1 - Creation of Hyphoteses <br>
		- 2.1.1 - Demographic Hyphoteses <br>
		- 2.1.2 - Geographic Hyphoteses <br>
		- 2.1.3 - Sociocultural Hyphoteses <br>
	2.2 - Final list of Hypotheses <br>
	2.3 - Feature Engineering <br>
**3.0 - VARIABLE FILTERING** <br>
	3.1 - Line filtering <br>
	3.2 - Column Selection <br>
### 5 - Data Exploration
**4.0 - EXPLORATORY DATA ANALYSIS** <br>
	4.1 - Univariate Analysis <br>
		- 4.1.1 - Response Variable <br>
		- 4.1.2 - Numerical Variable <br>
		- 4.1.3 - Categorical Variable <br>
	4.2 - Bivariate Analysis <br>
		- 4.2.1 - Summary of Hyphoteses <br>
	4.3 - Multivariate Analysis <br>
		- 4.3.1 - Numerical Attributes <br>
		- 4.3.2 - Categorical Attributes <br>
### 6 - Data Modeling
**5.0 - DATA PREPARATION** <br>
	5.1 - Normalization <br>
	5.2 - Rescaling <br>
	5.3 - Transformation <br>
		- 5.3.1 - Encoding <br>
		- 5.3.2 - Response Variable Transformation <br>
		- 5.3.3 - Nature Transformation <br>
**6.0 - FEATURE SELECTION** <br>
	6.1 - Split dataframe into training and test dataset <br>
	6.2 - Boruta as Feature Selection <br>
		- 6.2.1 - Best Feature from Boruta  <br>
### 7 - Machine Learning Algorithms
**7.0 - MACHINE LEARNING MOMDELLING** <br>
	7.1 - Average Model <br>
	7.2 - Linear Regression Model <br>
		- 7.2.1 - Linear Regression Model - Cross Validation <br>
	7.3 - Linear Regression Regularized Model <br>
		- 7.3.1 - Linear Regression - Lasso - Cross Validation <br>
	7.4 - Random Forest Regressor <br>
		- 7.4.1 - Random Forest Regressor - Cross Validation <br>
	7.5 - XGBoost Regressor <br>
		- 7.5.1 - XGBoost Regressor - Cross Validation <br>
	7.6 - Compare Model's Performance <br>
		- 7.6.1 - Single Performance <br>
		- 7.6.2 - Real Performance - Cross Validation <br>
**8.0 - HYPERPARAMETER FINE TUNING** <br>
	8.1 - Random Search <br>
	8.2 - Final Model <br>
### 8 - Evaluation of Algorithms
**9.0 - TRANSLATION AND INTERPRETATION OF THE ERROR** <br>
	9.1 - Business Performance <br>
	9.2 - Total Performance <br>
	9.3 - Machine Learning Performance <br>
### 9 - Production Model
**10.0 - DEPLOY MODEL TO PRODUCTION** <br>
	10.1 - Energy Consumption Class <br>
	10.2 - API Handler <br>
	10.3 - Tester <br>
