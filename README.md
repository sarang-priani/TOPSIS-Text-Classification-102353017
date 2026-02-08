readme = """
# TOPSIS for Text Classification Model Selection

## Overview
This project applies the TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) method to
select the most suitable text classification model based on multiple evaluation criteria. The goal is to
make a balanced decision rather than relying only on accuracy.

This work is done as part of an academic assignment for Text Classification (roll number ending with 7).

## Models Considered
The following models are compared in this study:
- Logistic Regression
- Support Vector Machine (SVM)
- Naive Bayes
- Random Forest

These models are commonly used for text classification tasks.

## Evaluation Criteria
The models are evaluated using four criteria:
- Accuracy (benefit criterion)
- F1-score (benefit criterion)
- Inference Time (cost criterion)
- Model Size (cost criterion)

Accuracy and F1-score represent performance, while inference time and model size represent efficiency.

## Methodology
TOPSIS is applied using the following steps:
1. Creation of a decision matrix
2. Normalization of the matrix
3. Assignment of weights to each criterion
4. Identification of ideal best and ideal worst solutions
5. Calculation of distance from ideal solutions
6. Computation of TOPSIS score and ranking

The model with the highest TOPSIS score is selected as the best overall model.

## Results
Based on the TOPSIS score, the models are ranked according to their overall performance.
Graphs are used to compare accuracy, inference time, and the final TOPSIS score.

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

## Conclusion
This project demonstrates that model selection based on multiple criteria provides a more practical
solution than using a single metric. TOPSIS helps in selecting a model that balances performance
and computational efficiency.
"""

print(readme)
