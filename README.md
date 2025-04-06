# Breast_cancer_detection
                        




The Breast Cancer Wisconsin dataset is made up of features extracted from a digitalized image of a fine needle aspirate (FNA) of the breast tumor.There are 569 entries in the dataset. Independent variables include measures such as radius, texture, perimeter, and smoothness and the dependent variable includes tumors being classified as malignant or benign.

**Steps for ML project:**

**Data Preprocessing:**
*  Step 1: Data preprocessing and found out that our dataset has no null values and duplicate values.
*  Step 2: There is "Diagnosis" category column in the dataset. Since the output only contains two sorts of classes benign and malignant ,we have to execute label encoding in order to transform it into a numerical column. Similar to how label encoding gives each category a distinct integer number. Even though we should have used one-hot encoding for our nominal categorical column, we tried both and discovered that label-encoding was more efficient. Here Malignant (M) is considered as 1 and Benign (B) is considered as 0
* Step 3: In this project, applying min-max scaling to numeric features ensures that all variables are uniformly scaled between 0 and 1, which makes it easier for the model to understand and make predictions.

**Model Selection:**
This is a classification algorithm and The model is using KNN algorithm as we have learnt only KNN and we have more practice in using KNN

**Confusion Matrix:**

The confusion matrix provides a tabular summary of the model's predictions versus the actual labels in the test dataset.
The first row and first column represents the actual instances and predicted instances of the benign class (0).
The second row and second represents the actual instances and predicted instances of the malignant class (1).

**This confusion matrix indicates:**
True Negatives (TN): 139 instances were correctly predicted as class 0.
False Positives (FP): 1 instance was incorrectly predicted as class 1.
False Negatives (FN): 7 instances were incorrectly predicted as class 0.
True Positives (TP): 81 instances were correctly predicted as class 1.

The false prediction in the model might be because the dataset is hard to understand, or maybe because of the selection of algorithm.

**Classification Report:**

The classification report provides a summary of Evaluation metrics, including precision, recall, F1-score, and support, for each class (0 and 1).

**For each class, the report provides:**
Precision for benign (class 0) is 95% and for malignant (class 1) is 99%.
Recall for benign is 99% and for malignant is 92%.
F1-score for benign is 97% and for malignant is 95%.
Accuracy is 96.49%, indicating overall model performance.

The precision, recall, and F1-score for both benign (class 0) and malignant (class 1) cases are relatively high, indicating that the model is making accurate predictions for both classes.
The accuracy of 96.49% is also high, suggesting that the model's overall performance is good.


**Conclusion:**

The breast cancer prediction model is performing good. It's highly accurate and can effectively distinguish between benign and malignant cases with great precision. This indicates its reliability and ability to assist doctors in identifying cancerous tumors more accurately.
