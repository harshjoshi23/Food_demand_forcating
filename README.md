<b> Food_demand_forcating </b> 

<b>Context</b>
It is a meal delivery company which operates in multiple cities. They have various fulfillment centers in these cities for dispatching meal orders to their customers. The client wants you to help these centers with demand forecasting for upcoming weeks so that these centers will plan the stock of raw materials accordingly.

<b>Content</b>
The replenishment of majority of raw materials is done on weekly basis and since the raw material is perishable, the procurement planning is of utmost importance. Secondly, staffing of the centers is also one area wherein accurate demand forecasts are really helpful. Given the following information, the task is to predict the demand for the next 10 weeks (Weeks: 146-155) for the center-meal combinations in the test set

<b>Inspiration</b>
Forecasting accurately could male the business growth in well directed direction.


<b> Problem Statement </b> <br>
Your client is a meal delivery company which operates in multiple cities. They have various fulfillment centers in these cities for dispatching meal orders to their customers. The client wants you to help these centers with demand forecasting for upcoming weeks so that these centers will plan the stock of raw materials accordingly.<br>

The replenishment of majority of raw materials is done on weekly basis and since the raw material is perishable, the procurement planning is of utmost importance. Secondly, staffing of the centers is also one area wherein accurate demand forecasts are really helpful. Given the following information, the task is to predict the demand for the next 10 weeks (Weeks: 146-155) for the center-meal combinations in the test set:  <br>

Historical data of demand for a product-center combination (Weeks: 1 to 145)
Product(Meal) features such as category, sub-category, current price and discount<br>
Information for fulfillment center like center area, city information etc.<br>

<b>Data Dictionary</b>
 
Weekly Demand data (train.csv): Contains the historical demand data for all centers, test.csv contains all the following features except the target variable<br>
 

<b>Variable	Definition:</b><br>
 
id	Unique ID<br>
week	Week No<br>
center_id	Unique ID for fulfillment center<br>
meal_id	Unique ID for Meal<br>
checkout_price	Final price including discount, taxes & delivery charges<br>
base_price	Base price of the meal<br>
emailer_for_promotion	Emailer sent for promotion of meal<br>
homepage_featured	Meal featured at homepage<br>
num_orders	(Target) Orders Count<br>
   

fulfilment_center_info.csv: Contains information for each fulfilment center: <br>
 
Variable	Definition<br>
center_id	Unique ID for fulfillment center<br>
city_code	Unique code for city<br>
region_code	Unique code for region<br>
center_type	Anonymized center type<br>
op_area	Area of operation (in km^2)<br>
 

meal_info.csv: Contains information for each meal being served :<br>
 
Variable	Definition<br>
meal_id	Unique ID for the meal<br>
category	Type of meal (beverages/snacks/soups….)<br>
cuisine	Meal cuisine (Indian/Italian/…)<br>
 

<b>Evaluation Metric </b>:
The evaluation metric for this competition is 100*RMSLE where RMSLE is Root of Mean Squared Logarithmic Error across all entries in the test set.<br>

<b>Public and Private Split: </b><br>
Test data is further randomly divided into Public (30%) and Private (70%) data.<br>

Your initial responses will be checked and scored on the Public data.<br>
The final rankings would be based on your private score which will be published once the competition is over.<br>
