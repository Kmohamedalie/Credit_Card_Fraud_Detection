# Credit Card Fraud Detection   

### **Task:** Examples represent 1 and 0 instances of Fraudulent and Genuine Transaction of European customers.
### **Trained Model:** 
[Model](), Training Time: 37min 21s,  Accuracy: 100% but note that 99.8% of the transactions were Genuine and 0.1667% were Fraudulent, so it likely that 99% of the time the model will predict the transaction as Genuine. So it is better we focus on other metrics such as f1-score (Genuine: 100%, Fraud: 87%), precision (Genuine: 100%, Fraud: 95%) and recall (Genuine: 100%, Fraud: 81%) since the dataset is imbalanced.
### **Dataset available on:** [Kaggle Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

**Developers' Guide:** [Amazon Machine Learning](https://docs.aws.amazon.com/pdfs/machine-learning/latest/dg/machinelearning-dg.pdf#cross-validation),  [Google Machine Learning Education](https://developers.google.com/machine-learning)                                            
**Link to the notebook:** Credit Card Fraud Detection -[xgboost](https://github.com/Kmohamedalie/Credit_Card_Fraud_Detection/blob/master/Notebook/Credit_Card_Fraud_Detection_XGBOOST_%26_GridSearchCV.ipynb)



![image](https://github.com/Kmohamedalie/Credit_Card_Fraud_Detection-SVM/assets/63104472/8219a470-ff04-4689-89d8-f73dcce764f5)

### About Dataset: <br>
### Context: <br>
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

### Content: <br>
The dataset contains transactions made by credit cards in September 2013 by European cardholders.  <br>
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is <br> highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.  <br>

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we  <br> 
cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal   <br>
components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time'  <br>
contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction   <br>
Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes     <br> 
value 1 in case of fraud and 0 otherwise.  <br>

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC).  <br>
Confusion matrix accuracy is not meaningful for unbalanced classification.  <br>
