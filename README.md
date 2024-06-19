# SMS-Spam-Classifier 

# Introduction
This project involves the classification of SMS messages as either "ham" (legitimate) or "spam" using various machine learning techniques. The dataset used is the "SMSSpamCollection.tsv", which contains labeled SMS messages and is a realtime dataset.

# Dataset
The dataset smsspamcollection.tsv is a tab-separated values file with two columns:

1. label: Indicates whether the message is "ham" or "spam".
2. message: The content of the SMS message.

# Prerequisites
1. Python 3.x
2. pandas
3. numpy
4. scikit-learn
5. matplotlib

# Code Overview
1. Loading and Exploring the Data
2. Load the data using pandas and display the first few rows.
3. Check the length of the dataset.
4. Check for missing values.
5. Explore the distribution of the labels (ham/spam).
6. Data Visualization
7. Visualize the length of messages for ham and spam using histograms.
8. Visualize the punctuation counts in messages for ham and spam.
9. Data Preparation
Split the data into training and testing sets.
X: Features (message length and punctuation count).
y: Labels (ham/spam).
10. Model Training and Evaluation
a) Logistic Regression:Train a logistic regression model.Evaluate the model using a confusion matrix, classification report, and accuracy score.
b) Naive Bayes:Train a Naive Bayes classifier.Evaluate the model using a confusion matrix, classification report, and accuracy score.
c) Support Vector Machine (SVM):Train an SVM classifier. Evaluate the model using a confusion matrix, classification report, and accuracy score.
11. Feature Extraction from Text. Reload the dataset.
12. Split the data into training and testing sets.
13. Use CountVectorizer to convert text messages into a matrix of token counts.
14. Use TfidfTransformer to transform the count matrix to a normalized tf-idf representation.
15. Combine the CountVectorizer and TfidfTransformer steps using TfidfVectorizer.
16. Model Training with Text Features
17. Train a LinearSVC classifier using the tf-idf features.
18. Build a pipeline that includes tf-idf vectorization and the classifier.
19. Evaluate the model using a confusion matrix, classification report, and accuracy score.

# Results
Using the text of the messages, the final model performed exceedingly well, correctly predicting spam with an accuracy of 98.97%.

# Conclusion
This project demonstrates the process of building and evaluating several machine learning models for SMS spam detection. It also highlights the importance of feature extraction from text data for improving model performance.

# Contact
If you have any questions or feedback, please contact Jugal Deshmukh at mrjugaldeshmukh@gmail.com.

This README file provides a detailed overview of your project, from prerequisites and installation to usage and a brief code explanation.
