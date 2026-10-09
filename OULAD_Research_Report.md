
# Early Prediction of At-Risk Students Using Learning Analytics

## 1. Introduction

Student disengagement and course withdrawal are important
challenges in online education. Learning analytics can help
identify students who may fail or withdraw by examining
their early engagement with online learning resources.

This project uses the Open University Learning Analytics
Dataset (OULAD) to investigate whether student activity
during the first four weeks can help predict academic risk.

## 2. Research Objective

The objective is to investigate whether early online
learning activity can help predict students who are likely
to fail or withdraw from a course.

Students with final results of Fail or Withdrawn are
classified as at risk. Pass and Distinction are classified
as not at risk.

## 3. Dataset and Features

The project uses student information and Virtual Learning
Environment (VLE) activity data.

The dataset contains 32,593 student records. Early activity
features are calculated using VLE data from days 0 to 27.

The features include:
- Early total clicks
- Number of active days
- Number of unique learning sites accessed
- Clicks during weeks 1-2
- Clicks during weeks 3-4

## 4. Methodology

The data is divided into training and testing sets using
an 80:20 split, with stratification by the target class.

A Neural Network model is evaluated using three features.
A second Neural Network uses five features. A Random Forest
model is also evaluated using the five features.

Model performance is assessed using accuracy, precision,
recall, and F1-score.

## 5. Preliminary Results

The five-feature Random Forest model achieved:
- Accuracy: 65.32%
- Precision: 67.31%
- Recall: 66.71%
- F1-score: 67.01%

Among the five features, clicks during weeks 3-4 had the
highest Random Forest feature importance (approximately
25.27%).

These results are preliminary and should be interpreted
with consideration of the models' moderate predictive
performance and the overlap between activity features.
