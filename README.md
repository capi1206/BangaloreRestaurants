# BangaloreRestaurants
Regression model for predicting the approximate price per dish in restaurants in Bangalore,
the model first tries a regression over the whole data. The models produce a MSE of about 50000 units
after cleaning and transforming the variables into a Machine Learning usable format.
After that a new set of variables is created,
these variables tell how one of the initial variables is related to the cost of the dish being above or below the average
price . Wether they are positively or negatively correlated. With this new variables a clustering algorithm generates naturally two 
groups, using the elbow method.
With these new groups a regression model is generated for each particular group and the MSE lowers to about 6000 units, considerably 
lower than the initial formulation.

Later a k nearest neighbours algorithm determines to which cluster a new point should belong basing the proximity distance in the old features 
which are originally used to predict the price, this algorithm determines the right cluster of a point with 100% precision
