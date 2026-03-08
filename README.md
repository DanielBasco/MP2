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

8) What could be done for further improvement of the accuracy of the models?
   If we want more accuracy of the models we need to implement more attributes like: make, type and even small ones like doors. We can also compare our decision tree to our random forest and see a much bigger accuracy for the random forest
   due to multiple trees with less overfitting.
   
9) Which were the challenges in the project development?
A big challenge was the cleaning part, where we needed to have an overview og what should be sorted and how we could simplify and make the columns understandable as much as possible.
A challenge during clustering with k-means was to analyze the elbow method which could be interpreted as 3 and 5 too. 





Asger and Daniel.
