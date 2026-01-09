# Insurance-uptake-classification-

Motivation

We all know that "Acquiring a new customer is 5x more costly than retaining the existing ones". Then why not focus on doing more business with existing customers, leveraging their trust and further strengthening it. Ultimately, reducing the marketing cost and building a loyal customer base.

Overview

The objective is to effectively predict interested customers in purchasing vehicle insurance from the already existing customer base of Health insurance, so that targeted marketing strategies could be implemented. The dataset has 1,00,000+ rows with features like age, gender, previous insurance, annual premium, etc.

During EDA, I found class imbalance where only a small percentage of customers were actually interested in insurance. I handled outliers and duplicate observations to improve model stability.

To handle class imbalance, I used SMOTE / class weights and trained models like Logistic Regression, Naive Bayes, Random Forest and XG-Boost. While evaluation I focused on the recall of the positive class, which also happened to be the minority class, because maximizing detection of interested customers is more important than overall accuracy.

The best performance was achieved with the Logistic Regression with 87% recall, 79% accuracy and 0.70 AUC-ROC. I chose Logistic Regression for the best recall and simpler explanation and stable calibration. The model is significantly helpful in identifying potential buyers, reducing marketing cost and improving conversion rates.

Why is Recall so important here

I have prioritized identifying customers who would actually purchase the insurance because missing a potential customers means lost sales and lost revenue, a loss. So what exactly is recall in this case? Recall measures how many of the potential customers have been correctly identified by the model. In other words, among all the customers who would actually be interested in purchasing insurance, how many did the model identify correctly.
