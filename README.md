# Early Prediction of At-Risk Students Using Learning Analytics

## Overview
This project investigates whether early online learning activity
can help predict students who may fail or withdraw from a course.

## Dataset
The project uses the Open University Learning Analytics Dataset
(OULAD), including student information and VLE activity records.

- Student records: 32,593
- VLE activity records: approximately 10.65 million
- Early activity window: days 0-27

## Features
- Early total clicks
- Early active days
- Unique learning sites accessed
- Clicks during weeks 1-2
- Clicks during weeks 3-4

## Models
1. Neural Network with three features
2. Neural Network with five features
3. Random Forest with five features

## Preliminary Results

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Neural Network (3 features) | 65.19% | 68.68% | 62.64% | 65.52% |
| Neural Network (5 features) | 65.19% | 69.01% | 61.85% | 65.24% |
| Random Forest (5 features) | 65.32% | 67.31% | 66.71% | 67.01% |

The five-feature Random Forest achieved the highest F1-score among
these three experiments. Its overall accuracy was 65.32%, so the
predictive performance remains moderate.

## Feature Importance
The most important feature in the Random Forest model was clicks
during weeks 3-4 (approximately 25.27%).

## Limitations
The results are preliminary. The activity features overlap, and
feature importance does not establish causation. Further validation,
baseline comparisons, and careful evaluation are needed.

## Tools
- Python
- Pandas
- Scikit-learn
- Google Colab

## Research Report
See `OULAD_Research_Report.md` for the initial research report.
