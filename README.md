# Coursera_Capstone1

# Analysing accident data

Please see the accompanying Notebook here - https://jupyterlab-24.labs.cognitiveclass.ai/hub/user-redirect/lab/tree/labs/DV0101EN/Coursera_Capstone1/Capstone%20projectV2.ipynb

# Discussion of the background:

To complete Capstone, I will be working on a case study which is to predict the severity of an accident. 

Say you are driving to another city for work or to visit some friends. It is rainy and windy, and on the way, you come across a terrible traffic jam on the other side of the highway. Long lines of cars barely moving. As you keep driving, police car start appearing from afar shutting down the highway. Oh, it is an accident and there's a helicopter transporting the ones involved in the crash to the nearest hospital. They must be in critical condition for all of this to be happening.

# Problem:
Now, wouldn't it be great if there is something in place that could warn you, given the weather and the road conditions about the possibility of you getting into a car accident and how severe it would be, so that you would drive more carefully or even change your travel if you are able to. Well, this is exactly what you will be working on in this course.

# Data:
We will be using our shared data for Seattle city as an example of how to deal with the accidents data. 

The first column is the labelled data. The remaining columns have different types of attributes. Some or all can be used to train the model.

The label for the data set is severity, which describes the fatality of an accident. The shared data has unbalanced labels. The data will be balanced, otherwise, you will create a biased ML model. We can do some feature engineering to improve the predictability of the model.

# Attributes: 
In total there are 37 attributes (columns). Some attributes have missing data, and includes both numerical and categorical types of data. Attributes include Location, Weather condition, Car speeding, Light conditions, Road condition, Junction junction, number of people involved, number of vehicles involved. 

Severity key 1 = Property Damage Only Collision    (136485 collisions)
Severity key 2 = Injury Collision                   (58188 collisions)

# Methodology:
The problem states that the road conditions and weather should be categories that indicate whether there is likelihood of getting into a car accident.

I have decided to use a **decision tree** because, looking at the categories, the weather and road conditions will effectively point to a damage only collision, or an injury collision. If a decision tree does not produce a high enough accuracy, I will try another method.

I will **clean the data** removing any blank or Unknown values from the Weather and Road Conditions columns. 

# Discussion: 
The problem with the data is that it only tells us of those journeys where there was an accident. It does not help tell us whether a journey will definitely result in an accident or not. 

# Conclusion:

In conclusion, based on the work done below, the data set cannot tell us the the possibility of getting into a car accident, but can tell us that if we are in an accident in certain conditions how severe it would be.

The decision tree model works 100% of the time on the test data after being trained. 
