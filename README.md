# Analyticsindiamag-used-car-price-prediction
Machine hack Predicting The Costs Of Used Cars - Hackathon By Imarticus Learning

![alt text](https://github.com/Anbulenin/Analyticsindiamag-used-car-price-prediction/blob/master/Predicting-The-Costs-Of-Used-Cars-Hackathon-By-Imarticus-1-1-768x432.jpg)
 



Numerical values:
•	Kilometers Driven
•	Mileage
•	Engine
•	Power
•	Price
Categorical values:
•	Name
•	Location
•	Year
•	Fuel type
•	Transmission
•	Owner type
•	Seats

Preprocessing :

Train data preprocessing:
1.Remove  New_price column  
2. Remove all NULL values from Train data
3. Handle missing values in Test data
 
Mileage, Engine, Power is replaced with Mean of respected columns.
Seats are replaced with most frequent item. 


4. Check unique variables in both test data and train data.  
Remove Lamborghini from Train data. (for better decision making) 
Remove 1996 row from Test data. (Since 1996 is not present in train data)

5. Combine Train data and Test data (concat)
6. Label encode Categorical variables 
7. One hot encode the label encoded variables 
8. Extract the Price column into Y variable (remove from dataframe) and apply minmax transformation 
9. Apply minmax scalar over a whole dataframe (X)
10. Split the dataframe into Train and Test
11. Train the model with 100% of Train data
12. Make Predictions using Test data
13. Inverse transform the minmax scalar applied over Y (Price from Train)
14. On the Place of year (1996 year) input the average value of predicted results.
    Approx. values for 1996 is  (4.0 lacks)
15. Save the results in a dataframe.
 
![alt text](https://github.com/Anbulenin/Analyticsindiamag-used-car-price-prediction/blob/master/results%20form%20validation.JPG)




Further optimization:
•	Handling NULL values in train data, test data with subbytes of the whole dataframe.
•	Feature Importance for better correlated features.
•	Feature engineering with valuable formulation with existing parameters.
•	Model ensemble for better predictions. 
 


