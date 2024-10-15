- **DOMAIN :*** Automobiles 
- **CONTEXT :** There is a huge demand for used cars in the Indian Market today. As sales of new cars have slowed down in the recent past, the pre-owned car market has continued to grow over the past years and is larger than the new car market now. Cars4U is a budding tech start-up that aims to  ind footholes in this market. In 2018-19, ![ref2]while new car sales were recorded at 3.6 million units, around 4 million second-hand cars were bought and sold. There is a slowdown in new car sales and that could mean that the demand is shifting towards the pre-owned market. In fact, some car sellers replace their old cars with pre-owned cars instead of buying new ones. Unlike new cars, where price and supply are fairly deterministic and managed by OEMs (Original Equipment Manufacturer / except for dealership level discounts which come into play only in the last stage of the customer journey), used cars are very different beasts with huge uncertainty in both pricing and supply. Keeping this in mind, the pricing scheme of these used cars becomes important in order to grow in the market. As a senior data scientist at Cars4U, you have to come up with a pricing model that can effectively predict the price of used cars and can help the business in devising pro itable strategies using differential pricing. For example, if the business knows the market price, it will never sell anything below it.
- **DATA  DESCRIPTION  :** The  data  contains  the  different  attributes  of  used  cars  sold  in  different  locations.  The detailed data dictionary is given below.
- **DATA DICTIONARY :** 
1. S.No.: Serial number 
1. Name: Name of the car which includes brand name and model name
1. Location: Location in which the car is being sold or is available for purchase (cities)
1. Year: Manufacturing year of the car
1. Kilometres\_driven: The total kilometers driven in the car by the previous owner(s) in km
1. Fuel\_Type: The type of fuel used by the car (Petrol, Diesel, Electric, CNG, LPG)
1. Transmission: The type of transmission used by the car (Automatic/Manual)
1. Owner: Type of ownership 
1. Mileage: The standard mileage o ered by the car company in kmpl or km/kg
1. Engine: The displacement volume of the engine in CC
1. Power: The maximum power of the engine in bhp
1. Seats: The number of seats in the car
1. New\_Price: The price of a new car of the same model in INR Lakhs (1 Lakh INR = 100,000 INR)
1. Price: The price of the used car in INR Lakhs
- **PROJECT OBJECTIVE*:***   

To explore and visualise the dataset, build a linear regression model to predict the prices of used cars, and generate a set of insights and recommendations that will help the business

- **STEPS AND TASKS** : **[ Total Score: 40 Marks]** 
1. Data Understanding and Preparation**:** [10 Marks]
1. Read the  used\_cars\_data.csv  dataset, check the dimensions and print the  irst 10 rows.  [1 Mark] 
1. Check data types and duplicate values in the data-frame. Treat the duplicates if any, with an explanation to your approach.  [1 Mark] 
1. Observe if there s any relationship between the units given in the mileage column and the Fuel\_Type. Split mileage column into numeric values and units. [1 Mark]** 
1. Extract numeric values from  Engine ,  Power  and  New\_Price . Check for variation in their units and drop the units if necessary [1 Mark] 
1. Extract the Car Brand Name and Model Name from the  Name  column. **[**1 Mark]** 
1. Create new variables by log transforming  Price  and  Kilometers\_Driven  columns as  price\_log  and  kilometers\_driven\_log . [1 Mark] 
1. Drop the redundant columns and print a 5-point summary of the data-frame and share your observation.** [1 Mark] 
1. Check the missing values and extreme values in the dataset and impute them. [1 Mark](Do not impute missing values for price as it is our target column).![ref2]
1. Check the distribution of non-numeric features (display the  irst 10 values if the number of categories/ classes are more than 10). [1 Mark] 
1. Share the average of used car prices by brand. [1 Mark] 
2. Data Exploration and Analysis: [10 Marks] 
   1. Perform Univariate Analysis on numerical and Categorical data. Share your insights.                                            [5 Marks] 
   1. Perform detailed Bivariate and Multivariate Analysis on the data and share your insights.                                     [5 Marks] 
2. Model Building: [15 Marks]
1. Drop the missing values in price and  price\_log . [1 Mark] 
1. Create dummy variables for string type variables and convert other column types to  loat if any                       [1 Mark] 
1. Model with Price 
   1) Split the data into X and Y, where Y= Price and Drop  price\_log . [1 Mark]  
   1) Split the dataset into train and test sets with 70:30 proportion. [1 Mark] 
   1) Fit a linear regression model. [1 Mark] 
   1) Check the performance of the model using appropriate performance metrics. [2 Mark] 
1. Model with log\_Price 
   1) Split the data into X and Y, where Y= price\_log and Drop  Price . [1 Mark]  
   1) Split the dataset into train and test sets with 70:30 proportion. [1 Mark] 
   1) Fit a linear regression model. [1 Mark] 
   1) Check the performance of the model using appropriate performance metrics. [2 Mark] 
1. Compare the performance of both for the train & test set and provide your insights. [3 Marks]

**4.Business Recommenda on: [5 Marks]** 

A. Provide a detailed and useful Business Insights and Recommendation based on your observations and 

analysis
