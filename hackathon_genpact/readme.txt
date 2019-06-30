# machine_learning_hackathon
Analytics Vidhya: genpact machine learning hackathon. Predict the demand for the next 10 weeks (Weeks: 146-155) for the center-meal combinations in the test set.


DATA DICTIONARY:
 
Weekly Demand data (train.csv): Contains the historical demand data for all centers, test.csv contains all the following features except the target variable
 
VARIABLE 		DEFINITION
id 			Unique ID
week 			Week No
center_id 		Unique ID for fulfillment center
meal_id 		Unique ID for Meal
checkout_price 		Final price including discount, taxes & delivery charges
base_price 		Base price of the meal
emailer_for_promotion 	Emailer sent for promotion of meal
homepage_featured 	Meal featured at homepage
num_orders 	(Target) Orders Count
 

fulfilment_center_info.csv: Contains information for each fulfilment center
 
VARIABLE 	DEFINITION
center_id 	Unique ID for fulfillment center
city_code 	Unique code for city
region_code 	Unique code for region
center_type 	Anonymized center type
op_area 	Area of operation (in km^2)
 

meal_info.csv: Contains information for each meal being served

VARIABLE 	DEFINITION
meal_id 	Unique ID for the meal
category 	Type of meal (beverages/snacks/soups….)
cuisine 	Meal cuisine (Indian/Italian/…)

EVALUATION METRIC
The evaluation metric for this competition is 100*RMSLE where RMSLE is Root of Mean Squared Logarithmic Error across all entries in the test set.
Public and Private Split

Test data is further randomly divided into Public (30%) and Private (70%) data.

    Your initial responses will be checked and scored on the Public data.
    The final rankings would be based on your private score which will be published once the competition is over.

lINK: https://datahack.analyticsvidhya.com/contest/genpact-machine-learning-hackathon/ 

