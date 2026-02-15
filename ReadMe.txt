MSCS 634 – Lab 2: KNN and Radius Neighbors Classification Using the Wine Dataset
Overview

This lab explores the performance of two machine learning classification algorithms—K-Nearest Neighbors (KNN) and Radius Neighbors (RNN)—using the Wine dataset from the scikit-learn library. The goal is to understand how different hyperparameter values (k and radius) influence model accuracy and how to visualize these accuracy trends for comparison. This hands-on work provides practical exposure to data loading, train-test splitting, model training, evaluation, and performance visualization.

Objectives

Load and explore the Wine dataset

Implement KNN with different k values

Implement RNN with different radius values

Record and compare model accuracies

Visualize accuracy trends for both algorithms

Form conclusions on model performance and parameter behavior

Steps Completed in the Lab
1. Dataset Loading and Preparation

Loaded the Wine dataset using sklearn.datasets.load_wine()

Converted data into a Pandas DataFrame for exploration

Observed feature details and class distribution

Split data into 80% training and 20% testing

2. K-Nearest Neighbors (KNN) Implementation

Implemented KNN using the following parameter values:
k = 1, 5, 11, 15, 21

Trained each model on the training set

Calculated accuracy using the test set

Logged accuracy for each k-value

Plotted accuracy results to visualize trends

3. Radius Neighbors (RNN) Implementation

Implemented RNN using radius values:
350, 400, 450, 500, 550, 600

Trained each RNN model

Evaluated classification accuracy

Recorded accuracy for comparison

Created a plot showing accuracy vs. radius value

4. Visual Comparison

Generated visual plots for both algorithms

Compared stability, sensitivity, and accuracy differences between KNN and RNN

Noted when one model outperforms the other and why

Key Insights

KNN Accuracy Trends:
Lower k-values (e.g., k = 1 or 5) tend to perform better because they rely on highly localized patterns. Higher k-values may smooth out decision boundaries too much, leading to slight accuracy drops.

RNN Accuracy Trends:
RNN accuracy is highly dependent on choosing an appropriate radius.
Too small → not enough neighbors to classify
Too large → decision boundary becomes overly generalized

Model Comparison:
KNN showed more stable and predictable behavior.
RNN performance varied more widely and was more sensitive to the chosen radius.

Files Included

Lab2_KNN_RNN.ipynb – Jupyter Notebook containing full code and visualizations

/screenshots/ – Folder containing all required screenshots

README.md – Documentation of purpose, results, and insights

Challenges Faced

Selecting radius values that avoid RNN errors (e.g., no neighbors within radius)

Ensuring accuracy plots clearly reflect performance differences

Understanding how parameter changes affect decision boundaries

Conclusion

This lab demonstrated the practical differences between KNN and RNN classifiers and how hyperparameter selection directly impacts model accuracy. Through visualization and comparison, it became clear that KNN generally provides more consistent performance, while RNN requires careful tuning of radius values. The hands-on approach helped reinforce concepts related to supervised learning, parameter tuning, and model evaluation techniques.