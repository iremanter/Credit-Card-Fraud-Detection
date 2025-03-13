# Credit-Card-Fraud-Detection

**Data Cleaning:**

The main objective of this task is to detect fraudulent transactions in the credit card dataset. During this analysis, the "creditcard.csv" dataset with 284,807 records, collected over two days, has been used. This dataset includes information of some confidential features, which are converted to numerical values and named V1, V2, ..., V28, the number of seconds elapsed between the first transaction and other transactions, transaction amounts, and fraudulent transactions.
In this real life case study of a financial institution, the main focuses are to examine the data, perform necessary preprocessing and cleaning methods, identify and visualize the trends and patterns by using linear algebra concepts, analyzing the correlation between attributes, developing models to detect credit card fraud transactions, and finally evaluating and comparing the models’ performance.

Information and types of the dataset have been obtained, descriptions as min-max values, average etc. have been listed and missing values of the credit card dataset have been checked. Also, duplicated values of the dataset have been determined and eliminated. The ‘Class’ attribute is a boolean attribute and ‘0’ indicates no fraud and ‘1’ indicates fraud transaction. After the duplicate elimination, the total number of both non-fraudulent and fraudulent transactions have been counted. There are 283,253 non-fraudulent transactions and 473 fraudulent transactions. 

**Exploratory Data Analysis (EDA):**
In this part, fraudulent and non-fraudulent transactions have been visualized. It is revealed that only 0,17% of the dataset contains fraud records. Moreover, heatmap has been plotted in order to see the correlation between the features and their importance. To obtain the importance levels of features on fraud actions, bar-chart has been plotted. It was revealed that V17, V14, and V12 features have the most effect on fraud actions.
Lastly, statistical details of transaction amount of fraud records have been listed as count, mean, standard deviation, min-max values etc.

**Data Modelling:**
Before developing the models, outliers were eliminated using the z-score method. During the literature review, an article highlighted the importance of outlier elimination using the z-score technique.
Afterward, min-max scaling was performed to normalize the data, and then the dataset was split into training (80%) and testing (20%) sets.

Random Forest and Decision Tree Models wer developed.

**Model Comparison and Evaluation:**

Random Forest Model’s performance metrics as follows: Accuracy is 0.9996. For the fraudulent transactions; Precision is 0.98, Recall is 0.79 and F1-Score is 0.88.
Decision Tree Model’s performance metrics as follows: Accuracy is 0.9991. For the fraudulent transactions; Precision is 0.71, Recall is 0.74, and F1-Score is 0.72.
To sum up, the Random Forest model has higher precision, recall, and F1-score for fraud detection compared to the Decision Tree model. While the Random Forest model is more reliable for identifying fraud cases, the Decision Tree model leads to more false positives and a worse performance. Therefore, the Random Forest model is better for fraud detection due to its higher precision and recall.

ROC curve graph compares a Random Forest model and a Decision Tree model. By examining True Positive Rate vs. False Positive Rate, it has been obtained that both models are good at distinguishing between positive and negative classes. However, when Area Under the Curve (AUC) is considered, Random Forest model with an AUC of 0.96 is better than Decision Tree model with an AUC of 0.91.
In conclusion, the Random Forest model performs better at distinguishing between classes than the Decision Tree model, as shown by its higher AUC score.
