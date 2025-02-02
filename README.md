# Credit-Card-Fraud-Detection
![Alt text](CCFD.png?raw=true "Title")
### Data Source: https://www.kaggle.com/mlg-ulb/creditcardfraud/data
It is a CSV file, contains 31 features, the last feature is used to classify the transaction whether it is a fraud or not. 
### Information about data set
* The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
* It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues original features are not provided and more background information about the data is also not present. Features V1, V2, ... V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.
* Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.
* I think RECALL score is the most important metric here since the goal is to correctly classify frauds as frauds. Even if non-frauds are predicted frauds won't harm much as they will be under suspect but if frauds are predicted non-frauds then that is where the model fails.
* The dataset has been collected and analysed during a research collaboration of Worldline and the Machine Learning Group (http://mlg.ulb.ac.be) of ULB (Université Libre de Bruxelles) on big data mining and fraud detection.
## Flow of Project
* Exploratory Data Analysis on full data and also deal with Outliers. 
* Dataset is highly imbalance, applied Undersampling technique to deal with this imbalance. 
* Used Logistic Regression and Decision Tree techniques to predict to train the data and to predict whether the transaction is Fraud or not. 
* Also applied Recursive Feature Elimination(RFE) technique for selecting features that are more relevant in predicting the target variable.
## Quick Results
#### Important Features
![Alt text](Important_Features.png?raw=true "Title")
#### Precision-Recall Curve After Undersampling data
![Alt text](Precision-Recall_Curve.png?raw=true "Title")
### How to Run the Project
In order to run the project just download the data from above mentioned source then run the file.
### Prerequisites
You need to have installed following softwares and libraries in your machine before running this project.
* Python 3
* Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy, scipy.
### Installing
* Python 3: https://www.python.org/downloads/
* Anaconda: https://www.anaconda.com/download/
## Authors
Nilesh Deshmukh - Complete work
## Acknowledgments
Data Science & Business Analytics Course

