### Business Case

* FicZon Inc, an IT solution provider with a range of products from on-premises to SAAS-based solutions, faces challenges due to increasing market maturity and the entry of new competitors. 


* To address the dip in sales, FicZon aims to enhance sales force effectiveness, which heavily relies on lead quality. 


* Currently, lead categorization is done manually and depends heavily on the sales staff. 


* The quality process currently updates lead categorization for post-analysis rather than real-time decision-making.


* To overcome these challenges and improve sales effectiveness, FicZon plans to leverage Machine Learning for pre-categorizing lead quality.

### Problem Statement

##### " Predicting Lead Categories to Improve Sales Effectiveness "

### Project  Objective:

The objective of this project is to implement a Machine Learning-based lead classification system that pre-categorizes leads based on their quality.

### Project Goal :

The goal is to enhance sales effectiveness by enabling the sales team to prioritize high-quality leads and allocate resources efficiently.

1. Data exploration insights - Sales effectiveness.
2. ML model to predict the Lead Category ( High Potential, Low Potential )


### Summary of the project

* The project's main objective was to determine the Lead Quality, deciding whether a lead should be pursued or not. The company aimed to invest its resources in the right prospects. To achieve this, the following steps were taken:


* Data Import: Data was imported, and relevant predictor and target variables were identified. Columns with no use in the analysis were dropped.


* Label Compression and Encoding: Lead labels were compressed to include only 'Good' and 'Bad' categories. Label Encoding was applied to represent these categories numerically.


* Data Split: The dataset was divided into training and test sets. SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the data and address class imbalances.


* Algorithm Training: Various machine learning algorithms, including Logistic Regression, Support Vector Machine, Decision Tree, Random Forest, Naive Bayes, K-Nearest Neighbor and XGBoost Classifier were trained using the data. The goal was to identify the algorithm with the highest accuracy.

### Conclusion

* Earlier, the Decision Tree Classifier, Random Forest Classifier, and XGBoost Classifier outperformed Support Vector Machine and K-Nearest Neighbor in terms of performance. However, Logistic Regression and Naive Bayes showed lower accuracy.


* To further improve the accuracy of the top three algorithms, we applied hyperparameter tuning using GridSearch Cross Validation:


* Decision Tree Classifier: We tuned hyperparameters like max depth, minimum samples per leaf, and the splitting criterion (gini or entropy) to find the best configuration that maximizes accuracy.


* Random Forest Classifier: For Random Forest, we optimized hyperparameters such as the number of trees (n_estimators), maximum depth of trees, minimum samples per leaf, and the splitting criterion.


* XGBoost Classifier: In XGBoost, we tuned parameters like the learning rate, number of boosting rounds (n_estimators), maximum depth of trees, and the regularization parameters (gamma and lambda).


* After hyperparameter tuning, the XGBoost Classifier achieved the highest accuracy of 72%.
