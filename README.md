# AI/ML Project - Credit Card Fraud Detection 💳

<p align="center"><img src="https://user-images.githubusercontent.com/54996245/147120008-9ef5f88f-6b99-42ec-84e1-cca391ec5aa8.jpg" style="width: 1000px;"/></p>

### Description:

It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

### Acknowledgements:
This dataset has been referred from Kaggle: \
https://www.kaggle.com/mlg-ulb/creditcardfraud

### Objective:
- Understand the Dataset & cleanup (if required).
- Build classification model to predict weather the the transaction is fraudulent or not.
- Also fine-tune the hyperparameters & compare the evaluation metrics of vaious classification algorithms.

### Stractegic Plan of Action:
**We aim to solve the problem statement by creating a plan of action, Here are some of the necessary steps:**
1. Data Exploration
2. Exploratory Data Analysis (EDA)
3. Data Pre-processing
4. Data Manipulation
5. Feature Selection/Extraction
6. Predictive Modelling
7. Project Outcomes & Conclusion

### Some Visuals of the Project:

**1. Target Variable Distribution**
  
<p align="left"><img src="https://user-images.githubusercontent.com/54996245/147120205-c9ff7616-cabf-43a8-846f-f07e8213ac52.png" /></p>

<!--**2. Categorical Feature-set Distribution**-->
**Fraudulent Transactions for various amounts across timstamps

![image](https://user-images.githubusercontent.com/54996245/147120339-12cd6961-6f16-4664-b03b-164d7b75310d.png)

**3. Numerical Feature-set Distribution**

![image](https://user-images.githubusercontent.com/54996245/147120356-504e0242-7f82-4a87-bfe4-ba54d42d5ac0.png)
![image](https://user-images.githubusercontent.com/54996245/147120372-b30cbae3-97f8-42e8-bbc2-6cb0022370d3.png)

**4. Relationship between the Feature-set**



**5. Data Retention after preforming preprocessing step**

![image](https://user-images.githubusercontent.com/54996245/147120409-f4e7b0f7-a4ff-4398-9e1f-ba2e87c12dc8.png)

**6. Correlation plot for features**

![image](https://user-images.githubusercontent.com/54996245/147120437-017c2e86-03c8-4def-b599-b9c3f680638f.png)

**7. VIF & RFE Scores & PCA Decomposition**
  
![image](https://user-images.githubusercontent.com/54996245/147120457-51fc6718-fb59-4125-a4ac-a3b33aa890dd.png)
![image](https://user-images.githubusercontent.com/54996245/147120467-c9db4036-7aa6-473e-aa61-196fb919dec8.png)
![image](https://user-images.githubusercontent.com/54996245/147120482-6654c0db-87a7-4748-b233-d70bbb1e981f.png)
![image](https://user-images.githubusercontent.com/54996245/147120507-ab3e880f-333e-491a-9d2a-f31564395014.png)

**8. ROC Plots**

![image](https://user-images.githubusercontent.com/54996245/147120537-f90d6450-4ded-42f2-a6c7-06d0e91a3598.png)

**9. Tree Plot & Feature Importance in Random Forest
  
![image](https://user-images.githubusercontent.com/54996245/147120559-55c2a1a5-0061-4d2f-b8e1-3d034ee2efb6.png)
![image](https://user-images.githubusercontent.com/54996245/147120576-6ef9c12c-b1e2-4506-860a-ad519a491b0b.png)


**10. ML Algorithm's Scores for the Dataset**
  
![image](https://user-images.githubusercontent.com/54996245/147120612-8812ebc7-4c15-4361-868c-642e996d7328.png)
![image](https://user-images.githubusercontent.com/54996245/147120629-1598c250-dbf7-44ef-8626-d1bdc67dd454.png)

  
### Here are some of the key outcomes of the project:
- The Dataset was quiet large totalling around 28Lakh samples & after preprocessing 34.6% of the datasamples were dropped. 
- The samples were highly imbalanced after processing, hence SMOTE Technique was applied on the data to  balance the classes, adding 21.7% more samples to the dataset.
- Visualising the distribution of data & their relationships, helped us to get some insights on the relationship between the feature-set.
- Feature Selection/Eliminination was carried out and appropriate features were shortlisted.
- Testing multiple algorithms with fine-tuning hyperparamters gave us some understanding on the model performance for various algorithms on this specific dataset.
- The Boosting & Random Forest Classifier performed exceptionally well on the current dataset, considering Recall Score as the key-metric.
- Yet it wise to also consider simpler model like Logistic Regression as it is more generalisable & is computationally less expensive, but comes at the cost of slight misclassifications.

