# mic_round1
IMDb Sentiment Classification

This project aims to classify IMDb movie reviews as either positive or negative using classical machine learning models. The dataset contains 50,000 reviews, each labeled with its sentiment.


**Dataset**

Source: IMDb movie reviews

Size: 50,000 rows

Columns:

review: the text of the movie review

sentiment: label (positive or negative)



**Approach**

The overall workflow can be summarized in three main stages:

Preprocessing the text

1.Removed HTML tags, numbers, and special characters.

2.Converted all text to lowercase.

3.Removed extra whitespaces.

4.Dropped duplicates and rows with missing values.

5.Converted sentiment labels into numeric format (positive → 1, negative → 0).



**Feature extraction**

Applied TF-IDF vectorization to convert raw text into numerical vectors .



**Models Implemented**

1.Logistic Regression

2.Support Vector Machine (SVM)

3.Random Forest

4.XGBoost

5.Naive Bayes 



**Evaluation Metrics**

1.Accuracy

2.Precision

3.Recall

4.F1-score

5.Confusion Matrix



**Results** 

| Model               | Accuracy | Precision | Recall | F1-score |
| ------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression | 0.9006   | 0.8959    | 0.9074 | 0.9016   |
| SVM                 | 0.9006   | 0.9014    | 0.9003 | 0.9009   |
| Random Forest       | 0.8581   | 0.8569    | 0.8612 | 0.8590   |
| XGBoost             | 0.8704   | 0.8578    | 0.8893 | 0.8732   |
| Naive Bayes         | 0.8695   | 0.8650    | 0.8768 | 0.8709   |

Logistic Regression and SVM achieved the best overall performance (~90% accuracy and F-1 score).

Random Forest and XGBoost did not outperform the linear models.
