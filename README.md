# Project-Bankruptcy-prediction
# Key features: 
EDA, Logistic Regression, Random Forest, Naive Bayes, Decison Trees, Ensemble methods, Ridge, Lasso models. 

# Business objective: 
the objective of the analysis is to predict whether a company will go bankrupt or not given the various features of a company that would help in predicting the strength of a company and its adaptability like industrial risk, credibility, competitiveness, etc. To also find out which features of the entire data set affect the classification variable the most. 

# Data Visualizations:
there are 250 rows and 7 columns, each row represents one company. the first six columns represent the various features like industrial risk, financial flexibility, credibility, etc. and the seventh column denotes whether the company is bankrupt or not. the features take three values 0, 0.5 and 1.0, the class variable takes two values- bankrupt and non-bankrupt.  For industrial risk, the value of 0 means the risk is low and 1 means that the risk is high. But if the credibility is 0 then the credibility is low and if 1 then the credibility is high. EDA -  firstly, a heatmap is plotted with the input data being the correlation values between the features and the class variable. With financial flexibility, credibility and competitiveness being the features having the most correlation values with respect to the class variable. Hence they are the most important features.  secondly, various cross tabulation plots are then plotted like the ones between financial_flexibility and class variable, the operating_risk and class variable. thirdly, isolation forests and anamoly detection is done to detect the outliers, there were three outliers and they were removed. Feature Engineering- Univariate Feature Selection and Random Feature Elimination algorithms are done to identify the most important feature for the classification to be done. Bothe the algorithms give the same results and these results coincide with the conclusions made after the correlation analysis. 

# Data Modeling: 
the train-test splitting model is done with the test data being 20% of the dataset. Various classification models are used to classify the data accurately. Logistic Regression is used and an accuracy of 100% is obtained on both the training and testing dataset. The ridge and lasso regularization modesl are used, elasitc net model is also used. knearest neighbors is used, naive bayes classifier is used, support vector machines and decision tree classifier. Random Forest classifier and neural network models are also used. The various models are used to train and predict the values on the test dataset.  The finalized model is Decision Tree Classifier the F1 score is: 0.975. 

# Model Deployment:
Stremalit api is used to deploy this model.
