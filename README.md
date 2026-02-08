
# TOPSIS-Based Model Selection for Text Classification
Roll No: 102353017

## Overview
This project focuses on selecting the best text classification model using the
TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) method.
Instead of choosing a model based only on accuracy, multiple criteria are used
to make a balanced decision.

The models are first trained and evaluated, and then TOPSIS is applied on the
obtained results.

## Dataset
A subset of the 20 Newsgroups dataset is used for experimentation.
The following two categories are selected:
- rec.sport.hockey
- sci.space

The dataset is divided into training and testing sets.

## Models Trained
The following text classification models are trained and evaluated:
- Logistic Regression
- Support Vector Machine (SVM)
- Naive Bayes
- Random Forest

TF-IDF is used for text feature extraction.

## Evaluation Criteria
Each model is evaluated using the following criteria:
- Accuracy (benefit criterion)
- F1-score (benefit criterion)
- Inference Time (cost criterion)
- Model Size (cost criterion)

Accuracy and F1-score measure classification performance, while inference time
and model size represent computational efficiency.

## Methodology
The TOPSIS method is applied using these steps:
1. Train models and calculate evaluation metrics
2. Construct the decision matrix
3. Normalize the decision matrix
4. Apply weights to each criterion
5. Identify ideal best and ideal worst solutions
6. Compute distances from ideal solutions
7. Calculate TOPSIS score and rank the models

The model with the highest TOPSIS score is selected as the best overall model.

## Results
Based on the TOPSIS score, the models are ranked according to their overall
performance. Graphs are generated to compare accuracy, inference time, and
final TOPSIS scores.

## Tools Used
- Python
- Google Colab
- Scikit-learn
- Pandas
- NumPy
- Matplotlib

## Conclusion
This project shows that selecting a model using multiple criteria provides a
more practical evaluation than relying on a single metric. TOPSIS helps in
choosing a model that balances performance and computational efficiency.





