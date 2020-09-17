# Titanic 
My attempt at the Kaggle Titanic classification challenge

This is my first attempt at the Titanic survived classification challenge on Kaggle. My submission scored a 77% accuracy on the final test set. I was disappointed to not hit 80%, but I still enjoyed the project. 

The first notebook is my exploratory data analysis. I perhaps performed a bit too much EDA in this notebook, but I was focused on finding non-obvious relationships in the data. In the end, sex and pclass appeared to be the largest indicators of survival. I know some people use cabin in their final model, but I think this leads to data leakage. There are so many missing data points in 'cabin,' that I have to believe the cabin values that are known are becuase the occupant survived. In this notebook I also performed feature engineering and data cleaning on the training set.

The second notebook is data cleaning of the test set. I was sure to match all the feateure creation and cleaning steps I took for the training set. The test set was prepared for an SVC model.

The third notebook is where I run the machine learning model. I tried 4 different classifiers: random forest, gradient boosted decision tree, logistic regression, and SVC. After doing cross validation and grid search, I moved forward with the SVC model as it performed the best on the training set. 

