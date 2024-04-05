# DishHealthPredictor 🍽️

Welcome to DishHealthPredictor! This project aims to predict the healthiness rating of various dishes based on attributes such as ingredients, diet, home or restaurant preparation, and likeness.

## Transformation Stage 🔄
In this stage, we utilize the Random Forest classifier to reduce the dimensions of the features. By setting the important feature threshold to 0.01, we effectively narrow down the initial 1633 columns to 22 significant ones.

## Modelling 🤖
Employing ensemble techniques and grid search, we determine the best parameters and models among Random Forest, Support Vector Classifier (SVC), and logistic regression. These models are well-known for their effectiveness in classification problems.

## Methodology 📊
We adopt an 80:20 split on the entire dataset for training and testing. The models are trained on the training dataset using various classification algorithms. Performance metrics such as accuracy scores, confusion matrices, precision, and recall are evaluated on both training and test datasets.

## Dataset 📑
Test data is utilized for making predictions. We utilize a sample dataset and present a correlation matrix of the extracted features for reference.

## Conclusions 📝
While we've implemented feature extraction and feature reduction transformations and built models using various classification algorithms, there's room for improvement in model accuracy and performance. Despite attempts to extract features from images such as texture and color, the models did not significantly improve. Surprisingly, using attributes solely from the CSV file yielded better results. Thus, we've focused solely on the CSV data for the classification model submission.

Future work could focus on extracting more useful features from images and employing complex Convolutional Neural Network (CNN) models. However, it's crucial to note that CNN architectures require a deeper understanding of deep learning modeling and may introduce complexity to the project.
