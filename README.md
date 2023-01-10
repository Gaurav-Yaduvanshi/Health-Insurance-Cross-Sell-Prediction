# Health-Insurance-Cross-Sell-Prediction
Capstone project -3 Health Insurance Cross Sell Prediction
# Problem Statement
Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee.
Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.
Now, in order to predict, whether the customer would be interested in Vehicle insurance, you have information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc.

#ALGORITHMS USED:
I. Logistic Regression II. Decision Tree Classifier III. Random Forest Classifier IV. KNeighbors Classifier V. GaussianNB VI. Gradient Boosting Classifier VII. XGB Classifier VIII. AdaBoost Classifier IX. LGBMClassifier

#Solution Strategy
My strategy to solve this challenge was:

Step 01: Data Description: Use statistics metrics to identify data distribuctions.

Step 02: Feature Engineering: Derive new attributes based on the original variables to better describe the phenomenon that will be modeled.

Step 03: Exploratory Data Analysis: Explore the data to find insights and better understand the impact of variables on model learning.

Step 04: Feature Selection: Selection of the most significant attributes for training the model.

Step 05: Machine Learning Modelling: Machine Learning model training.

Step 06: Hyperparameter Fine Tunning: hoose the best values for each of the parameters of the model selected from the previous step.

Step 07: Convert Model Performance to Business Values: Convert the performance of the Machine Learning model into a business result.

Step 08: Deploy Model to Production: Publish the model in a cloud environment so that other people or services can use the results to improve the business decision.

#Conclusion
After loading our dataset, we initially checked for null values and duplicates. There were no null values and duplicates so treatment of such was not required. Before data processing, we applied feature scaling techniques to normalize our data to bring all features on the same scale and make it easier to process by ML algorithms.

Through Exploratory Data Analysis, we categorized Age as YoungAge, MiddleAge, and OldAge. Further, we observed that customers belonging to youngAge are more interested in vehicle insurance. We observed that customers having vehicles older than 2 years are more likely to be interested in vehicle insurance. Similarly, customers having damaged vehicles are more likely to be interested in vehicle insurance.

For Feature Selection, We used feature imortance and we observed that Previously_Insured is the most important feature and has the highest impact on the dependent feature and there is no correlation between the numeric features.

Next we implemented nine machine learning algorithms namely, 'LogisticRegression', 'DecisionTreeClassifier', 'RandomForestClassifier', 'KNeighborsClassifier', 'GaussianNB', 'GradientBoostingClassifier', 'XGBClassifier', 'AdaBoostClassifier', 'LGBMClassifier'. We did hyperparameter tuning into improve our models performance. The 'RandomForestClassifier', 'XGBClassifier', 'LGBMClassifier' models are best performing models with test accuracy score of 82% but we have an imbalance dataset, So we have to consider precision and recall and roc_auc score as well, accuracy alone can be misleading.

Key points:

Customers of age between 30 to 60 are more likely to buy insurance.

Customers with Vehicle_Damage are likely to buy insurance.

Customers with Driving License have higher chance of buying Insurance.

The variable Vehicle_damage, Age, Previously_insured, Annual_premium are affecting the target variable.
