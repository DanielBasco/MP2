# MP2
Car dataframe.

1) Which are the most decisive factors, forming the price of a car?
   When we created the price_segment we used ccm2, km/l, kilometertal and alder.
   When we checked the importance of the attributes from the model, we saw alder had the highest importance value of 31%
   then km/l with 29.89%, kilometertal with 28.25% and the lowest influence ccm2 with 10.37%.
   
2) Which make and model of a car is most popular, according this data source? Which are its
technical characteristics?
The most popular car is the Ford Fiesta and it's technical characteristics are High price according to our price segment,
11.39 km/l, 5 doors, ccm2 = 1000.0 and the model is EcoBoost Titanium X. 

3) Is there any obvious tendency in the preference of the car models during the past 5-10 years?
 It shows Fiesta is quite popular throughout the 10 years and we can see a tendency from 10-years to now that
 the amount is growing. Yaris and Aygo appears more often from 5 years to now, but with some outliers like Aygo 7 years ago.

4) Do people in Denmark prefer big or small cars? How reliable is your answer of this question?
We look at engine size compared to what preferences people have in Denmark/Our dataframe, it shows most people prefer smaller engines. Our answer isn't much accurate since we couldn't find the size of the cars but only the engine.
     
5) Are there any locations in Denmark, where the expensive cars are preferred choice by the
owners?
We used our price_segment model and compared it to the region attribute where we looked at the count on the very high segment. We can observe Syd- og Sønderjylland with 150 cars in very high price segment and København with 147 cars in very high price segment are the region with the highest prices of a car according to our classifcation model.

6) Which machine learning methods did you choose to apply in the solution and why?
  Firstly we applied linear regression (supervised learning) to predict the value of price.
  Secondly we applied Clustering with K-mean algorithm (unsupervised learning) to make categories and segments based on specific attributes like price, km/l etc.
  The third method we used was classification to try and predict the segment/category of a price without using the   attribute price
   
7) How accurate are your solutions of prediction? Explain the meaning and the difference between
the various quality measures.

For the classification we use Accuracy, Precision, Recall and F1-score. Accuracy: 0.83/83%
It means that 83% of the cars got placed in the right price segment. 

Precision shows how many of the cars the model predicts in a category, that actually belongs in that category
Examples from our output:
High: 0.88
Low: 0.80
Medium: 0.79
Very high: 0.88

Recall shows how many of the right cars in a category the model find
Example:
High recall = 0.74     

F1-score is a balance between precision and recall
Example:
Segment    F1-score
High    0.80
Low    0.85
Medium    0.78
Very high    0.90.       

Accuracy: 83% is good
It's best at predictiom the Very high cars segment 90%
It's hardest task is to predeict the medium cars segment 78%

For regression we've used MAE, MSE, RMSE and R²
- MAE: output is: 48061.378942819334 which means that the model calculates 48061.4 wrong in the price.
- MSE:  measures the average squared difference between predicted and actual values. We have a value on 4015105119.12623 which can be translated to 63,364. It means that the model from what MSE have calculated, that the model calculates 63.364 wrong in the price.
- RMSE:  Is the square root of MSE and represents the typical size of prediction errors  in the same unit as price. If RMSE is close to MAE, it means the model does not produce many extreme errors.
- R²: The R² score indicates how much of the variation in car prices is explained by the model. From the R² value, the model explains approximately 60% of the variation in car prices.

Short conclusion: The regression model explains about 60% of the variation in car prices. On average the prediction error is around 48,000–63,000 DKK. The classification model has an accuracy of about 83%, meaning most cars were placed in the correct price segment. Overall, the models perform reasonably well, but some factors influencing car prices are not included in the dataset.

8) What could be done for further improvement of the accuracy of the models?
   If we want more accuracy of the models we need to implement more attributes like: make, type and even small ones like doors. We can also compare our decision tree to our random forest and see a much bigger accuracy for the random forest
   due to multiple trees with less overfitting.
   
9) Which were the challenges in the project development?
A big challenge was the cleaning part, where we needed to have an overview og what should be sorted and how we could simplify and make the columns understandable as much as possible.
A challenge during clustering with k-means was to analyze the elbow method which could be interpreted as 3 and 5 too. 





Asger and Daniel.
