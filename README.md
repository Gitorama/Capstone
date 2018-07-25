# Capstone
  For my Capstone Project, I predicted what a college student will eat for dinner. I used a kaggle dataset titled food preferences 
of college students for my analysis. The dataset consisted of 125 rows and 61 columns. I used scikit-learn's resample function to 
bootstrap the number of rows to 1000 so that I would have sufficient amounts of rows for my training and test data. I ended up taking
4 of the columns with meal/food preferences and I applied Natural Language Processing those columns so that I could extract specific
keywords and create new columns(i.e. pizza, tacos, Indian food, etc.) out of those 4 original columns(those columns either had a 1
(student liked the food) or 0(student did not like the food). I also ended up deleting a few other columns as it largely consisted of
null or erroneous values. I finally ended up with 50 features and 21 targets, and so I label encoded the features with a non-integer
datatypes and I used the Multi Output Classifier Function so that I could fit one classifier for all of the 21 targets combined.

  I did 5 different types of train test splits, one for the cleaned up dataset, one for all female students, one for all male students, 
one for all students who cook everyday, and one for all students who never cook. I did a 67/33 train test split for each scenario. I used
Logistic Regression, Tensorflow, and Random Forest Classification and ended up using Random Forest Classification to build all of my 
predictive algorithms as it gave me the highest accuracy of around 97%. 

  Some of the most shocking results were that there was only a 25% chance that a student would eat mac and cheese for dinner, and that 
there is a 92% chance that women who cook everyday will want to eat Thai Grilled Chicken Pizza for dinner and that they're 50% more 
likely to eat it than men who cook everyday. The other thing was that female college students were 19% more likely to have Thai food 
while male college students were 21% more likely to have Indian food. 
