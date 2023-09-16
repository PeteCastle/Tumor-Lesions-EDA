# FDG-PET/CT Dataset for Tumor Lesions
## Exploratory Data Analysis

This exploratory data analysis analyzes the characteristic of tumor lesions across 197 cancer patients. Then, I used Principal Component Analysis to reduce the features from >400 to less than 20.  Feature normalization is also used.  Then, I used and compared 5 models: Logistic Regression, Random Forest Classifier, Gradient Boost Classifier, Support Vector Classifier, KNeighbors Classifier.  The following scores were used for model evaluation: Best Score, Accuracy, F1 Score, and ROC AUC Score.

**The Dataset**

Dataset is obtained from [this source](https://coursebank.ph/assets/courseware/v1/4bf7bc69429d39dee06cb120e862b464/asset-v1:DAP+SP901+2020_Q2+type@asset+block/SP901_CS_completedata.csv).
Each row represents a tumor lesion. Each column represents a feature of the tumor lesion such as volume, axis length, SUV, etc.

**Results and Conclusion**

| Model             | Best Score | Accuracy  | F1 Score  | ROC AUC Score |
|-------------------|------------|-----------|-----------|---------------|
| Logistic Regression | 0.783095   | 0.692308  | 0.666667  | 0.696296      |
| Random Forest       | 0.870000   | 0.769231  | 0.777778  | 0.768889      |
| KNN                 | 0.832381   | 0.807692  | 0.821429  | 0.805926      |
| SVC                 | 0.835952   | 0.826923  | 0.808511  | 0.831852      |
| Gradient Boosting   | 0.855238   | 0.788462  | 0.800000  | 0.787407      |


Among the models listed, the **Random Forest model** achieved the highest "Best Score" of 0.87, suggesting it performed the best overall according to the chosen evaluation metric, but suffers from precision and recall scores.

KNN and SVC also achieved relatively high scores, both in terms of accuracy, F1 score, and ROC AUC score.

However, logistic regression performed poorly, suggesting that the data is not linear in nature.

https://github.com/PeteCastle/Hospitality-and-Location-Dataset/raw/main/resources/images/2023-08-26-19-05-32.png

**Francis Mark M. Cayco**

https://github.com/PeteCastle

*SP901: Data Science and Machine Learning Using Python*

*Capstone Project*
